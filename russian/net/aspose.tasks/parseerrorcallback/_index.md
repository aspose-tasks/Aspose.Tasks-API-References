---
title: "Делегат ParseErrorCallback"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Представляет метод обратного вызова для обработки ошибок разбора, которые могут возникнуть при чтении XML-данных"
type: docs
weight: 1250
url: /ru/net/aspose.tasks/parseerrorcallback/
---
## ParseErrorCallback delegate

Представляет обратный вызов метода для обработки ошибок разбора, которые могут возникнуть при чтении XML-данных.

```csharp
public delegate object ParseErrorCallback(object sender, ParseErrorArgs args);
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| отправитель | Объект | исходный объект ошибки разбора. |
| args | ParseErrorArgs | экземпляр класса [`ParseErrorArgs`](../parseerrorargs/), содержащий данные события. |

### Возвращаемое значение

приведённое значение, которое следует установить в указанный объект‑отправитель.

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

* class [ParseErrorArgs](../parseerrorargs/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


