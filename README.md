# Pipeline
### 此jenkinsfile是一个多分支流水线文件，可以扫描仓库内所有分支的jenkinsfile，如何你需要多分支流水线发布，将此jenkinsfile略微修改即可应用

### 需要安装jenkins插件：kubernetes、Generic Webhook Trigger、Hidden Parameter
### 按你需求更换构建容器，或者将构建工具集成在slave容器内
### 将此jenkinsfile放在需要构建的分支中
### 在gitlab中配置webhook地址，token在jenkinsfile中默认是123.com，如果需要更改请将jenkinsfile中的token改为你需要的token值
    http://jenkins_url:port/generic-webhook-trigger/invoke?token=123.com
