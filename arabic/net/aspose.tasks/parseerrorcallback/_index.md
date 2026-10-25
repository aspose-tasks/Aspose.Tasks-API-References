---
title: "المندوب ParseErrorCallback"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "يمثل استدعاء طريقة لمعالجة أخطاء التحليل التي يمكن أن تحدث عند قراءة بيانات XML"
type: docs
weight: 1250
url: /ar/net/aspose.tasks/parseerrorcallback/
---
## ParseErrorCallback delegate

يمثل callback طريقة لمعالجة أخطاء التحليل التي قد تحدث عند قراءة بيانات XML.

```csharp
public delegate object ParseErrorCallback(object sender, ParseErrorArgs args);
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| المرسل | كائن | كائن المصدر لخطأ التحليل. |
| args | ParseErrorArgs | مثال من الفئة [`ParseErrorArgs`](../parseerrorargs/) التي تحتوي على بيانات الحدث. |

### قيمة الإرجاع

القيمة المحوَّلة لتعيينها إلى كائن المرسل المحدد.

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

* class [ParseErrorArgs](../parseerrorargs/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


