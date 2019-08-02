# Uda-DA-Projects | 数据分析课程项目

## 简介

本项目(Uda-DA-Projects)为数据分析（入门）课程的Python部分项目合集，项目内提供的均为个人解决方案。

项目内容包括：
1. 探索美国共享单车数据；
2. 探索数据集；
3. 分析A/B测试结果。

如要查看报告，请打开.ipynb或.html。

## 探索美国共享单车数据

本项目使用Python探索美国三大城市（芝加哥、纽约和华盛顿）的自行车共享系统的相关数据。该项目设计目的在于考察Python编写能力，项目结果将以交互式脚本为最终形式。

本项目使用[Motivate](https://www.motivateco.com/)提供的数据集，项目中所用数据为2017年上半年数据，已经过整理，最终三个数据文件都包含核心六列：

* Start Time 起始时间
* End Time 结束时间 
* Trip Duration 骑行时长 
* Start Station 起始车站 
* End Station 结束车站 
* User Type 用户类型 表中Subscriber/Registered为订阅者，Customer/Casual为客户

芝加哥和纽约市文件还包含以下两列：

* Gender 性别 
* Birth Year 出生年份 

## 探索数据集

原始项目共提供了4个不同的数据集供分析，分别是TMDb电影数据，未前往就诊的挂号预约，Gapminder World和FBI 枪支数据。本项目选择了Gapminder World作为探索对象。

[Gapminder World](https://www.gapminder.org/data/)是一个非营利性组织，其建立旨在了解各个地区与国家在社会、经济和环境发展的统计数据与其他信息。本项目使用了Gapminder提供的数据，对数据进行了整理于分析，旨在探索中国的GDP增长率、城市化发展程度、就业率、农业就业人口比例、教育程度之间的变化如何，是否呈现相关性。

文件说明如下：

数据集名称 | 起始年份 | 结束年份 | 数据描述 |
---------- | -------- | -------- | -------- |
gdp_total_yearly_growth.csv | 1801 | 2013 | GDP年度总增长率 |
gdppercapita_us_inflation_adjusted.csv | 1960 | 2017 | 人均国内生产总值 |
agriculture_workers_percent_of_employment.csv |1970|2017 | 农业就业者占总人口比例 |
female_agriculture_workers_percent_of_female_employment.csv | 1991 | 2022 | 女性农业就业者占女性总人口比例 |
male_agriculture_workers_percent_of_male_employment.csv | 1991 | 2022 | 男性农业就业者占男性总人口比例 |
urban_population_percent_of_total.csv | 1960 | 2017 | 城镇人口占总人口比例 |
literacy_rate_adult_total_percent_of_people_ages_15_and_above.csv | 1982 | 2011 | 成人识字率（15周岁以上，含15周岁 |

## 分析A/B测试结果 
本项目设定了一个电子商务网站运营的A/B测试情景，该公司设计了新网站页面，想提高用户转化率，即购买公司产品的用户数量。

该项目重点解决以下问题：
1. 该公司应该使用新页面还是保留旧页面，还是将测试时间延长？
2. 通过拟合回归模型，用户收到不同页面是否存在显著的转化差异？
3. 是否有影响用户发生转化的其他因素？

该项目数据文件共有两个，项目第一部分使用文件为ab-data.csv
该文件共有以下五列：
* user_id 用户id
* timestamp 时间戳
* group 分组，表中control为控制组，treatment为对照组
* landing_page 着陆页，指访问者浏览时到达的第一个页面
* converted 是否已转化

项目第二部分使用文件为countries.csv
该文件共有以下两列：
* user_id 用户id
* country 用户所在国家



