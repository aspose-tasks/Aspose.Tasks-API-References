---
title: "LoadOptions.ErrorHandler"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية LoadOptions. تحصل أو تعيّن طريقة رد نداء للتعامل مع أخطاء تحليل xml"
type: docs
weight: 40
url: /ar/net/aspose.tasks/loadoptions/errorhandler/
---
## LoadOptions.ErrorHandler property

يحصل أو يعيّن طريقة رد نداء للتعامل مع أخطاء تحليل XML.

```csharp
public ParseErrorCallback ErrorHandler { get; set; }
```

## الأمثلة

يظهر كيفية قراءة مشروع من ملف Primavera XML مع خطأ في التحليل.

```csharp
var options = new PrimaveraReadOptions
{
    ProjectUid = 4557
};

var loadOptions = new LoadOptions()
{
    PrimaveraReadOptions = options,
    ErrorHandler = CustomDurationHandlerForFile
};

// يعيد مشروعًا بمعرف UID خاص.
var project = new Project(OutDir + "IgnoreInvalidCharacters_out.xml", loadOptions);
Console.WriteLine(project.Get(Prj.Name));
```

يوضح كيفية تحميل مشروع Primavera باستخدام &lt;see cref="LoadOptions" /&gt; مع معالجة الأخطاء.

```csharp
public void WorkWithLoadOptionsAndPrimaveraOptionsAndErrorHandler()
{
    var loadOptions = new LoadOptions();

    var primaveraOptions = new PrimaveraReadOptions
    {
        ProjectUid = 3882
    };

    // تعيين خيارات قراءة primavera
    loadOptions.PrimaveraReadOptions = primaveraOptions;
    loadOptions.ErrorHandler = CustomDurationHandlerForFile;

    var project = new Project(DataDir + "PrimaveraProject.xml", loadOptions);

    // العمل مع المشروع...
}

private static object CustomDurationHandlerForFile(object sender, ParseErrorArgs args)
{
    var regex = new Regex("[*]{2}(\\d+)Hrs(\\d+)Mins(\\d+)Secs[*]{2}");
    if (args.FieldType != typeof(TimeSpan))
    {
        throw args.Exception;
    }

    Console.WriteLine("Object field: {0}, Object field type: {1}, Invalid value: {2}", args.FieldName, args.FieldType, args.InvalidValue);
    var duration = regex.Replace(args.InvalidValue, "PT$1H$2M$3S");
    var value = Duration.ParseTimeSpan(duration);
    Console.WriteLine("New value : {0}", value);
    return value;
}
```

### انظر أيضًا

* delegate [ParseErrorCallback](../../parseerrorcallback/)
* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


