---
title: "LoadOptions.ErrorHandler"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti LoadOptions. Mendapatkan atau mengatur metode callback untuk menangani kesalahan parsing xml"
type: docs
weight: 40
url: /id/net/aspose.tasks/loadoptions/errorhandler/
---
## LoadOptions.ErrorHandler property

Mendapatkan atau mengatur metode callback untuk menangani kesalahan parsing xml.

```csharp
public ParseErrorCallback ErrorHandler { get; set; }
```

## Contoh

Menampilkan cara membaca proyek dari file XML Primavera dengan kesalahan parsing.

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

// Mengembalikan proyek dengan UID khusus
var project = new Project(OutDir + "IgnoreInvalidCharacters_out.xml", loadOptions);
Console.WriteLine(project.Get(Prj.Name));
```

Menampilkan cara memuat proyek Primavera menggunakan &lt;see cref="LoadOptions" /&gt; dengan penanganan kesalahan.

```csharp
public void WorkWithLoadOptionsAndPrimaveraOptionsAndErrorHandler()
{
    var loadOptions = new LoadOptions();

    var primaveraOptions = new PrimaveraReadOptions
    {
        ProjectUid = 3882
    };

    // atur opsi pembacaan primavera
    loadOptions.PrimaveraReadOptions = primaveraOptions;
    loadOptions.ErrorHandler = CustomDurationHandlerForFile;

    var project = new Project(DataDir + "PrimaveraProject.xml", loadOptions);

    // bekerja dengan proyek...
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

### Lihat Juga

* delegate [ParseErrorCallback](../../parseerrorcallback/)
* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


