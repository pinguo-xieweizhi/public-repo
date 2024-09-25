# 数据库迁移说明

| 待迁移数据库名 | 老库实例 | 新库实例 | 数据量 | 使用数据库服务 | 服务发版方式 | 是否运维修改configmap | 是否需要运维迁移数据 |
| ---- | ---- | ----- | ---- | ----- | ----- | ----- | ---- |
| infras-svc | cn-hz-public-40 | cn-hz-public-mongo | 20MB |   pinguo-icc/infras-svc | argo-cd | 是(目前argo-cd发版仓部署文件未配置configmap) | 是 |
| cdp_usergroup | cn-hz-public-40 | cn-hz-public-mongo | 10MB | pinguo-icc/cdp-usergroup-svc | jenkins（jenkins 已禁用且迁移到gitops发版攀哥未搞完） | 是 | 是 |
| cdp-association | cn-hz-public-40  en-sg-public-mix-bmall-pt  | cn-hz-public-mongo   en-sg-public-mongo  | 2MB | pinguo-icc/cdp-association-svc | jenkins（jenkins 已禁用且迁移到gitops发版攀哥未搞完）| 是 | 是 |
| cdp_proxy  | cn-hz-public-40 | cn-hz-public-mongo | 2MB | pinguo-icc/cdp-proxy-svc | jenkins（jenkins 已禁用且迁移到gitops发版攀哥未搞完） | 是 | 是 |
| blind-test | cn-hz-public-40 | cn-hz-public-mongo | 2MB | pinguo-icc/blind-test-svc | jenkins | 是 | 是 |
|  db2s3 |  en-sg-public-mix-bmall-pt  | en-sg-public-mongo | 6MB | pinguo-icc/db2s3 | jenkins | 是 |是 |
|  exchange-rate |  en-sg-public-mix-bmall-pt  | en-sg-public-mongo | 6MB | pinguo-icc/exchangerate-bff  | jenkins | 是 | 是 |
|  foresight  |  en-sg-public-mix-bmall-pt  | en-sg-public-mongo | 100KB | pinguo-icc/foresight-svc  | jenkins | 是 | 是 |
