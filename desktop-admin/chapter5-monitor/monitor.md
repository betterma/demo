## 5. 监控告警
### 5.1 监控面板

点击菜单“监控告警” → “监控面板”，可以查看每个数据中心对应的监控面板，点击可以跳转到grafana图形界面，可以查看各种指标。

### 5.2 配置邮箱服务器

邮箱服务器用于发送邮件，例如告警信息、修改密码确认等。目前邮件服务器的配置在“系统配置单数”中管理。  
点击“系统管理”→“配置参数管理”，搜索“STMP服务器配置”，如下图![](/assets/mail.png)  
点击“编辑”，配置邮件服务器参数接口。

![](/assets/mail-edit.png)

**注：目前邮件服务器参数以JSON字符串形式存储，改动的时候不要改动格式。**

### 5.3 接收组

接收组可以配置接收方的邮箱或者办公助手账号  
点击菜单“监控告警”→“接收组”，点击按钮“新增接收组”，填写相关信息即可。

![](/assets/接收组-insert.png)

### 5.4 告警订阅

点击菜单“监控告警”→“告警订阅”，点击按钮“订阅告警”，填写相应的信息即可

![](/assets/订阅告警.png)

![](/assets/告警订阅-insert.png)

### 5.5 查看告警信息

点击菜单“监控告警”→“告警信息”，或者“监控告警”→“告警指标”，查看相应的告警信息。

