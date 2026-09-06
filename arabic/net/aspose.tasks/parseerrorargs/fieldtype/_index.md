---
title: "ParseErrorArgs.FieldType"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية ParseErrorArgs. تحصل على نوع حقل الكائن"
type: docs
weight: 30
url: /ar/net/aspose.tasks/parseerrorargs/fieldtype/
---
## ParseErrorArgs.FieldType property

يحصل على نوع حقل الكائن.

```csharp
public Type FieldType { get; }
```

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

* class [ParseErrorArgs](../)
* namespace [Aspose.Tasks](../../parseerrorargs/)
* assembly [Aspose.Tasks](../../../)


