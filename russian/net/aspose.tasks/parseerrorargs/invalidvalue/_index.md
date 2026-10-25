---
title: "ParseErrorArgs.InvalidValue"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство ParseErrorArgs. Возвращает строковое значение, которое вызвало исключение"
type: docs
weight: 40
url: /ru/net/aspose.tasks/parseerrorargs/invalidvalue/
---
## ParseErrorArgs.InvalidValue property

Возвращает строковое значение, которое вызвало исключение.

```csharp
public string InvalidValue { get; }
```

## Примеры

Показывает, как прочитать проект из потока с XML‑файлом, содержащим недопустимые символы.

```csharp
public static void LoadProjectFromFile(string pathToModifiedXml)
{
    // откройте файл, содержащий XML с повреждёнными временными интервалами
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

### См. также

* class [ParseErrorArgs](../)
* namespace [Aspose.Tasks](../../parseerrorargs/)
* assembly [Aspose.Tasks](../../../)


