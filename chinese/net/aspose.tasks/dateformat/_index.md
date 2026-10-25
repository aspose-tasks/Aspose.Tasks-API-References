---
title: "枚举 DateFormat"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.DateFormat 枚举。指定日期格式"
type: docs
weight: 430
url: /zh/net/aspose.tasks/dateformat/
---
## DateFormat enumeration

指定日期格式。

```csharp
public enum DateFormat
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| DateMmDdYyHhMmAM | `0` | 示例：09/30/02 13:00 PM |
| DateMmDdYy | `1` | 示例：9/30/02 |
| DateMmmmDdYyyyHhMmAM | `2` | 示例：September 30, 2002 13:00 PM |
| DateMmmmDdYyyy | `3` | 示例：September 30, 2002 |
| DateMmmDdHhMmAM | `4` | 示例：Sep 30 13:00 PM |
| DateMmmDdYyy | `5` | 示例：Sep 30, '02 |
| DateMmmmDd | `6` | 示例：September 30 |
| DateMmmDd | `7` | 示例：Sep 30 |
| DateDddMmDdYyHhMmAM | `8` | 示例：Tue 9/30/02 13:00 PM |
| DateDddMmDdYy | `9` | 示例：Tue 9/30/02 |
| DateDddMmmDdYyy | `10` | 示例：Tue Sep 30, '02 |
| DateDddHhMmAM | `11` | 示例：Tue 13:00 PM |
| DateMmDd | `12` | 示例：9/30 |
| DateDd | `13` | 示例：30 |
| DateHhMmAm | `14` | 示例：13:00 PM |
| DateDddMmmDd | `15` | 示例：Tue Sep 30 |
| DateDddMmDd | `16` | 示例：Tue 9/30 |
| DateDddDd | `17` | 示例：Tue 30 |
| DateWwwDd | `18` | 示例：W41/2 |
| DateWwwDdYyHhMmAm | `19` | 示例：W41/2/02 13:00 PM |
| DateMmDdYyyy | `20` | 示例：9/30/2002 |
| Custom | `21` | DateTime 值使用格式字符串进行格式化，该字符串设置为项目的 [`CustomDateFormat`](../prj/customdateformat/) 属性。 |
| DateDdMmYyyy | `256` | 示例：19/07/2016 |
| Default | `255` | 示例：默认日期格式。 |

## 示例

展示如何自定义项目中所有要导出的日期格式。

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
project.Set(Prj.StartDate, new DateTime(2014, 9, 22));

// 默认情况下 project.DateFormat == DateFormat.Date_ddd_mm_dd_yy (Mon 09/22/14) 自定义 DateFormat (September 22, 2014)
project.Set(Prj.DateFormat, DateFormat.DateMmmmDdYyyy);
project.Save(OutDir + "CustomizeDateFormats1_out.pdf", SaveFileFormat.Pdf);

// 导出为日期格式 19/07/2016
project.Set(Prj.DateFormat, DateFormat.DateDdMmYyyy);
project.Save(OutDir + "CustomizeDateFormats2_out.pdf", SaveFileFormat.Pdf);
```

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


