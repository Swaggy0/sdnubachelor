### 山东师大-本科毕业论文-LaTeX模板说明

------

#### 编译环境说明####

- 编译系统发行版：TeX Live（2017或更高）
- LaTeX编译器：XeLaTeX
- 建议编辑器：TeXstudio

#### 开发说明####

本模板基于 CTeX 的 ctexart 标准文档类开发。请确保 CTeX 安装完整，并包含有 ctexart 文档类；二者已包含在 Tex Live 发行版中，建议安装 Tex Live 的离线完整版。模板参照山东师范大学教务处公布的本科生毕业论文示例模板（2018版）开发。

#### 使用说明####

##### 源文件及目录说明

相关 *.tex 源文件说明如下表：

| 源文件           | 编辑说明                                                     |
| ---------------- | ------------------------------------------------------------ |
| sdnubachelor.tex | 主组织文件，用于填写相关信息字段与组织编译。**使用者需关注并进行字段填写。** |
| abstract.tex     | 摘要源文件，从sdnubachelor.tex中获取字段。使用者无需关注此源文件。 |
| appendix.tex     | 附录源文件，组织附录内容。**使用者需关注并在此编辑附录内容。** |
| article.tex      | 正文内容源文件，组织正文内容。**使用者需关注并在此编辑正文内容。** |
| bibliography.tex | 参考文件源文件，组织参考文献内容。**使用者需关注并在此编辑参考文件内容。** |
| cover.tex        | 封面源文件，从sdnubachelor.tex中获取字段。使用者无需关注此源文件。 |
| covertable.tex   | 封2表格源文件，从sdnubachelor.tex中获取字段。使用者无需关注此源文件。 |
| endtable1.tex    | 指导教师意见源文件，从sdnubachelor.tex中获取字段。使用者无需关注此源文件。 |
| endtable2.tex    | 评阅人意见源文件，从sdnubachelor.tex中获取字段。使用者无需关注此源文件。 |
| endtable3.tex    | 答辩学分委员会意见，从sdnubachelor.tex中获取字段。使用者无需关注此源文件。 |
| endtable4.tex    | 论文摘要表格源文件，从sdnubachelor.tex中获取字段。使用者无需关注此源文件。 |

##### 目录说明

- 本文件所在目录为模版主目录，包含 sdnubachelor.cls 格式文件与 sdnubachelor.tex 源文件以及编译生成的 PDF 文件。
- ./data/img/ 目录为正文图片存储目录。
- ./data/resource/ 目录为资源目录，上表中除 sdnubachelor.tex 外其余 *.tex 文件均在此目录中，需要使用者关注编辑的 *.tex 文件需在此打开。
- 编译过程中会生成相关过程文件与输出文件，可酌情删除；模板建议二次编译。

#####sdnubachelor.tex 中的字段说明

| 字段示例                                                    | 说明                                                         |
| ----------------------------------------------------------- | ------------------------------------------------------------ |
| \sdnutitle{人机博弈机制分析与算法研究}{English Title}       | 题目信息，花括号内依次键入中文标题与英文标题。               |
| \sdnuauthor{光头强}{201411010300}                           | 作者信息，花括号内依次键入作者姓名与学号。                   |
| \sdnumentor{熊大}                                           | 导师信息，花括号内键入导师姓名。                             |
| \sdnuinfo{信息科学与工程学院}{计算机科学与技术}{计信本1401} | 班级信息，花括号内依次键入学院名称、专业名称、行政班级。     |
| \sdnudate{2018}{2}{15}                                      | 封面时间，花括号内依次键入年、月、日。                       |
| \sdnukeyw{关键字1}{keyword1}                                | 关键词，花括号内依次中英文关键词。                           |
| \sdnuwdnum{66666}                                           | 论文字数，花括号内键入论文字数。                             |
| \sdnupaperinfo{2017.10.25}{2018.02.25}                      | 封2表格表头时间，花括号内依次键入选题时间与完成时间。        |
| \sdnutabledate{\qquad}{\qquad}{\qquad}                      | 封2表格表尾时间，花括号内依次键入年、月、日。                |
| \sdnupaperov{封2表格主内容1}{封2表格主内容1}                | 封2表格主内容，使用方式详见模板内说明。                      |
| \abstract{中文摘要}{english abstract}                       | 中英文摘要，花括号内依次键入中英文摘要。                     |
| \guidance{指导教师意见}{优}{2018}{3}{11}                    | 指导教师意见表内容，花括号内依次键入指导意见、成绩、年、月、日。 |
| \reviewerp{评阅人意见}{优}{2018}{3}{11}                     | 评阅人意见表内容，花括号内依次键入评阅意见、成绩、年、月、日。 |
| \reply{答辩意见}{优}{2018}{3}{11}                           | 答辩意见表内容，花括号内依次键入答辩意见、成绩、年、月、日   |
| \xuefen{优}{2018}{3}{11}                                    | 学院学位分委员会意见，花括号内依次键入学院学位分委员会成绩、年、月、日。 |
| \resdnuinfo{信工学院}{计算机科学与技术}{计信本1401}         | 论文摘要表格的班级信息重述，主要用于调整该表格美观程度，可适当使用学院简称等。 |
| \cabst{内容摘要}{优}{2018}{3}{11}                           | 论文摘要表格主内容，以及表尾成绩与时间等相关信息。           |

##### 使用步骤简述

1. 填写 sdnubachelor.tex  中相关字段的内容。
2. 在 ./data/resource/article.tex 中撰写您的正文。
3. 在 ./data/resource/bibliography.tex 中撰写您的参考文件，并可在正文中引用。
4. 在 ./data/resource/appendix.tex 中撰写您的附录。

注：上述步骤请灵活调整；可参考模板中已存在的部分内容与说明进行合理使用。

P(tu)S(cao)：教务处的新通知版本简直是无语，更改了边距，结果给的封面范例还是原来的边距(其实那个边距就是Word的默认边距而已)，难道一个文档要用不同的边距？！还是封面要与文档分离？！学校所谓的格式要求都是针对Word的，本模板致力于与Word版本保持一致，但word与Tex始终不一样，就像差等生与优等生也始终不一样。

PPS：伟大的圣人兰彻欧德斯曾经说过，学习是为了完善人生，追求卓越，成功就会出其不意的找上门来。

