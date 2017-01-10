---
title: mybatis注意的问题
date: 2017-01-10 16:52:25
tags: [mybatis]
---
mybatis在开发工作中遇到的一些问题，然后记录下来
<!--more-->
#### mybatis返回的map类型的值
当mybatis返回的map值时会过滤掉值为null的key（键）
可以通过配置mybatis-config.xml配置，不过滤

		<configuration>
		<settings>
			<setting name="callSettersOnNulls" value="true"/>
		</settings>
		</configuration>

#### mybatis的配置映射文件中写pl_sql
当报错：
	
	Cause: java.sql.SQLException: ORA-00911: 无效字符
	; bad SQL grammar []; nested exception is java.sql.SQLException: ORA-00911: 无效字符
	] with root cause
	
可以是你的PL_SQL结束时添加“;”，这个结束是必须的分号的

***
** 邮箱：** * 1051165801@qq.com * 
** 微信：** * liu1051165801 *