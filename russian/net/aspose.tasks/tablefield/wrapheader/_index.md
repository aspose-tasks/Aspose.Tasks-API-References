---
title: "TableField.WrapHeader"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство TableField. Получает или задает значение, указывающее, может ли заголовок столбца таблицы переноситься на несколько строк или должен обрезаться, когда превышает ширину столбца"
type: docs
weight: 70
url: /ru/net/aspose.tasks/tablefield/wrapheader/
---
## TableField.WrapHeader property

Возвращает или задает значение, указывающее, может ли заголовок столбца таблицы переноситься на несколько строк или должен обрезаться, когда превышает ширину столбца.

```csharp
public bool WrapHeader { get; set; }
```

## Примеры

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

* class [TableField](../)
* namespace [Aspose.Tasks](../../tablefield/)
* assembly [Aspose.Tasks](../../../)


