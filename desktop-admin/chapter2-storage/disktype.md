## 2.1 磁盘类型

磁盘类型是运营后台定义的逻辑规则，比较常用的有高速云盘、普通云盘、低速云盘、SSD高速云盘等，给用户创建卷快照时或者创建模板时使用。

针对安全问题，这里可以选择是否加密，但是加密只会对数据盘进行加密，系统盘不会加密，加密会对性能有一定的影响。  
创建磁盘类型的时候可以设置IOPS限速规格，磁盘类型的6项iops指标可以不填写，不填写表示不限速。  
一般填写read\_iops\_sec和write\_iops\_sec即可 ，不限速的情况下read\_iops\_sec大概7000左右 ，write\_iops\_sec大概350左右，可以根据需求填写相应的iops ，write\_bytes\_sec类似于U盘拷贝文件时的速度，注意单位是Bytes ，例如U盘拷贝文件时的速度是30m/s，那这里的数值就是30000000，read\_bytes\_sec是读的速度。  
**参数解释：**

```
read_iops_sec：随机读IOPS,不限速最高7000左右
write_iops_sec：随机写IOPS，不限速情况下最高350左右
total_iops_sec：前面两者的和
read_bytes_sec：顺序读的速度，即每秒读取多少Bytes
write_bytes_sec：顺序写的速度，即每秒写多少Bytes
total_bytes_sec：前面两者的和
```

点击菜单“存储资源”→“磁盘类型”，点击“新建磁盘类型”，创建即可。  
![](/assets/disk_type_insert_a.png)

