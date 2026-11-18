# 红魔助手 3.3.5

相对于原版 **3.3.4（334）** 的修改说明。原开发者 **酷安@卒迹** 保持不变，修改者为 [iammagicc](https://github.com/iammagicc/RedMagicHelper)。


## 与原版的变化

- 从 LSPosed legacy 接口迁移到 **libxposed Modern API 102**，目标框架为 **LSPosed 2.2.1（7912）**；替换模块入口及元数据。
- Hook、反优化和原方法调用改用现代 API；保留原有功能代码及设置界面。
- 设置使用应用私有配置，并通过 libxposed 服务同步到框架远程配置，取消旧式共享配置文件访问。模块激活状态从实际服务连接读取。
- 版本号更新为 **3.3.5**，内部版本码 **336**（高于迁移测试版的 335）；关于页面版本显示同步更新。
- 使用新的个人签名。与原作者签名不同，不能直接覆盖原作者签名的安装包。

## 验证范围

迁移版本已在红魔 9 Pro / Android 16 / RedMagicOS 11.0.3 / LSPosed 2.2.1（7912）上分阶段验证，包括配置同步、安装器开关对照、一次重启、状态栏秒数/双行网速/电池信息和最近任务内存显示。

安装包通过 APK v2/v3 签名及 16 KB ZIP 对齐检查。未逐项测试所有功能，也未进行性能、耗电或安全收益的对照测试，不承诺这些指标改善。

本仓库仅提供安装包与本 README 。

APK SHA-256：`519bcc68d48a7496bbf79381342c8b1ff321aad6cf612e4f44cf924aae41509f`

## 参考项目
- https://github.com/LSPosed/dexsql-release
- https://github.com/JingMatrix/Vector
