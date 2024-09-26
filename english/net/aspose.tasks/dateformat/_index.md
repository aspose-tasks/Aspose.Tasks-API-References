---
title: Enum DateFormat
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.DateFormat enum. Specifies the date format
type: docs
weight: 430
url: /net/aspose.tasks/dateformat/
---
## DateFormat enumeration

Specifies the date format.

```csharp
public enum DateFormat
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| DateMmDdYyHhMmAM | `0` | The example: 09/30/02 13:00 PM |
| DateMmDdYy | `1` | The example: 9/30/02 |
| DateMmmmDdYyyyHhMmAM | `2` | The example: September 30, 2002 13:00 PM |
| DateMmmmDdYyyy | `3` | The example: September 30, 2002 |
| DateMmmDdHhMmAM | `4` | The example: Sep 30 13:00 PM |
| DateMmmDdYyy | `5` | The example: Sep 30, '02 |
| DateMmmmDd | `6` | The example: September 30 |
| DateMmmDd | `7` | The example: Sep 30 |
| DateDddMmDdYyHhMmAM | `8` | The example: Tue 9/30/02 13:00 PM |
| DateDddMmDdYy | `9` | The example: Tue 9/30/02 |
| DateDddMmmDdYyy | `10` | The example: Tue Sep 30, '02 |
| DateDddHhMmAM | `11` | The example: Tue 13:00 PM |
| DateMmDd | `12` | The example: 9/30 |
| DateDd | `13` | The example: 30 |
| DateHhMmAm | `14` | The example: 13:00 PM |
| DateDddMmmDd | `15` | The example: Tue Sep 30 |
| DateDddMmDd | `16` | The example: Tue 9/30 |
| DateDddDd | `17` | The example: Tue 30 |
| DateWwwDd | `18` | The example: W41/2 |
| DateWwwDdYyHhMmAm | `19` | The example: W41/2/02 13:00 PM |
| DateMmDdYyyy | `20` | The example: 9/30/2002 |
| Custom | `21` | DateTime values are formatted using format string which is set to the project's [`CustomDateFormat`](../prj/customdateformat/) property. |
| DateDdMmYyyy | `256` | The example: 19/07/2016 |
| Default | `255` | The example: Default date format. |

## Examples

Shows how to customize date format of all dates in the project to be exported.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
project.Set(Prj.StartDate, new DateTime(2014, 9, 22));

// By default project.DateFormat == DateFormat.Date_ddd_mm_dd_yy (Mon 09/22/14) customize DateFormat (September 22, 2014)
project.Set(Prj.DateFormat, DateFormat.DateMmmmDdYyyy);
project.Save(OutDir + "CustomizeDateFormats1_out.pdf", SaveFileFormat.Pdf);

// Export to date format 19/07/2016
project.Set(Prj.DateFormat, DateFormat.DateDdMmYyyy);
project.Save(OutDir + "CustomizeDateFormats2_out.pdf", SaveFileFormat.Pdf);
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


