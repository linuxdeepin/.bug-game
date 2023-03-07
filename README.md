# .bug-game
“小浣熊杯Bug修复大赛”是在 deepin 员工内部进行的一个小规模比赛，不定期举行。

# 比赛规则
1. 友谊第一
2. 多位研发 + 一位测试组为一个队伍
3. 在规定时间内人均获得积分最多的队伍获胜
4. Bug是否修复以 __其他队伍__ 的测试人员的测试结论为准
5. 比赛中的代码暂不Merge，但是也要进行Review
6. 可以Review其他队伍的代码，如发现解决方案投机取巧，或代码有严重问题，则此修复不算数（打回重新提交代码和测试）
7. 比赛中的Issue先占先得， 先占有Issue再开始修复工作
8. 比赛开始后，会在当前项目中新建一个看板，并且为每一支队伍创建一列（以队伍名称命名）。队伍成员将Issue放置到对应的列则认为占有，__每个队伍同时占有的Issue不得超过队伍中研发人员数量的最大值__
9. 占有Issue时还需将对应的Issue链接发送到比赛时的交流（即时聊天）群中，当多个队伍对同一个Issue的占有有异议时，以群里收到消息的先后顺序为准。所发送的消息格式为：“XXXX队选定：https://github.com/XXXXXXXXXXXXXX”
10. 无法修复的Bug可以放弃，将其移动到看板的“放弃”一列则认为取消占有。 __取消占有后需要在聊天群中发消息告知其他队伍__
11. 比赛开始的标志为在本项目中新建Issue，在Issue中会提供本次比赛的所有信息，包括并不限于比赛开始和结束时间、组队信息、Issue的范围、看板的链接、聊天群的名称等
12. 每修复一个bug积1分
13. 每测试通过3个bug积1分

# 每个角色需要做的事情

## 研发人员

1. 从任务看板中选定Issue，并指派给自己。__注意不要超过每个队伍同时在进行的Issues数量__。
2. 将Issue拖动到看板中对应的列。
3. Bug修复后在群里进行通知。
4. 将放弃修复的Issue拖动到看板中“放弃”一列中，并在群里发消息通知。

## 测试人员

1. 观察群消息，通过回复研发人员的消息选定Issue进行验证。__每人同时只能测试一个Issue__。
2. 在验证通过的Issue中回复“测试通过”，并到聊天群中通知（测试不通过也需要通知）对应的研发人员。
3. 记录自己所验证通过的所有Issues，以及修复它的队伍名称。
