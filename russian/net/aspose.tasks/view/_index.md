---
title: "Класс View"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.View. Представляет представление в Project"
type: docs
weight: 2890
url: /ru/net/aspose.tasks/view/
---
## View class

Представляет представление в Project.

```csharp
public class View : IComparable<View>
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [View](view/#constructor)() | Инициализирует новый экземпляр класса `View`. |
| [View](view/#constructor_1)(ViewScreen) | Инициализирует новый экземпляр класса `View`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [Filter](../../aspose.tasks/view/filter/) { get; set; } | Получает или задает фильтр, используемый в отдельном представлении. |
| [Group](../../aspose.tasks/view/group/) { get; set; } | Получает или задает группу отдельного представления. |
| [HighlightFilter](../../aspose.tasks/view/highlightfilter/) { get; set; } | Получает или задает значение, указывающее, выделяет ли Microsoft Project фильтр для отдельного представления. |
| [Name](../../aspose.tasks/view/name/) { get; set; } | Получает или задает имя объекта View. |
| [PageInfo](../../aspose.tasks/view/pageinfo/) { get; } | Получает экземпляр класса [`PageInfo`](./pageinfo/). Представляет данные настройки страницы, присутствующие в формате файла mpp. |
| [ParentProject](../../aspose.tasks/view/parentproject/) { get; } | Получает родителя объекта View. Только для чтения [`Project`](../project/). |
| [Screen](../../aspose.tasks/view/screen/) { get; } | Получает тип экрана для отдельного представления. Только для чтения [`ViewScreen`](../viewscreen/). |
| [ShowInMenu](../../aspose.tasks/view/showinmenu/) { get; set; } | Получает или задает значение, указывающее, отображает ли Microsoft Project имя отдельного представления в выпадающих списках View или Other Views на ленте. |
| [Table](../../aspose.tasks/view/table/) { get; set; } | Получает или задает таблицу отдельного представления. |
| [Type](../../aspose.tasks/view/type/) { get; } | Получает тип элемента в отдельном представлении, например задачи или ресурсы. Только для чтения [`ItemType`](../itemtype/). |
| [Uid](../../aspose.tasks/view/uid/) { get; } | Получает уникальный идентификатор представления. |
| [VisualObjectsPlacements](../../aspose.tasks/view/visualobjectsplacements/) { get; } | Получает коллекцию объектов, представляющих размещение и внешний вид [`OleObject`](../oleobject/) в представлении. |

## Методы

| Имя | Описание |
| --- | --- |
| [CompareTo](../../aspose.tasks/view/compareto/)(View) | Сравнивает текущий экземпляр с другим объектом того же типа и возвращает целое число, указывающее, предшествует ли текущий экземпляр, следует за ним или находится в том же положении в порядке сортировки, что и другой объект. |
| override [Equals](../../aspose.tasks/view/equals/)(object) | Возвращает значение, указывающее, равен ли этот экземпляр указанному объекту. |
| override [GetHashCode](../../aspose.tasks/view/gethashcode/)() | Возвращает значение хеш-кода для экземпляра класса [`Resource`](../resource/). |
| [operator ==](../../aspose.tasks/view/op_equality/) | Возвращает значение, указывающее, равен ли этот экземпляр указанному объекту. |
| [operator &gt;](../../aspose.tasks/view/op_greaterthan/) | Возвращает значение, указывающее, больше ли этот экземпляр указанного объекта. |
| [operator &gt;=](../../aspose.tasks/view/op_greaterthanorequal/) | Возвращает значение, указывающее, больше ли или равен этот экземпляр указанному объекту. |
| [operator !=](../../aspose.tasks/view/op_inequality/) | Возвращает значение, указывающее, не равен ли этот экземпляр указанному объекту. |
| [operator &lt;](../../aspose.tasks/view/op_lessthan/) | Возвращает значение, указывающее, меньше ли этот экземпляр указанного объекта. |
| [operator &lt;=](../../aspose.tasks/view/op_lessthanorequal/) | Возвращает значение, указывающее, меньше ли или равен этот экземпляр указанному объекту. |

## Примеры

Показывает, как работать с представлением Project и добавить столбец в представление по умолчанию (которое отображается при открытии файла MPP в MS Project).

```csharp
// создать пустой проект без представлений
var project = new Project();
project.Set(Prj.Name, "Test View Project");

// Изменить представление по умолчанию (это представление диаграммы Ганта).
// Или вы можете выбрать представление по имени или через экран представлений, используя коллекцию project.View.
var view = (GanttChartView) project.DefaultView;

TableField newColumn = new TableField()
{
    AlignData = HorizontalStringAlignment.Center,
    Title = "My new column",
    Width = 30,
    Field = Field.TaskActualDuration
};

view.Table.TableFields.Add(newColumn);

// Флаг WriteViewData следует использовать для сохранения изменений свойств представления.
project.Save(OutDir + "ModifyView_output.mpp", new Saving.MPPSaveOptions
{
    WriteViewData = true
});
```

Показывает, как работать с представлениями MS Project.

```csharp
// создать пустой проект без представлений
var project = new Project();
project.Set(Prj.Name, "Test View Project");

// создать стандартное представление диаграммы Ганта
View view = new GanttChartView();

// установить некоторые свойства представления
// установить значение, указывающее, отображает ли Microsoft Project имя отдельного представления в списках View или Other Views в ленте
view.ShowInMenu = true;
// установить значение, указывающее, выделяет ли Microsoft Project фильтр для отдельного представления
view.HighlightFilter = true;

// запись следующих свойств не поддерживается
// устанавливает фильтр, используемый в отдельном представлении
view.Filter = null;
// устанавливает группу отдельного представления
view.Group = null;
// устанавливает таблицу отдельного представления
view.Table = null;

// настроим некоторые параметры представления
// установить количество первых столбцов, печатаемых на всех страницах
view.PageInfo.PageViewSettings.FirstColumnsCount = 4;
// установить значение, указывающее, печатать ли указанное количество первых столбцов на всех страницах
view.PageInfo.PageViewSettings.PrintFirstColumnsCountOnAllPages = true;

// добавить представление в наш проект
project.Views.Add(view);

// Флаг WriteViewData следует использовать для сохранения изменений project.Views.
project.Save(OutDir + "WorkWithView_output.mpp", new Saving.MPPSaveOptions
{
    WriteViewData = true
});
// проверим некоторые свойства недавно добавленного представления
// вывести уникальный идентификатор представления
Console.WriteLine("View Uid: " + view.Uid);
// вывести тип экрана для отдельного представления
Console.WriteLine("View Screen: " + view.Screen);
Console.WriteLine("View Type: " + view.Type);
Console.WriteLine("Parent Project of the view: " + view.ParentProject.Get(Prj.Name));
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


