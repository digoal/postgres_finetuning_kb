# postgres_finetuning_kb
PostgreSQL's knowledge base for LLM fine tuning.  
   
Let's contribute Postgres's QA used for LLM fine tuning.  
  
The goal of this project is to train an expert-level AI small model for PostgreSQL, making it more accessible to a wider audience.  

# 项目收益
1、通过微调之后, 可以产出模型适配文件、发布生成新的模型.  
  
2、新的模型可被广泛应用于DBA的自我革命产品:  
- 助手
- 教学
- 诊断
- SQL审查
- 数据库健康报告解读
- ... 更多模型应用等你发掘.
   
高并发的业务可以启用基于规则判断的产品(类比鳄鱼脑), 低并发的复杂业务可以启用基于AI和推理能力的产品(类比理性脑).
    
# 微调方法
参考: https://github.com/digoal/blog/blob/master/202407/20240724_01.md
   
# 加入我们
这个项目需要大量理论、实践经验丰富的老专家, 以及一些算力投入. 为了让项目更好的运行下去我决定成立一个虚拟组织“DBA发展联盟”, 有兴趣的朋友可以加我的微信拉大家加入组织.  
  
![pic](https://github.com/digoal/blog/raw/master/pic/digoal_weixin.jpg)   
   
# QA reference prompt
生成好的问题和答案参考: 
- https://github.com/digoal/blog/blob/master/202407/20240730_01.md
- https://github.com/digoal/blog/blob/master/202407/20240806_02.md  

据说微调要达到比较好的效果, 至少需要1000条QA. 大家一起加油吧.  
  
## 1、使用模型生成问题和内容  
  
1、Q1 市面上有哪些`PostgreSQL`开源数据库相关的职业或岗位?  
  
2、Q2 要成为一名优秀的`xxx`, 需要掌握哪些知识点?   
  
3、Q3 要考察`PostgreSQL` `xxx`职业或岗位的应聘者是否已深刻掌握`xxx`知识点, 可以提出哪些连贯性问题(每个问题尽可能是对前一个问题的追问和深入探究), 问题的难度请标记为初级、中级、高级.   
请给出问题即可, 不需要给出答案. 问题请以如下开头:   
```  
where is the // 去哪里找资料/代码  
What is // 名词/原理解释  
What is the difference // 热门的差异化对比问题  
why // 为什么  
how to // 怎么做、如何实现、如何解决  
```  
  
## 2、目录格式  
  
```  
job_$name/skill_$name/qa_$level_$number.md    
    
job_职业名称/skill_知识点名称/skill_难度(l|m|h)_问题编号(001).md    
```  
  
  
## 3、QA markdown 文件内容格式  
  
```  
## 职业    
...    
## 知识点    
...    
## 问题难度(l|m|h)    
...
## 关联问题
...  
## 问题    
...    
## 答案    
...    
## 校对信息    
校对人1, 校对时间    
...    
```  
  

