消息管理去掉redis
--tag

1、去掉redis

#message 去掉redis

```
add

update

delete

getList

get

reply


wxMessage  sbase:wx:message:info:<msgId>
redis 转 mysql
```


```
message redis 改造

```

改造涉及的地方 swcb  搜寻关键词key  eg:sbase:wx:msg:info:


首页统计 indexStatDao

```

各种key  微信信息关系表   sbase:wx:msg:<weChatId>
event message dialog(与微信直接对话的key)
key 与微信发关键词的消息
collect 收藏关系
reply 微信消息的回复关系
contact 联系人的消息关系
messageDao
增加消息明细   addMessage
setMessageEventDesc 设置消息详情
setMessageProcessed 息处理完后的数据处理

GetMainFansStatistics
```
