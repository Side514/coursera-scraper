# coursera-scraper

爬取coursera平台指定课程的基本信息及全部评论的工具。

## 使用方法

clone仓库到本地，python环境运行。

## 特性

### get_reviews.py

输入coursera平台课程URL，返回该课程所有评论。

每条评论的属性：

- rating（评分）
- text（评论文本）
- date（日期）
- completed（是否完成）

输出到文件：`coursera-课程名.json`

### get_course_list.py

输入查询关键字，利用coursera自带的搜索功能，查询数据库接口，返回平台查询到的所有课程信息。

每门课程的属性：

- 链接
- 课程名
- 提供方
- 注册人数
- 评价人数
- 评分
- 难度级别
- 学习计划
- 课程长度
- 平均学习时长
- 技能标签
- 授课语言
- 字幕语言

输出到文件：`list-查询关键字.csv`

## 依赖包

- beautifulsoup4
