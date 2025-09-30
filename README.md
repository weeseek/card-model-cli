# card-model-cli
Command-line tool based on card (routing) development model

pnpm workspace 管理

## 基础部分
  ### 入口
  * 初始化各类配置
  * 加载框架
  
  ### 框架
  * 初始化
  * 注册全局组件
  * 初始化根组件
  * 渲染主题组件（不同应用可以配置自有的主题）
  * 主题组件内渲染卡片组件（router-view）
  
## 卡片开发部分
  ### 思路
  * 本地生成JSON文件，拦截请求卡片信息，返回该JSON文件
  * 启动服务
  * 拦截根请求， 返回带头部的vue应用（卡片开发、开发配置）
  * 卡片开发路由：加载卡片组件
  * 开发配置路由：配置卡片JSON文件， 生产环境真正的接口返回（数据在管理控制台配置）
