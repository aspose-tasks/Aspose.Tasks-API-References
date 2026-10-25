---
title: "TableTextStyle.Field"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "TableTextStyle özelliği. Stil uygulanacak bir alanı alır veya ayarlar. Field"
type: docs
weight: 20
url: /tr/net/aspose.tasks.visualization/tabletextstyle/field/
---
## TableTextStyle.Field property

Stil uygulanacak bir alanı alır veya ayarlar. `Field`.

```csharp
public Field Field { get; set; }
```

## Örnekler

Bir projedeki farklı metin öğelerini biçimlendirmek için kullanılan tablo metin stillerinin nasıl özelleştirileceğini gösterir.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.NewTasksAreManual, false);

var view = (GanttChartView)project.Views.ToList()[0];

// ilk görev adı metin stilini ayarla
var style1 = new TableTextStyle(1);
// stilin uygulanacağı bir alan ayarla.
style1.Field = Field.TaskName;
// metin stilinin <see cref="P:Aspose.Tasks.Visualization.TextStyle.Font" /> ayarla.
style1.Font = new FontDescriptor("Impact", 12F, FontStyles.Bold | FontStyles.Italic);
// metin stili yazı tipinin punto cinsinden boyutunu ayarla.

// ikinci görev süresi metin stilini ayarla
var style2 = new TableTextStyle(2);
style2.Field = Field.TaskDurationText;
style2.Font = new FontDescriptor("Impact", 16F, FontStyles.Underline);

view.TableTextStyles.Add(style1);
view.TableTextStyles.Add(style2);

SimpleSaveOptions options = new MPPSaveOptions
{
    // görünüm verisinin yazılması gerektiğini gösteren bir bayrak ayarla
    WriteViewData = true
};
project.Save(OutDir + "WorkWithTableTextStyle_out.mpp", options);
```

### Ayrıca Bakınız

* enum [Field](../../../aspose.tasks/field/)
* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)


