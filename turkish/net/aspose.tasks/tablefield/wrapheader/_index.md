---
title: "TableField.WrapHeader"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "TableField özelliği. Tablo sütunu başlığının birden fazla satıra sarılıp sarılamayacağını veya sütun genişliğini aştığında kesilip kesilmeyeceğini belirten bir değeri alır veya ayarlar"
type: docs
weight: 70
url: /tr/net/aspose.tasks/tablefield/wrapheader/
---
## TableField.WrapHeader property

Tablo sütun başlığının birden çok satıra kaydırılıp kaydırılamayacağını veya sütun genişliğini aştığında kesilip kesilmeyeceğini belirten bir değeri alır veya ayarlar.

```csharp
public bool WrapHeader { get; set; }
```

## Örnekler

Proje tablolarını nasıl okuyacağınızı gösterir.

```csharp
var project = new Project(DataDir + "ReadTableData.mpp");

// tabloyu al
var table = project.Tables.ToList()[0];
Console.WriteLine("Print table fields of {0}", table.Name);
Console.WriteLine("Table Fields Count" + table.TableFields.Count);

// tüm tablo alanlarının bilgilerini göster
foreach (var field in table.TableFields)
{
    Console.WriteLine("  Field: " + field.Field);
    Console.WriteLine("  Width: " + field.Width);
    Console.WriteLine("  Title: " + field.Title);
    Console.WriteLine("  Title Alignment: " + field.AlignTitle);
    Console.WriteLine("  Data Alignment: " + field.AlignData);
    Console.WriteLine("  Wrap Header: " + field.WrapHeader);
    Console.WriteLine("  Wrap Text: " + field.WrapText);
    Console.WriteLine();
}
```

### Ayrıca Bakınız

* class [TableField](../)
* namespace [Aspose.Tasks](../../tablefield/)
* assembly [Aspose.Tasks](../../../)


