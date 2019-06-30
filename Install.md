# 下载Jenkins， 初始化配置

   1. 下载jenkins.war, 下载地址： [https://jenkins.io](https://jenkins.io)
   2. 启动jenkins, 需要安装Java JDK1.8以上, 使用命令:  `java -jar jenkins`  
    默认启动端口是8080， 使用其他端口启动， 例如9090: `java -jar jenkins -httpPort=9090`
   3. 浏览到 http://localhost:8080（或安装时为Jenkins配置的任何端口），并等待 解锁 Jenkins 页面出现 
   4. 解锁jenkins，一开始需要输入jenkins的密码，这个密码在${user}/.jenkins/secrets/initialAdminPassword
   5. 安装jenkins插件， 一般可以选择推荐安装， 在大陆地区会因为网络缘故导致部分插件安装失败，点击继续就好。（后面可以配置jenkins镜像进行安装）
   6. 设置admin用户的用户名和密码
   7. 配置jenkins镜像： Manage Jenkins > Manage Plugins > Advanced, 将该页面的Update Site设置为: https://mirrors.tuna.tsinghua.edu.cn/jenkins/updates/update-center.json (这个是清华大学的镜像)  
   其他镜像信息： [http://mirrors.jenkins-ci.org/status.html](http://mirrors.jenkins-ci.org/status.html)

