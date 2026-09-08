---
title: "Класс TableField"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.TableField. Представляет поле таблицы в проекте."
type: docs
weight: 2340
url: /ru/net/aspose.tasks/tablefield/
---
## TableField class

Представляет поле таблицы в проекте.

```csharp
public class TableField
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [TableField](tablefield/)() | Инициализирует новый экземпляр класса `TableField`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [AlignData](../../aspose.tasks/tablefield/aligndata/) { get; set; } | Возвращает или задает выравнивание данных в поле таблицы. |
| [AlignTitle](../../aspose.tasks/tablefield/aligntitle/) { get; set; } | Возвращает или задает выравнивание заголовка в поле таблицы. |
| [Field](../../aspose.tasks/tablefield/field/) { get; set; } | Возвращает или задает тип поля таблицы. |
| [Title](../../aspose.tasks/tablefield/title/) { get; set; } | Возвращает или задает заголовок поля в таблице. |
| [Width](../../aspose.tasks/tablefield/width/) { get; set; } | Возвращает или задает ширину в пунктах столбца поля в таблице. |
| [WrapHeader](../../aspose.tasks/tablefield/wrapheader/) { get; set; } | Возвращает или задает значение, указывающее, может ли заголовок столбца таблицы переноситься на несколько строк или должен обрезаться, когда превышает ширину столбца. |
| [WrapText](../../aspose.tasks/tablefield/wraptext/) { get; set; } | Получает или задает значение, указывающее, может ли текст столбца переноситься на несколько строк или должен обрезаться, когда превышает ширину столбца. Поддерживается версией MSP 2010 и более поздними. |

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

Показывает, как читать таблицы проекта.

```csharp
var project = new Project(DataDir + "ReadTableData.mpp");

// получить таблицу
var table = project.Tables.ToList()[0];
Console.WriteLine("Print table fields of {0}", table.Name);
Console.WriteLine("Table Fields Count" + table.TableFields.Count);

// отобразить информацию обо всех полях таблицы
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

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


