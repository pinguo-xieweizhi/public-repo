# 告警日志记录

| 服务名 | 日志错误信息 | traceId | 原因 | 处理方式 | 时间 |  负责人 | 状态 |
| --- | ---- | ---- | ---- | ---- | --- | ---- | ---- |
|  operations-placing-mgr-bff    |    connection reset by peer  |   ceae9f44d2c463e4fb4837e84a78d092   |    可能是由于网络不稳定导致 或 数据库负载过高中断连接  |  原因未确定，且不好定位，暂未处理    | 2024-09-25T16:32:24+08:00 | 谢伟志 | 持续跟进 |
|  operational-materials    |    connection reset by peer  |   67918a66e0643e912f912dca0a2123ee   |    可能是由于网络不稳定导致 或 数据库负载过高中断连接  |  原因未确定，且不好定位，暂未处理    | 2024-09-25T06:29:41+08:00 | 谢伟志 | 持续跟进 |
|   cdp-usergroup   |  runtime error   |      |   空指针异常    |   https://github.com/pinguo-icc/cdp-usergroup-svc/pull/61   | 2024-09-25T15:50:33+08:00 |  谢伟志 | 待发版 |
|  iam-svc    |   connection(10.0.2.230:3717[-43]) failed to write: context canceled  |    a93f5693774d6c42e6bd6be908039e24  |   上下文被取消    |   联系运维屏蔽即可（待处理）   | 2024-09-25T11:29:59.875930759+08:00 | 谢伟志 | 待联系运维处理 |
|   operational-product-svc   |  no documents in result   |   f5e62d2dd196e2979bdb3bedfc0dddaa   |   当位置不存在任何上架的计划会返回 mongo.NoDocumentErr    |   返回自定义 error https://github.com/pinguo-icc/placing-svc/pull/104/files  | 2024-09-25 11:27:33  | 谢伟志 | 发版，已处理 |
|   bmall-bff   |  "subCode\":404,\"message\":not found   |   6c87a9bcddc4731444c4692e4b7132f1   |   从bmall 获取商品失败或超时    |  bmall 有些时候获取不到商品，据古sir说应该是某些服务器上的代码还是老代码    | 2024-09-26T01:53:43 | 古忠志 | 持续跟进 |
|  bmall-bff  |  order not ship, try again later   |   942122e3c0cfb9785a8d8f93a3521837   |   检查发货，订单在指定的循环次数后未发货则会提示    |  暂不处理，会重新发货    | 2024-09-25T23:08:45 | 无 | 不处理 |
|  video-beats-cli    | ERROR WatchRegionData    |    无  |    无   |   不用处理   | 2024-09-25T01:53:43 | 王平 | 不处理 |
|  operational-materials    |  AutoRefresh.FieldDefinition:"rpc error: code = DeadlineExceeded desc = context deadline exceeded"   |  ec7ee3640a8292242993093ddf25c22e 与 无     |  刷新字段表缓存 超时    |   原因未确定，有可能是竞争锁，或者访问数据库超时，暂时打印日志跟踪一下 https://github.com/pinguo-icc/field-definitions-svc/pull/319  | 2024-09-25T04:52:37 | 谢伟志 | 需跟进 |
|  transaction-svc    |  deviceID不能为空   |   d28ab575e9c2be5a26ef0ef89b0effbc   |   订单手动查询用户会员信息未判断参数导致    |  增加入参判断    |  2024-09-28T16:18:45 | 谢伟志 | 已处理，待与关联用户一起发版 | 
|  push-go    |   FCM v2 send result:  |  无    |   请求 https://fcm.googleapis.com/v1/projects/%s/messages:send 出现503    |   暂不处理，可能为对方服务器负载过高  | 2024-09-26 17:06:19  | 谢伟志 | 持续跟进，或联系运维降级 |
|   push-go   |  参数错误   |   66f38606acb6148248c77683   |   参数错错误类的日志级别设置的是error  |   做降级处理，https://github.com/PGWireless/dispatcher-go/pull/602   | 2024-09-25 11:40:54 | 谢伟志 | 待合并代码并发版 |
|   app-camera360   |  参数错误: useId和deviceId不能同时为空   |   3ddf164c8c014b521044d21f1cd0d48b   |   请求的设备id是不合法的id 上报vip信息接口有检验    |   告警规则添加忽略   | 2024-09-28 | 谢伟志 | 待联系运维屏蔽 |
|      |     |      |       |      |
|      |     |      |       |      |
|      |     |      |       |      |
|      |     |      |       |      |
