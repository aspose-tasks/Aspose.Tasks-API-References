---
title: "الفئة ParseErrorArgs"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "فئة Aspose.Tasks.ParseErrorArgs. توفر بيانات لمندوب ParseErrorCallback."
type: docs
weight: 1240
url: /ar/net/aspose.tasks/parseerrorargs/
---
## ParseErrorArgs class

توفر بيانات للمندوب [`ParseErrorCallback`](../parseerrorcallback/).

```csharp
public class ParseErrorArgs
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Exception](../../aspose.tasks/parseerrorargs/exception/) { get; } | يحصل على الاستثناء الذي تم رفعه أثناء تحليل قيمة السلسلة. |
| [FieldName](../../aspose.tasks/parseerrorargs/fieldname/) { get; } | يحصل على اسم حقل الكائن. |
| [FieldType](../../aspose.tasks/parseerrorargs/fieldtype/) { get; } | يحصل على نوع حقل الكائن. |
| [InvalidValue](../../aspose.tasks/parseerrorargs/invalidvalue/) { get; } | يحصل على قيمة السلسلة التي أثارت استثناءً. |

## الأمثلة

يوضح كيفية قراءة مشروع من تدفق يحتوي على ملف XML بأحرف غير صالحة.

```csharp
public static void LoadProjectFromFile(string pathToModifiedXml)
{
    // افتح الملف الذي يحتوي على XML مع فترات زمنية مكسورة
    var project = new Project(pathToModifiedXml, CustomDurationHandlerForFile2);
    Console.WriteLine(project.Get(Prj.Name));
}

public static object CustomDurationHandlerForFile2(object sender, ParseErrorArgs args)
{
    var regex = new Regex("[*]{2}(\\d+)Hrs(\\d+)Mins(\\d+)Secs[*]{2}");
    if (args.FieldType != typeof(TimeSpan))
    {
        throw args.Exception;
    }

    Console.WriteLine("Object field: {0}, Object field type: {1}, Invalid value: {2}", args.FieldName, args.FieldType, args.InvalidValue);
    var duration = regex.Replace(args.InvalidValue, "PT$1H$2M$3S");
    var newValue = Duration.ParseTimeSpan(duration);
    Console.WriteLine("New value : {0}", newValue);
    return newValue;
}
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


