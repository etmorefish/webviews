* 将教程范例（意见反馈平台DEMO）中的管理端部分的列表加载变成实时数据库监听形式触发。用户端列表加载云函数适配超过100条的场景，采用promise all的形式进行改造，使其可以支持超过100条。

按照init-admin 修改云函数init，在index.js里面使用调用云函数init加载意见列表 admin.js使用tcb-sdk本地调用

> bug:在我使用的会出现谷歌浏览器上会出现未初始化的情况，但是打开一个新的浏览器则没问题, 后续在研究吧
