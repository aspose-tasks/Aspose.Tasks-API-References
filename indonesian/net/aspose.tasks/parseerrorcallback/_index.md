---
title: "Delegasi ParseErrorCallback"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Mewakili callback metode untuk menangani kesalahan parsing yang dapat terjadi saat membaca data xml"
type: docs
weight: 1250
url: /id/net/aspose.tasks/parseerrorcallback/
---
## ParseErrorCallback delegate

Mewakili callback metode untuk menangani kesalahan parsing yang dapat terjadi saat membaca data xml.

```csharp
public delegate object ParseErrorCallback(object sender, ParseErrorArgs args);
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| pengirim | Objek | objek sumber dari kesalahan parsing. |
| args | ParseErrorArgs | instansi dari kelas [`ParseErrorArgs`](../parseerrorargs/) yang berisi data acara. |

### Nilai Kembali

nilai yang dipaksa untuk disetel ke objek pengirim yang ditentukan.

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

* class [ParseErrorArgs](../parseerrorargs/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


