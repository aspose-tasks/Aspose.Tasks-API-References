---
title: "Sınıf ParseErrorArgs"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.ParseErrorArgs sınıfı. ParseErrorCallback temsilcisi için veri sağlar"
type: docs
weight: 1240
url: /tr/net/aspose.tasks/parseerrorargs/
---
## ParseErrorArgs class

[`ParseErrorCallback`](../parseerrorcallback/) temsilcisi için veri sağlar.

```csharp
public class ParseErrorArgs
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Exception](../../aspose.tasks/parseerrorargs/exception/) { get; } | Dize değerini ayrıştırma sırasında ortaya çıkan istisna alınır. |
| [FieldName](../../aspose.tasks/parseerrorargs/fieldname/) { get; } | Nesne alanının adını alır. |
| [FieldType](../../aspose.tasks/parseerrorargs/fieldtype/) { get; } | Nesne alanının tipini alır. |
| [InvalidValue](../../aspose.tasks/parseerrorargs/invalidvalue/) { get; } | İstisna oluşturan dize değerini alır. |

## Örnekler

Geçersiz karakterler içeren XML dosyasıyla bir akıştan proje nasıl okunacağını gösterir.

```csharp
public static void LoadProjectFromFile(string pathToModifiedXml)
{
    // Bozuk zaman aralıkları içeren XML içeren dosyayı açın
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

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


