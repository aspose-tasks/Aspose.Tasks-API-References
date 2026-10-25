---
title: "تعداد DateFormat"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "تعداد Aspose.Tasks.DateFormat. يحدد تنسيق التاريخ."
type: docs
weight: 430
url: /ar/net/aspose.tasks/dateformat/
---
## DateFormat enumeration

يحدد تنسيق التاريخ.

```csharp
public enum DateFormat
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| DateMmDdYyHhMmAM | `0` | المثال: 09/30/02 13:00 م |
| DateMmDdYy | `1` | المثال: 9/30/02 |
| DateMmmmDdYyyyHhMmAM | `2` | المثال: سبتمبر 30, 2002 13:00 م |
| DateMmmmDdYyyy | `3` | المثال: سبتمبر 30, 2002 |
| DateMmmDdHhMmAM | `4` | المثال: سبتمبر 30 13:00 م |
| DateMmmDdYyy | `5` | المثال: Sep 30, '02 |
| DateMmmmDd | `6` | المثال: September 30 |
| DateMmmDd | `7` | المثال: Sep 30 |
| DateDddMmDdYyHhMmAM | `8` | المثال: Tue 9/30/02 13:00 PM |
| DateDddMmDdYy | `9` | المثال: Tue 9/30/02 |
| DateDddMmmDdYyy | `10` | المثال: Tue Sep 30, '02 |
| DateDddHhMmAM | `11` | المثال: Tue 13:00 PM |
| DateMmDd | `12` | المثال: 9/30 |
| DateDd | `13` | المثال: 30 |
| DateHhMmAm | `14` | المثال: 13:00 PM |
| DateDddMmmDd | `15` | المثال: Tue Sep 30 |
| DateDddMmDd | `16` | المثال: Tue 9/30 |
| DateDddDd | `17` | المثال: Tue 30 |
| DateWwwDd | `18` | المثال: W41/2 |
| DateWwwDdYyHhMmAm | `19` | المثال: W41/2/02 13:00 PM |
| DateMmDdYyyy | `20` | المثال: 9/30/2002 |
| Custom | `21` | يتم تنسيق قيم DateTime باستخدام سلسلة التنسيق التي تم تعيينها إلى خاصية [`CustomDateFormat`](../prj/customdateformat/) للمشروع. |
| DateDdMmYyyy | `256` | المثال: 19/07/2016 |
| Default | `255` | المثال: تنسيق التاريخ الافتراضي. |

## الأمثلة

يعرض كيفية تخصيص تنسيق التاريخ لجميع التواريخ في المشروع لتصديره.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
project.Set(Prj.StartDate, new DateTime(2014, 9, 22));

// بشكل افتراضي project.DateFormat == DateFormat.Date_ddd_mm_dd_yy (Mon 09/22/14) تخصيص DateFormat (September 22, 2014)
project.Set(Prj.DateFormat, DateFormat.DateMmmmDdYyyy);
project.Save(OutDir + "CustomizeDateFormats1_out.pdf", SaveFileFormat.Pdf);

// تصدير إلى تنسيق التاريخ 19/07/2016
project.Set(Prj.DateFormat, DateFormat.DateDdMmYyyy);
project.Save(OutDir + "CustomizeDateFormats2_out.pdf", SaveFileFormat.Pdf);
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


