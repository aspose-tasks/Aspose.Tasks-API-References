---
title: "Класс ResourceUsageView"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.ResourceUsageView. Представляет представление использования ресурсов в проекте"
type: docs
weight: 1810
url: /ru/net/aspose.tasks/resourceusageview/
---
## ResourceUsageView class

Представляет представление использования ресурсов в проекте.

```csharp
public sealed class ResourceUsageView : UsageView
```

## Свойства

| Имя | Описание |
| --- | --- |
| [AlignDetailsData](../../aspose.tasks/usageview/aligndetailsdata/) { get; set; } | Получает или задает выравнивание данных деталей. |
| [BottomTimescaleTier](../../aspose.tasks/usageview/bottomtimescaletier/) { get; set; } | Получает или задает настройки нижнего уровня шкалы времени представления. [`TimescaleTier`](../../aspose.tasks.visualization/timescaletier/) |
| [DisplayDetailsHeaderColumn](../../aspose.tasks/usageview/displaydetailsheadercolumn/) { get; set; } | Получает или задает значение, указывающее, отображать ли столбец заголовка деталей в представлении или нет. |
| [DisplayShortDetailHeaderNames](../../aspose.tasks/usageview/displayshortdetailheadernames/) { get; set; } | Получает или задает значение, указывающее, отображать ли короткие имена заголовков деталей или нет. |
| [FieldCollection](../../aspose.tasks/resourceusageview/fieldcollection/) { get; } | Получает объект [`ResourceUsageViewFieldCollection`](../resourceusageviewfieldcollection/) этого ResourceUsageView. |
| [Filter](../../aspose.tasks/view/filter/) { get; set; } | Получает или задает фильтр, используемый в отдельном представлении. |
| [Group](../../aspose.tasks/view/group/) { get; set; } | Получает или задает группу отдельного представления. |
| [HighlightFilter](../../aspose.tasks/view/highlightfilter/) { get; set; } | Получает или задает значение, указывающее, выделяет ли Microsoft Project фильтр для отдельного представления. |
| [MiddleTimescaleTier](../../aspose.tasks/usageview/middletimescaletier/) { get; set; } | Получает или задает настройки среднего уровня шкалы времени представления. [`TimescaleTier`](../../aspose.tasks.visualization/timescaletier/). |
| [Name](../../aspose.tasks/view/name/) { get; set; } | Получает или задает имя объекта View. |
| [PageInfo](../../aspose.tasks/view/pageinfo/) { get; } | Получает экземпляр класса [`PageInfo`](../view/pageinfo/). Представляет данные настройки страницы, присутствующие в формате файла mpp. |
| [ParentProject](../../aspose.tasks/view/parentproject/) { get; } | Получает родителя объекта View. Только для чтения [`Project`](../project/). |
| [RepeatDetailsHeaderOnAllRows](../../aspose.tasks/usageview/repeatdetailsheaderonallrows/) { get; set; } | Получает или задает значение, указывающее, повторять ли заголовок деталей во всех строках назначений или нет. |
| [Screen](../../aspose.tasks/view/screen/) { get; } | Получает тип экрана для отдельного представления. Только для чтения [`ViewScreen`](../viewscreen/). |
| [ShowInMenu](../../aspose.tasks/view/showinmenu/) { get; set; } | Получает или задает значение, указывающее, отображает ли Microsoft Project имя отдельного представления в выпадающих списках View или Other Views на ленте. |
| [Table](../../aspose.tasks/view/table/) { get; set; } | Получает или задает таблицу отдельного представления. |
| [TimescaleSizePercentage](../../aspose.tasks/usageview/timescalesizepercentage/) { get; set; } |  |
| [TopTimescaleTier](../../aspose.tasks/usageview/toptimescaletier/) { get; set; } | Получает или задает настройки верхнего уровня шкалы времени представления. [`TimescaleTier`](../../aspose.tasks.visualization/timescaletier/). |
| [Type](../../aspose.tasks/view/type/) { get; } | Получает тип элемента в отдельном представлении, например задачи или ресурсы. Только для чтения [`ItemType`](../itemtype/). |
| [Uid](../../aspose.tasks/view/uid/) { get; } | Получает уникальный идентификатор представления. |
| [VisualObjectsPlacements](../../aspose.tasks/view/visualobjectsplacements/) { get; } | Получает коллекцию объектов, представляющих размещение и внешний вид [`OleObject`](../oleobject/) в представлении. |

## Методы

| Имя | Описание |
| --- | --- |
| [CompareTo](../../aspose.tasks/view/compareto/)(View) | Сравнивает текущий экземпляр с другим объектом того же типа и возвращает целое число, указывающее, предшествует ли текущий экземпляр, следует за ним или находится в том же положении в порядке сортировки, что и другой объект. |
| override [Equals](../../aspose.tasks/view/equals/)(object) | Возвращает значение, указывающее, равен ли этот экземпляр указанному объекту. |
| override [GetHashCode](../../aspose.tasks/view/gethashcode/)() | Возвращает значение хеш-кода для экземпляра класса [`Resource`](../resource/). |

## Примеры

Показывает, как отобразить представление использования ресурсов.

```csharp
var project = new Project(DataDir + "ResourceUsageView.mpp");

// Определите SaveOptions с требуемыми настройками TimeScale как Days
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Days,

    // Установите формат Presentation в ResourceUsage
    PresentationFormat = PresentationFormat.ResourceUsage
};

project.Save(OutDir + "ResourceUsage_days_out.pdf", options);
```

### См. также

* class [UsageView](../usageview/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


