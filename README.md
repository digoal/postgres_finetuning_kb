# postgres_finetuning_kb
PostgreSQL's knowledge base for LLM fine tuning.  
   
Let's contribute Postgres's QA used for LLM fine tuning.  
  
The goal of this project is to train an expert-level AI small model for PostgreSQL, making it more accessible to a wider audience.  
  
# QA reference prompt
https://github.com/digoal/blog/blob/master/202407/20240730_01.md  

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
  


  
