---
title: "Project.Project"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Project yapıcı. Project sınıfının yeni bir örneğini başlatır."
type: docs
weight: 10
url: /tr/net/aspose.tasks/project/project/
---
## Project() {#constructor}

[`Project`](../) sınıfının yeni bir örneğini başlatır.

```csharp
public Project()
```

## Örnekler

Bir proje oluşturmanın ve MPP şablon dosyası geçirmeden MPP formatında kaydetmenin nasıl yapılacağını gösterir.

```csharp
var project = new Project();

// Proje, dahili MPP şablonu kullanılarak MPP olarak kaydedilecektir.
project.Save(OutDir + "CreateEmptyProjectSaveMPP_out.mpp", SaveFileFormat.Mpp);
```

### Ayrıca Bakınız

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string, string) {#constructor_12}

Şifre korumalı bir şablondan (mevcut mpp veya mpt dosyası) [`Project`](../) sınıfının yeni bir örneğini başlatır.

```csharp
public Project(string projectTemplate, string protectionPassword)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| projectTemplate | Dize | Projeyi oluşturmak için şablonun yolu. |
| protectionPassword | Dize | Koruma şifresi. |

## Açıklamalar

Şifre korumalı dosyaların okunması şu anda yalnızca MSP 2003 dosya formatı için desteklenmektedir.

## Örnekler

Şifre korumalı MPP dosyalarını okumanın nasıl yapılacağını gösterir.

```csharp
var project = new Project(DataDir + "PasswordProtectedProject.mpp", "password");
Console.WriteLine(project.Get(Prj.Name));
```

### Ayrıca Bakınız

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string) {#constructor_8}

Şablondan (mevcut mpp veya mpt dosyası) [`Project`](../) sınıfının yeni bir örneğini başlatır.

```csharp
public Project(string projectTemplate)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| projectTemplate | Dize | Projeyi oluşturmak için şablonun yolu. |

## Örnekler

Bir MPP dosyasını okumanın nasıl yapılacağını gösterir.

```csharp
var project = new Project(DataDir + "ReadProjectFiles.mpp");
project.Save(OutDir + "ReadProjectFiles_out.mpp", SaveFileFormat.Xml);
```

### Ayrıca Bakınız

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream, PrimaveraReadOptions) {#constructor_5}

Belirtilen [`PrimaveraReadOptions`](../../primaverareadoptions/) sınıfı örneğiyle Stream'den [`Project`](../) sınıfının yeni bir örneğini başlatır.

```csharp
public Project(Stream stream, PrimaveraReadOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | Akış | Project Streamclass'ın Akışı |
| options | PrimaveraReadOptions | belirtilen [`PrimaveraReadOptions`](../../primaverareadoptions/) sınıfı örneği, Primavera formatlarını (XER veya XML) okuma özelleştirmesine izin verir. |

## Örnekler

Bir akıştan, birden çok proje içeren Primavera XML veya Primavera XER dosyasıyla bir proje nasıl okunacağını gösterir.

```csharp
var options = new PrimaveraReadOptions
{
    ProjectUid = 4557
};
using (var stream = new FileStream(DataDir + "Project.xml", FileMode.Open, FileAccess.Read))
{
    // Özel UID'ye sahip projeyi döndürür
    var project = new Project(stream, options);
    Console.WriteLine(project.Get(Prj.Name));
}
```

### Ayrıca Bakınız

* class [PrimaveraReadOptions](../../primaverareadoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string, ParseErrorCallback) {#constructor_10}

Şablondan (mevcut mpp veya mpt dosyası) [`Project`](../) sınıfının yeni bir örneğini başlatır.

```csharp
public Project(string projectTemplate, ParseErrorCallback parseErrorHandler)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| projectTemplate | Dize | Projeyi oluşturmak için şablonun yolu. |
| parseErrorHandler | ParseErrorCallback | xml ayrıştırma hatalarını işlemek için belirtilen geri çağırma yöntemi. |

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

* delegate [ParseErrorCallback](../../parseerrorcallback/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream) {#constructor_2}

Bir akıştan yeni bir [`Project`](../) sınıfı örneği başlatır.

```csharp
public Project(Stream stream)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | Akış | Şablonun yükleneceği akış. |

## Örnekler

Bir akıştan XML proje dosyasının nasıl okunacağını gösterir.

```csharp
using (Stream stream = new FileStream(DataDir + "Project.xml", FileMode.Open))
{
    var project = new Project(stream);
    project.Save(OutDir + "ReadProjectFileFromStream_out.xml", SaveFileFormat.Xml);
}
```

### Ayrıca Bakınız

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(StreamReader) {#constructor_7}

Bir StreamReader örneğinden yeni bir [`Project`](../) sınıfı örneği başlatır.

```csharp
public Project(StreamReader reader)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| reader | StreamReader | Şablonun yükleneceği akış okuyucu. |

## Örnekler

Belirli kodlamayla MPX dosyalarının nasıl okunacağını gösterir.

```csharp
using (var streamReader = new StreamReader(DataDir + "EUC-KR-encoding.mpx", System.Text.Encoding.GetEncoding("ISO-8859-1")))
{
    var project = new Project(streamReader);
    Console.WriteLine(project.RootTask.Children.ToList()[0].Get(Tsk.Name));
    project.Save(OutDir + "WorkingWithEncodings_out.mpx", SaveFileFormat.Mpx);
}
```

### Ayrıca Bakınız

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string, PrimaveraReadOptions) {#constructor_11}

Mevcut bir MPP veya MPT dosyası (şablon) ve belirtilen [`PrimaveraReadOptions`](../../primaverareadoptions/) sınıfı örneği ile yeni bir [`Project`](../) sınıfı örneği başlatır.

```csharp
public Project(string projectTemplate, PrimaveraReadOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| projectTemplate | Dize | Projeyi oluşturmak için şablon yolu |
| options | PrimaveraReadOptions | belirtilen [`PrimaveraReadOptions`](../../primaverareadoptions/) sınıfı örneği. |

## Örnekler

Primavera okuma seçeneklerini kullanarak birden çok proje içeren Primavera XML veya Primavera XER dosyasından bir projenin nasıl okunacağını gösterir.

```csharp
var options = new PrimaveraReadOptions()
{
    ProjectUid = 4557
};

// Özel UID'ye sahip projeyi döndürür
var project = new Project(DataDir + "Project.xml", options);
Console.WriteLine(project.Get(Prj.Name));
```

### Ayrıca Bakınız

* class [PrimaveraReadOptions](../../primaverareadoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(DbSettings) {#constructor_1}

[`DbSettings`](../../../aspose.tasks.connectivity/dbsettings/) sınıfı örneğiyle belirtilen bir veritabanından veri okumak için yeni bir [`Project`](../) sınıfı örneği başlatır.

```csharp
public Project(DbSettings settings)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| settings | DbSettings | belirtilen [`DbSettings`](../../../aspose.tasks.connectivity/dbsettings/) sınıfı örneği. |

## Örnekler

Veritabanı ayarlarını kullanarak bir Primavera veritabanından proje nasıl içe aktarılacağını gösterir.

```csharp
var sb = new SqlConnectionStringBuilder
{
    DataSource = "192.168.56.3,1433",
    Encrypt = true,
    TrustServerCertificate = true,
    InitialCatalog = "PrimaveraEDB",
    NetworkLibrary = "DBMSSOCN",
    UserID = "privuser",
    Password = "***",
};

// Bağlantı dizesi ve proje kimliği ile PrimaveraDbSettings sınıfının yeni bir örneğini başlat
var settings = new PrimaveraDbSettings(sb.ConnectionString, 4502);

// Project sınıfının yeni bir örneğini başlat
var project = new Project(settings);
Console.WriteLine(project.Get(Prj.Name));
```

### Ayrıca Bakınız

* class [DbSettings](../../../aspose.tasks.connectivity/dbsettings/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream, ParseErrorCallback) {#constructor_4}

Şablondan (mevcut MPP veya MPT dosyası) yeni bir [`Project`](../) sınıfı örneği başlatır.

```csharp
public Project(Stream stream, ParseErrorCallback parseErrorHandler)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | Akış | Şablonun yükleneceği akış. |
| parseErrorHandler | ParseErrorCallback | xml ayrıştırma hatalarını işlemek için belirtilen geri çağırma yöntemi. |

## Örnekler

Geçersiz karakterler içeren bir XML dosyasından proje nasıl okunacağını gösterir.

```csharp
public static void LoadProjectFromStream(string brokenXmlData)
{
    // Bozuk zaman aralıkları içeren XML'i içeren akışı açın
    byte[] bytes = Encoding.UTF8.GetBytes(brokenXmlData);
    using (var stream = new MemoryStream(bytes))
    {
        var project = new Project(stream, CustomDurationHandlerForStream2);
        Console.WriteLine(project.Get(Prj.Name));
    }
}

public static object CustomDurationHandlerForStream2(object sender, ParseErrorArgs args)
{
    var regex = new Regex("[*]{2}(\\d+)Hrs(\\d+)Mins(\\d+)Secs[*]{2}");
    if (args.FieldType != typeof(TimeSpan))
    {
        throw args.Exception;
    }

    Debug.Print("Object field : {0}, Invalid value : {1}", args.FieldName, args.InvalidValue);
    var duration = regex.Replace(args.InvalidValue, "PT$1H$2M$3S");
    var newValue = Duration.ParseTimeSpan(duration);
    Debug.Print("New value : {0}", newValue);
    return newValue;
}
```

### Ayrıca Bakınız

* delegate [ParseErrorCallback](../../parseerrorcallback/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream, string) {#constructor_6}

Şablondan (mevcut MPP veya MPT dosyası) yeni bir [`Project`](../) sınıfı örneği başlatır.

```csharp
public Project(Stream stream, string protectionPassword)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | Akış | Şablonun yükleneceği akış. |
| protectionPassword | Dize | Koruma şifresi. |

## Açıklamalar

Şifre korumalı dosyaların okunması şu anda yalnızca MSP 2003 dosya formatı için desteklenmektedir.

## Örnekler

MPP'nin şifre korumalı olup olmadığını nasıl kontrol edeceğinizi gösterir.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "PasswordProtected.mpp");
Console.WriteLine("Is file password protected?:" + info.IsPasswordProtected);
```

Şifre korumalı MPP dosyalarını bir akıştan nasıl okuyacağınızı gösterir.

```csharp
using (var stream = new FileStream(DataDir + "PasswordProtectedProject.mpp", FileMode.Open))
{
    var project = new Project(stream, "password");
    Console.WriteLine(project.Get(Prj.Name));
}
```

### Ayrıca Bakınız

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(string, LoadOptions) {#constructor_9}

Belirtilen [`LoadOptions`](../../loadoptions/) sınıfının örneğiyle bir şablondan (mevcut mpp veya mpt dosyası) yeni bir [`Project`](../) sınıfı örneği başlatır.

```csharp
public Project(string projectTemplate, LoadOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| projectTemplate | Dize | Projeyi oluşturmak için şablon yolu |
| options | LoadOptions | Belirtilen [`LoadOptions`](../../loadoptions/) sınıfının örneği. |

## Örnekler

Bir dosyadan projeyi &lt;see cref=\"Aspose.Tasks.LoadOptions\"/&gt; örneği kullanarak nasıl yükleyeceğinizi gösterir.

```csharp
var options = new LoadOptions
{
    Password = "password"
};
var project = new Project(DataDir + "PasswordProtectedProject.mpp", options);
Console.WriteLine(project.Get(Prj.Name));
```

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

### Ayrıca Bakınız

* class [LoadOptions](../../loadoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Project(Stream, LoadOptions) {#constructor_3}

Belirtilen [`LoadOptions`](../../loadoptions/) sınıfının örneğiyle Akıştan yeni bir [`Project`](../) sınıfı örneği başlatır.

```csharp
public Project(Stream stream, LoadOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | Akış | Project Streamclass'ın Akışı |
| options | LoadOptions | Belirtilen [`LoadOptions`](../../loadoptions/) sınıfının örneği. |

## Örnekler

Bir akıştan projeyi &lt;see cref=\"Aspose.Tasks.LoadOptions\"/&gt; örneği kullanarak nasıl yükleyeceğinizi gösterir.

```csharp
using (var stream = new FileStream(DataDir + "PasswordProtectedProject.mpp", FileMode.Open))
{
    var options = new LoadOptions
    {
        Password = "password"
    };
    var project = new Project(stream, options);
    Console.WriteLine(project.Get(Prj.Name));
}
```

### Ayrıca Bakınız

* class [LoadOptions](../../loadoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


