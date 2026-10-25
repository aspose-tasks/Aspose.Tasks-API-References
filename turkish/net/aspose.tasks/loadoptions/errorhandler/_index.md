---
title: "LoadOptions.ErrorHandler"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "LoadOptions özelliği. XML ayrıştırma hatalarını işlemek için bir geri çağırma yöntemi alır veya ayarlar"
type: docs
weight: 40
url: /tr/net/aspose.tasks/loadoptions/errorhandler/
---
## LoadOptions.ErrorHandler property

XML ayrıştırma hatalarını ele almak için bir geri arama yöntemi alır veya ayarlar.

```csharp
public ParseErrorCallback ErrorHandler { get; set; }
```

## Örnekler

Hata ayrıştırmasıyla bir Primavera XML dosyasından proje nasıl okunacağını gösterir.

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

// Özel UID'ye sahip projeyi döndürür
var project = new Project(OutDir + "IgnoreInvalidCharacters_out.xml", loadOptions);
Console.WriteLine(project.Get(Prj.Name));
```

Hata işleme ile &lt;see cref="LoadOptions" /&gt; kullanarak Primavera projesinin nasıl yükleneceğini gösterir.

```csharp
public void WorkWithLoadOptionsAndPrimaveraOptionsAndErrorHandler()
{
    var loadOptions = new LoadOptions();

    var primaveraOptions = new PrimaveraReadOptions
    {
        ProjectUid = 3882
    };

    // primavera okuma seçeneklerini ayarla
    loadOptions.PrimaveraReadOptions = primaveraOptions;
    loadOptions.ErrorHandler = CustomDurationHandlerForFile;

    var project = new Project(DataDir + "PrimaveraProject.xml", loadOptions);

    // projeyle çalış...
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

### Ayrıca Bakınız

* delegate [ParseErrorCallback](../../parseerrorcallback/)
* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


