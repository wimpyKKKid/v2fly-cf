# v2fly-cf
简要说明：
1. fork 项目
git.io/JJOUf
复制代码

2. 添加 Secrets
CF_USER_IBM  //账号
CF_PASSWORD_IBM  //密码
CF_CONFIG_URL_IBM  //v2fly服务端配置文件网址，示例：git.io/JJOUG
复制代码

3. 修改 manifest-ibm.yml  （可略过）
name: v2fly
复制代码

4. 修改.github/workflows/deploy-to-ibm.yml，组织和空间 名称： cloud.ibm.com/account/cloud-foundry
cf_org: AwesomeApp
cf_space: Development
复制代码

如果是部署到伦敦节点，修改api地址
cf_api:  api.eu-gb.cf.cloud.ibm.com
复制代码

5. 登录ibm，查看项目域名

6. 登录cloudflare，配置workers，可参考IBMYES

不会写教程，欢迎大神PR 或者 发博客分享介绍

MIT License
