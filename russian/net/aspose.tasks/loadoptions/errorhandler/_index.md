---
title: "LoadOptions.ErrorHandler"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "LoadOptions свойство. Получает или задает метод обратного вызова для обработки ошибок разбора xml"
type: docs
weight: 40
url: /ru/net/aspose.tasks/loadoptions/errorhandler/
---
## LoadOptions.ErrorHandler property

Получает или задает метод обратного вызова для обработки ошибок разбора XML.

```csharp
public ParseErrorCallback ErrorHandler { get; set; }
```

## Примеры

Показывает, как прочитать проект из XML‑файла Primavera с ошибкой разбора.

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

// Возвращает проект со специальным UID
var project = new Project(OutDir + "IgnoreInvalidCharacters_out.xml", loadOptions);
Console.WriteLine(project.Get(Prj.Name));
```

Показывает, как загрузить проект Primavera, используя &lt;see cref="LoadOptions" /&gt; с обработкой ошибок.

```csharp
public void WorkWithLoadOptionsAndPrimaveraOptionsAndErrorHandler()
{
    var loadOptions = new LoadOptions();

    var primaveraOptions = new PrimaveraReadOptions
    {
        ProjectUid = 3882
    };

    // установить параметры чтения primavera
    loadOptions.PrimaveraReadOptions = primaveraOptions;
    loadOptions.ErrorHandler = CustomDurationHandlerForFile;

    var project = new Project(DataDir + "PrimaveraProject.xml", loadOptions);

    // работать с проектом...
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

### См. также

* delegate [ParseErrorCallback](../../parseerrorcallback/)
* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


