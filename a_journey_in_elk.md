# A Journey in ELK

---
## TODO

自动化工具salt

kafka读写message：

*	partition均匀写
*	consumer僵死(logstash)
*	kafka监控

任务调度系统（celery）

logstash

*	用logstash满足各种各样的用户日志归一化需求


Elasticsearch

*	使用script做计算

*	curator好工具

Elasticsearch 非实时数据的聚合思路：

*	非实时的需求-报表需求
*	elasticsearch aggs, 优点(适合经常变化，不固定的聚合需求，用query+aggs很容易满足)，存在的问题：多层aggs, 非实时的聚合，CPU瓶颈。
*	logstash, 通过mutate做字段连接, logstash-filter-metric做event count  优点，局限性(只能满足很少的需求)
*	elasticsearch_aggregator 优点，局限性
*	spark 优点，局限性


业务数据监控：

*	elastalert

*	使用机器学习更准确的监控数据趋势变化

Docker化：

*	目的
链接我之前写的博客。

*	成果，思考：
未来的数据中心，我们需要DCOS.

数据可视化上的思考：

*	更简单易用的UI
思路：kibana 4作为数据可视化基础组件，负责展示图表，kibana 4之上再套一层自己开发的UI，目的是简化数据可视化的配置，主要负责用户点击后生成kibana图表。

*	从配置界面上的可视化元素到模型的总结（运维，基础用户行为分析[渠道转化率，激活量，活跃用户，留存率]，高级用户分析[用户画像，个性化推荐]）

整个架构流程上的思考：

*	吞吐量，延时，丢失率，跨机房

---

### 思考-分享什么？

*	分享我们的技术栈

*	分享我们踩过的坑

*	分享我们开源的软件

### 我的观点

*	未来的机器学习必定是简单易用的，人人都有权利使用机器学习

*	Dcos是未来的data center，

*	容器化是未来云计算的趋势，分享我之前的博文。


> Written with [StackEdit](https://stackedit.io/).