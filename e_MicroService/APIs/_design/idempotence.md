# 幂等性

## Implement
* 悲观锁（for update）
* 乐观锁
* 唯一约束
```md
最优排序：乐观锁 > 唯一约束 > 悲观锁
```

## 实例
```md
支付宝充值功能，如果支付宝同时通知多次，怎么保证幂等性？
```
* 悲观锁
```sql
select * from t_order where order_id = trade_no for update;
```
* 乐观锁
```sql
select * from t_order where order_id = trade_no;
update t_order set status = 1 where order_id = trade_no where status = 0;
//上面的update操作会返回影响的行数num
if (num==1){
 //表示更新成功
 提交事务;
} else {
 //表示更新失败
 回滚事务;
}
```
* 唯一约束
```sql
创建一个表：
CREATE TABLE `t_uq_dipose` (
 `id` bigint(20) NOT NULL AUTO_INCREMENT,
 `ref_type` varchar(32) NOT NULL DEFAULT '' COMMENT '关联对象类型',
 `ref_id` varchar(64) NOT NULL DEFAULT '' COMMENT '关联对象id',
 PRIMARY KEY (`id`),
 UNIQUE KEY `uq_1` (`ref_type`,`ref_id`) COMMENT '保证业务唯一性'
);
对于任何一个业务，有一个业务类型(ref_type)，业务有一个全局唯一的订单号，
业务来的时候，先查询t_uq_dipose表中是否存在相关记录，若不存在，继续放行。
```
```sql
select * from t_uq_dipose where ref_type = '充值订单' and ref_id = trade_no;
try{
 insert into t_uq_dipose (ref_type,ref_id) values ('充值订单', trade_no);
 //提交本地事务：
}catch(Exception e){
 //回滚本地事务;
}
```

## Reference
* [考虑没有分布式锁定与Ben Darfler的幂等性策略](https://www.bennadel.com/blog/3390-considering-strategies-for-idempotency-without-distributed-locking-with-ben-darfler.htm)
