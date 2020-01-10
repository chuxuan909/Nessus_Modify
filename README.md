# Nessus_modify

Nessus扫描完成，总要花挺多时间去整理报告，为此写了一个小脚本，用于自动化生成中文漏洞报告。

解析html报告，自动翻译成中文，并提供修复建议，减少整理报告的时间，提升工作效率。

#### 使用目录介绍

```txt
Nessus_Modify
 
│ Nessus_report.py           //脚本文件
│ README.md                 
│ vuln.db
```                     //中文漏洞库

#### 使用简介

1、Nessus扫描结束，选择HTML类型，Report选择Custom，Croup By 选择Host，导出HTML报告。

2、运行脚本：Nessus_resport.py test.html

在同目录下，生成CSV文件，包含服务器IP、漏洞名称、风险级别、漏洞描述、修复建议。

#### 中文漏洞库的升级

中文漏洞库：https://github.com/FunnyKun/NessusReportInChinese