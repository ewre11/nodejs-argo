# 说明
本项目是针对node环境的paas平台或游戏玩具而生，pass平台需要docker部署的才上传Dockerfile,其他玩具平台只需上传index.js和package.json即可。
如果是链接github部署，请先删除REDEME.md说明文件，安全起见，已混淆主代码部分，变量部分自行根据需要修改。

* PaaS 平台设置的环境变量，可在index,js中的13至25行中设置
  | 变量名        | 是否必须 | 默认值 | 备注 |
  | ------------ | ------ | ------ | ------ |
  | URL          | 否 | https://www.google.com     | 项目域名    |
  | PORT         | 否 |  3000  |监听端口，根据不同平台要求设置     |
  | WEB_USERNAME | 否 |  admin |访问list和sub的用户名             |
  | WEB_PASSWORD | 否 |password| 访问list和sub的密码              |
  | UUID         | 否 | de04add9-5c68-8bab-870c-08cd5320df00     |
  | NEZHA_SERVER | 否 |        | 域名+端口，例如nz.aaa.com:5555   |
  | NEZHA_PORT   | 否 |  5555  | 哪吒探针客户端口                 |
  | NEZHA_KEY    | 否 |        | 哪吒探针客户端专用 Key           | 
  | NEZHA_TLS    | 否 |    0   | 默认不启用，若启用请填1           |
  | ARGO_DOMAIN  | 否 |        | argo固定隧道域名                 |
  | ARGO_AUTH    | 否 |        | argo固定隧道json或token          |
  | CFIP         | 否 |skk.moe | 节点优选域名或ip                 |
  | NAME         | 否 |  ABCD  | 节点名称前缀，例如：Glitch，Replit| 

  # 节点
  输出list和sub文件，list文件会在2分钟后自动删除，域名/list或域名/sub查看节点信息。

  # 其他
  本项目已添加自动访问功能，需在第14行中添加项目分配的域名
   replit codesnabox，glitch及很多游戏玩具平台均已测试ok
  # 免责声明
  本程序仅供学习了解, 非盈利目的，请于下载后 24 小时内删除, 不得用作任何商业用途, 文字、数据及图片均有所属版权, 如转载须注明来源。
  使用本程序必循遵守部署免责声明。使用本程序必循遵守部署服务器所在地、所在国家和用户所在国家的法律法规, 程序作者不对使用者任何不当行为负责。
