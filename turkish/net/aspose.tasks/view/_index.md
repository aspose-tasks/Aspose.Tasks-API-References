---
title: "Sınıf View"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.View sınıfı. Project içinde bir görünümü temsil eder"
type: docs
weight: 2890
url: /tr/net/aspose.tasks/view/
---
## View class

Project içinde bir görünümü temsil eder.

```csharp
public class View : IComparable<View>
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [View](view/#constructor)() | Yeni bir `View` sınıfı örneği başlatır. |
| [View](view/#constructor_1)(ViewScreen) | Yeni bir `View` sınıfı örneği başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Filter](../../aspose.tasks/view/filter/) { get; set; } | Tek bir görünümde kullanılan bir filtreyi alır veya ayarlar. |
| [Group](../../aspose.tasks/view/group/) { get; set; } | Tek bir görünümün grubunu alır veya ayarlar. |
| [HighlightFilter](../../aspose.tasks/view/highlightfilter/) { get; set; } | Microsoft Project'in tek bir görünüm için filtreyi vurgulayıp vurgulamayacağını belirten bir değeri alır veya ayarlar. |
| [Name](../../aspose.tasks/view/name/) { get; set; } | Bir View nesnesinin adını alır veya ayarlar. |
| [PageInfo](../../aspose.tasks/view/pageinfo/) { get; } | [`PageInfo`](./pageinfo/) sınıfının bir örneğini alır. mpp dosya formatında bulunan sayfa ayarı verilerini temsil eder. |
| [ParentProject](../../aspose.tasks/view/parentproject/) { get; } | View nesnesinin üst nesnesini alır. Salt okunur [`Project`](../project/). |
| [Screen](../../aspose.tasks/view/screen/) { get; } | Tek bir görünüm için ekran tipini alır. Salt okunur [`ViewScreen`](../viewscreen/). |
| [ShowInMenu](../../aspose.tasks/view/showinmenu/) { get; set; } | Microsoft Project'in tek bir görünüm adını Şerit'teki Görünüm veya Diğer Görünümler açılır listelerinde gösterip göstermeyeceğini belirten bir değeri alır veya ayarlar. |
| [Table](../../aspose.tasks/view/table/) { get; set; } | Tek bir görünümün tablosunu alır veya ayarlar. |
| [Type](../../aspose.tasks/view/type/) { get; } | Tek bir görünümdeki öğenin türünü alır, örneğin görevler veya kaynaklar. Salt okunur [`ItemType`](../itemtype/). |
| [Uid](../../aspose.tasks/view/uid/) { get; } | Bir görünümün benzersiz tanımlayıcısını alır. |
| [VisualObjectsPlacements](../../aspose.tasks/view/visualobjectsplacements/) { get; } | Görünümdeki [`OleObject`](../oleobject/) yerleşimini ve görünümünü temsil eden nesneler koleksiyonunu alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [CompareTo](../../aspose.tasks/view/compareto/)(View) | Mevcut örneği aynı türdeki başka bir nesneyle karşılaştırır ve mevcut örneğin diğer nesneye göre sıralama düzeninde önce mi, sonra mı yoksa aynı konumda mı olduğunu belirten bir tam sayı döndürür. |
| override [Equals](../../aspose.tasks/view/equals/)(object) | Bu örneğin belirtilen nesneye eşit olup olmadığını gösteren bir değer döndürür. |
| override [GetHashCode](../../aspose.tasks/view/gethashcode/)() | [`Resource`](../resource/) sınıfının örneği için bir karma kod değeri döndürür. |
| [operator ==](../../aspose.tasks/view/op_equality/) | Bu örneğin belirtilen nesneye eşit olup olmadığını gösteren bir değer döndürür. |
| [operator &gt;](../../aspose.tasks/view/op_greaterthan/) | Bu örneğin belirtilen nesneden büyük olup olmadığını gösteren bir değer döndürür. |
| [operator &gt;=](../../aspose.tasks/view/op_greaterthanorequal/) | Bu örneğin belirtilen nesneden büyük veya ona eşit olup olmadığını gösteren bir değer döndürür. |
| [operator !=](../../aspose.tasks/view/op_inequality/) | Bu örneğin belirtilen nesneye eşit olmadığını gösteren bir değer döndürür. |
| [operator &lt;](../../aspose.tasks/view/op_lessthan/) | Bu örneğin belirtilen nesneden küçük olup olmadığını gösteren bir değer döndürür. |
| [operator &lt;=](../../aspose.tasks/view/op_lessthanorequal/) | Bu örneğin belirtilen nesneden küçük veya ona eşit olup olmadığını gösteren bir değer döndürür. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


