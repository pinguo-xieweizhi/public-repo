# 告警日志记录

| 服务名 | 日志错误信息 | traceId | 原因 | 处理方式 | 时间 |
| --- | ---- | ---- | ---- | ---- | --- |
|  operations-placing-mgr-bff    |    connection reset by peer  |   ceae9f44d2c463e4fb4837e84a78d092   |    可能是由于网络不稳定导致 或 数据库负载过高中断连接  |  原因未确定，且不好定位，暂未处理    | 2024-09-25T16:32:24+08:00 |
|   cdp-usergroup   |  runtime error   |      |   空指针异常    |   https://github.com/pinguo-icc/cdp-usergroup-svc/pull/61   | 2024-09-25T15:50:33+08:00
|  iam-svc    |   connection(10.0.2.230:3717[-43]) failed to write: context canceled  |    a93f5693774d6c42e6bd6be908039e24  |   上下文被取消    |   联系运维屏蔽即可（待处理）   | 2024-09-25T11:29:59.875930759+08:00 |
|   operational-product-svc   |  no documents in result   |   f5e62d2dd196e2979bdb3bedfc0dddaa   |   当位置不存在任何上架的计划会返回 mongo.NoDocumentErr    |   返回自定义 error https://github.com/pinguo-icc/placing-svc/pull/104/files  | 2024-09-25 11:27:33  |
|      |     |      |       |      |
|      |     |      |       |      |
|      |     |      |       |      |
|      |     |      |       |      |
|      |     |      |       |      |
|      |     |      |       |      |
|      |     |      |       |      |
|      |     |      |       |      |
|      |     |      |       |      |
|      |     |      |       |      |
|      |     |      |       |      |
|      |     |      |       |      |
