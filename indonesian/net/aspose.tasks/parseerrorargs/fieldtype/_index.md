---
title: "ParseErrorArgs.FieldType"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "ParseErrorArgs properti. Mendapatkan tipe bidang objek"
type: docs
weight: 30
url: /id/net/aspose.tasks/parseerrorargs/fieldtype/
---
## ParseErrorArgs.FieldType property

Mendapatkan tipe bidang objek.

```csharp
public Type FieldType { get; }
```

## Contoh

Menampilkan cara membaca proyek dari aliran dengan file XML yang berisi karakter tidak valid.

```csharp
public static void LoadProjectFromFile(string pathToModifiedXml)
{
    // buka file yang berisi XML dengan rentang waktu yang rusak
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

### Lihat Juga

* class [ParseErrorArgs](../)
* namespace [Aspose.Tasks](../../parseerrorargs/)
* assembly [Aspose.Tasks](../../../)


