# 高可用集群设计

## 特性

- 节点状态为leader，leaderfollower,follower,candidate
- 选举逻辑的，通过对每个节点的硬件配置、网络状况等因素进行自身的打分再上传到算法层进行综合评估，选择最优的节点作为Leader
- 提出副主节点，提前选举好仅次于主节点的节点，当主节点挂掉时，副主节点可以顶替主节点的位置，保证服务的可用性

## 分层架构

- 应用层
- 算法层

## channel

- tickc
- receivec
- propc
- readc
- advanc
