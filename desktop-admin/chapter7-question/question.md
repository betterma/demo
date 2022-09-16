
### 1. 给租户关联OS失败

出现这种问题的一般原因是存在同名的域或者项目，给租户分配OS使用，会在os集群创建域（租户名）、项目（租户名-default），可以采用os命令查看，在os的controller节点上操作

```
. admin-openrc
openstack domain list (查看是存在要创建的域)
openstack project list （查看是否存在要创建的项目）
```

如果域存在，请确认要创建的域是否已经被使用，不确认请请教专业人士，不要操作，如果确认可以操作

```
openstack set domain 域名 --disable
openstack domain delete 域名
```

如果存在要创建的项目名，同理，确认可以自己操作的情况下，执行

```
openstack project delete 项目名
```



