---
title: "TableField sınıfı"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.TableField sınıfı. Bir projedeki tablonun bir alanını temsil eder"
type: docs
weight: 2340
url: /tr/net/aspose.tasks/tablefield/
---
## TableField class

Bir projedeki tablonun bir alanını temsil eder.

```csharp
public class TableField
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [TableField](tablefield/)() | `TableField` sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [AlignData](../../aspose.tasks/tablefield/aligndata/) { get; set; } | Tablo alanındaki verinin hizalamasını alır veya ayarlar. |
| [AlignTitle](../../aspose.tasks/tablefield/aligntitle/) { get; set; } | Tablo alanındaki başlığın hizalamasını alır veya ayarlar. |
| [Field](../../aspose.tasks/tablefield/field/) { get; set; } | Bir tablo alanının tipini alır veya ayarlar. |
| [Title](../../aspose.tasks/tablefield/title/) { get; set; } | Tablodaki alanın başlığını alır veya ayarlar. |
| [Width](../../aspose.tasks/tablefield/width/) { get; set; } | Tablodaki alan sütununun puan cinsinden genişliğini alır veya ayarlar. |
| [WrapHeader](../../aspose.tasks/tablefield/wrapheader/) { get; set; } | Tablo sütun başlığının birden çok satıra kaydırılıp kaydırılamayacağını veya sütun genişliğini aştığında kesilip kesilmeyeceğini belirten bir değeri alır veya ayarlar. |
| [WrapText](../../aspose.tasks/tablefield/wraptext/) { get; set; } | Sütun metninin birden çok satıra kaydırılıp kaydırılamayacağını veya sütun genişliğini aştığında kesilip kesilmeyeceğini belirten bir değeri alır veya ayarlar. MSP 2010 sürümü ve sonrasında desteklenir. |

## Örnekler

Project'in görünümüyle nasıl çalışılacağını ve varsayılan görünüme (MPP dosyası MS Project'te açıldığında gösterilen) bir sütun eklemeyi gösterir.

```csharp
// görünümler olmadan boş bir proje oluştur
var project = new Project();
project.Set(Prj.Name, "Test View Project");

// Varsayılan görünümü (bu bir Gantt şeması görünümüdür) değiştir.
// Veya proje.View koleksiyonunu kullanarak görünümü isimle ya da Görünüm Ekranı ile seçebilirsiniz.
var view = (GanttChartView) project.DefaultView;

TableField newColumn = new TableField()
{
    AlignData = HorizontalStringAlignment.Center,
    Title = "My new column",
    Width = 30,
    Field = Field.TaskActualDuration
};

view.Table.TableFields.Add(newColumn);

// WriteViewData bayrağı, görünüm özelliklerinin değişikliklerini kalıcı hale getirmek için kullanılmalıdır.
project.Save(OutDir + "ModifyView_output.mpp", new Saving.MPPSaveOptions
{
    WriteViewData = true
});
```

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


