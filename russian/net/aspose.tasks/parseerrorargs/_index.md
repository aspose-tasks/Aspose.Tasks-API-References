---
title: "Класс ParseErrorArgs"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.ParseErrorArgs. Предоставляет данные для делегата ParseErrorCallback."
type: docs
weight: 1240
url: /ru/net/aspose.tasks/parseerrorargs/
---
## ParseErrorArgs class

Предоставляет данные для делегата [`ParseErrorCallback`](../parseerrorcallback/).

```csharp
public class ParseErrorArgs
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Exception](../../aspose.tasks/parseerrorargs/exception/) { get; } | Возвращает возникшее исключение при разборе строкового значения. |
| [FieldName](../../aspose.tasks/parseerrorargs/fieldname/) { get; } | Возвращает имя поля объекта. |
| [FieldType](../../aspose.tasks/parseerrorargs/fieldtype/) { get; } | Возвращает тип поля объекта. |
| [InvalidValue](../../aspose.tasks/parseerrorargs/invalidvalue/) { get; } | Возвращает строковое значение, которое вызвало исключение. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


