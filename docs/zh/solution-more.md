# 更多...

下面每一个方案，都经过实践证明行之有效，希望能够对你有帮助

## 域名绑定

绑定域名的前置条件是：Mattermost已经可以通过解析后的域名访问。  

虽然如此，从服务器安全和后续维护考量，**域名绑定**步骤不可省却  

Mattermost 域名绑定操作步骤：

1. 登录云服务器
2. 修改 [Nginx虚拟机主机配置文件](/zh/stack-components.md#nginx)，将其中的域名项的值 *mattermost.example.com* 修改为你的域名
   ```text
   server {
      listen 80;
      server_name    mattermost.example.com; # 改为自定义域名
   ...
   ```
3. 保存配置文件，重启[Nginx服务](/zh/admin-services.md#nginx)
4. 登录Mattermost控制台，打开：【ENVIRONMENT】>【Web Server】，修改 【Site URL】值
   ![](https://libs.websoft9.com/Websoft9/DocsPicture/en/mattermost/mattermost-urlset-websoft9.png)


## 迁移

暂无
