---
title: "ParseErrorArgs.InvalidValue"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ParseErrorArgs özelliği. Bir istisna oluşturan dize değerini alır."
type: docs
weight: 40
url: /tr/net/aspose.tasks/parseerrorargs/invalidvalue/
---
## ParseErrorArgs.InvalidValue property

İstisna oluşturan dize değerini alır.

```csharp
public string InvalidValue { get; }
```

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

* class [ParseErrorArgs](../)
* namespace [Aspose.Tasks](../../parseerrorargs/)
* assembly [Aspose.Tasks](../../../)


