---
title: "Project.DefaultView"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Project özelliği. Projenin varsayılan görünümünü alır veya ayarlar."
type: docs
weight: 360
url: /tr/net/aspose.tasks/project/defaultview/
---
## Project.DefaultView property

Projenin varsayılan görünümünü alır veya ayarlar.

```csharp
public View DefaultView { get; set; }
```

## Örnekler

Bir projenin varsayılan görünümüyle nasıl çalışılacağını gösterir.

```csharp
var project = new Project(DataDir + "TaskUsageViewWithDetails.mpp");

// Varsayılan görünümü al
UsageView view = (TaskUsageView)project.DefaultView;

// Ayrıntılar başlık sütunu görüntülenmeyecek
view.DisplayDetailsHeaderColumn = false;
view.RepeatDetailsHeaderOnAllRows = false;
view.AlignDetailsData = HorizontalStringAlignment.Near;
project.Save(OutDir + "task usage1_out.pdf", SaveFileFormat.Pdf);

// Ayrıntılar başlık sütununu göster
view.DisplayDetailsHeaderColumn = true;

// Tüm atama satırlarında ayrıntılar başlığını tekrarla
view.RepeatDetailsHeaderOnAllRows = true;
view.AlignDetailsData = HorizontalStringAlignment.Far;
project.Save(OutDir + "task usage2_out.pdf", SaveFileFormat.Pdf);
```

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

### Ayrıca Bakınız

* class [View](../../view/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


