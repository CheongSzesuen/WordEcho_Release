# 测试公告 #4：readAfter 联动（readAfter=test-005）

此公告测试 **readAfter** 功能。

- 点"已阅"后，test-005 会被标记为 dismissed
- **本次启动**：test-005 仍会弹出（因为队列是快照）
- **下次启动**：test-005 不会弹出（被 readAfter dismiss 了）

如果下次启动 test-005 没弹，说明 readAfter 生效。
