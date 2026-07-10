# 测试公告 #3：有过期日期（expireDate=未来）

此公告测试 **expireDate + remindable** 组合。

- 设了 expireDate（未来日期），公告应正常显示
- 但不应显示"不再提醒"复选框（即使 remindable=true）
- 因为代码逻辑：`remindable && expireDate == null` 才显示复选框

如果没有看到复选框，说明 expireDate 对复选框的抑制生效。
