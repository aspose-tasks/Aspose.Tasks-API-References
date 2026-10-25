---
title: "Sınıf OleObject"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.OleObject sınıfı. Gantt Şeması Görünümü'ne bir MPP dosyasında eklenebilen bir OLE nesnesini temsil eder."
type: docs
weight: 1120
url: /tr/net/aspose.tasks/oleobject/
---
## OleObject class

Bir MPP dosyasının Gantt Chart View'ına eklenebilen bir OLE nesnesini temsil eder.

```csharp
public class OleObject
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [OleObject](oleobject/)() | `OleObject` sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [ApplicationName](../../aspose.tasks/oleobject/applicationname/) { get; set; } | Gömülü nesneyi açmak için kullanılacak uygulama adını alır veya ayarlar. |
| [Content](../../aspose.tasks/oleobject/content/) { get; set; } | Gömülü dosyanın verilerini alır veya ayarlar; veri gömülmemişse null döner. |
| [DisplayAsIcon](../../aspose.tasks/oleobject/displayasicon/) { get; set; } | OLE nesnesinin bir simge olarak mı yoksa normal resmi olarak mı gösterileceğini belirten bayrağı alır veya ayarlar. |
| [FileFormat](../../aspose.tasks/oleobject/fileformat/) { get; set; } | Gömülü nesnenin dosya formatını alır veya ayarlar. |
| [FullPath](../../aspose.tasks/oleobject/fullpath/) { get; set; } | Eklelen nesnenin tam yolunu alır veya ayarlar. |
| [Id](../../aspose.tasks/oleobject/id/) { get; set; } | Nesne kimliğini alır veya ayarlar. |
| [Label](../../aspose.tasks/oleobject/label/) { get; set; } | Eklelen nesnenin etiketini alır veya ayarlar. |
| [Linked](../../aspose.tasks/oleobject/linked/) { get; } | Proje dosyasının yalnızca bağlantı kaynağında depolanan gerçek veriye bir bağlantı içerip içermediğini gösteren bir değeri alır. |
| [Name](../../aspose.tasks/oleobject/name/) { get; set; } | OLE nesnesinin örneğinin adını alır veya ayarlar. |
| [TemporaryFile](../../aspose.tasks/oleobject/temporaryfile/) { get; set; } | Eklelen nesnenin geçici dosyasının yolunu alır veya ayarlar. |
| [View](../../aspose.tasks/oleobject/view/) { get; set; } | Eklelen nesnenin ait olduğu [`View`](./view/) sınıfının örneğini alır veya ayarlar. |

## Örnekler

OLE nesneleri hakkında bilgi okumanın nasıl yapılacağını gösterir.

```csharp
[Test]
public void WorkWithOleObject()
{
    var images = new Project(DataDir + "TaskImage2010.mpp");
    List<OleObject> oleObjects = images.OleObjects.ToList();

    Console.WriteLine("Ole Objects Count: " + oleObjects.Count);
    foreach (var oleObject in oleObjects)
    {
        Console.WriteLine(" Id: " + oleObject.Id);
        Console.WriteLine(" Name: " + oleObject.Name);
        Console.WriteLine(" DisplayAsIcon: " + oleObject.DisplayAsIcon);
        Console.WriteLine(" Application Name: " + oleObject.ApplicationName);
        Console.WriteLine(" File Format: " + oleObject.FileFormat);
        Console.WriteLine(" Label: " + oleObject.Label);
        Console.WriteLine(" Full Path: " + oleObject.FullPath);
        Console.WriteLine(" Is Linked: " + oleObject.Linked);
        Console.WriteLine(" View Name: " + oleObject.View.Name);
        Console.WriteLine(" Content (first 10 bytes): " + this.Get10Bytes(oleObject));
    }
}

private string Get10Bytes(OleObject oleObject)
{
    byte[] bytes = oleObject.Content;
    var chunk = new byte[10];
    Array.Copy(bytes, chunk, 10);
    var builder = new StringBuilder();
    foreach (var b in chunk)
    {
        builder.Append(b + ", ");
    }

    builder.Remove(builder.Length - 3, 1);
    return builder.ToString();
}
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


