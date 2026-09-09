---
title: "View.ShowInMenu"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "View özelliği. Microsoft Project'in Tek Görünüm adını Görünüm veya Diğer Görünümler açılır menülerinde Şerit'te gösterip göstermediğini belirten bir değeri alır veya ayarlar."
type: docs
weight: 90
url: /tr/net/aspose.tasks/view/showinmenu/
---
## View.ShowInMenu property

Microsoft Project'in tek bir görünüm adını Şerit'teki Görünüm veya Diğer Görünümler açılır listelerinde gösterip göstermeyeceğini belirten bir değeri alır veya ayarlar.

```csharp
public bool ShowInMenu { get; set; }
```

## Örnekler

MS Project görünümleriyle nasıl çalışılacağını gösterir.

```csharp
// görünümler olmadan boş bir proje oluştur
var project = new Project();
project.Set(Prj.Name, "Test View Project");

// standart bir Gantt şeması görünümü oluştur
View view = new GanttChartView();

// bazı görünüm özelliklerini ayarla
// Microsoft Project'in Tek Görünüm adını Görünümde mi yoksa Şeritteki Diğer Görünümler açılır listelerinde mi gösterdiğini belirten bir değer ayarla
view.ShowInMenu = true;
// Microsoft Project'in tek bir görünüm için filtreyi vurgulayıp vurgulamadığını belirten bir değer ayarla
view.HighlightFilter = true;

// sonraki özelliklerin yazılması desteklenmiyor
// tek bir görünümde kullanılan filtreyi ayarlar
view.Filter = null;
// tek bir görünümün grubunu ayarlar
view.Group = null;
// tek bir görünümün tablosunu ayarlar
view.Table = null;

// bazı görünüm ayarlarını ayarlayalım
// tüm sayfalarda yazdırılacak ilk sütun sayısını ayarla
view.PageInfo.PageViewSettings.FirstColumnsCount = 4;
// tüm sayfalarda belirli sayıda ilk sütunun yazdırılıp yazdırılmayacağını belirten bir değer ayarla
view.PageInfo.PageViewSettings.PrintFirstColumnsCountOnAllPages = true;

// görünümü projemize ekle
project.Views.Add(view);

// WriteViewData bayrağı, project.Views üzerindeki değişiklikleri kalıcı kılmak için kullanılmalıdır.
project.Save(OutDir + "WorkWithView_output.mpp", new Saving.MPPSaveOptions
{
    WriteViewData = true
});
// yeni eklenen görünümün bazı özelliklerini kontrol edelim
// bir görünümün benzersiz tanımlayıcısını yazdır
Console.WriteLine("View Uid: " + view.Uid);
// tek bir görünüm için ekran tipini yazdır
Console.WriteLine("View Screen: " + view.Screen);
Console.WriteLine("View Type: " + view.Type);
Console.WriteLine("Parent Project of the view: " + view.ParentProject.Get(Prj.Name));
```

### Ayrıca Bakınız

* class [View](../)
* namespace [Aspose.Tasks](../../view/)
* assembly [Aspose.Tasks](../../../)


