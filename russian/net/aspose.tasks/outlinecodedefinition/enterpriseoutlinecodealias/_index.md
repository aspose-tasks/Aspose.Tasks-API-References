---
title: "OutlineCodeDefinition.EnterpriseOutlineCodeAlias"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство OutlineCodeDefinition. Возвращает или задает ссылку на другое пользовательское поле, для которого это определение кода структуры является псевдонимом"
type: docs
weight: 50
url: /ru/net/aspose.tasks/outlinecodedefinition/enterpriseoutlinecodealias/
---
## OutlineCodeDefinition.EnterpriseOutlineCodeAlias property

Возвращает или задает ссылку на другое пользовательское поле, для которого это определение кода структуры является псевдонимом.

```csharp
public int EnterpriseOutlineCodeAlias { get; set; }
```

## Примеры

Показывает, как работать с определениями кодов структуры.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

// создать новое определение кода структуры
var outline = new OutlineCodeDefinition();

// установить номер поля кода структуры
outline.FieldId = ExtendedAttributeTask.OutlineCode7.ToString("D");

// установить имя пользовательского кода структуры
outline.FieldName = "Outline Code1";

// установить Guid кода структуры
outline.Guid = "e6afac06-0d86-4359-a96c-db705e3d2ca8";

// установить значение, указывающее, должны ли значения, указанные в этом поле кода структуры, быть конечными значениями
outline.LeafOnly = false;

// установить псевдоним пользовательского кода структуры
outline.Alias = "My Outline Code";

// установить фонетическое произношение псевдонима пользовательского кода структуры
outline.PhoneticAlias = "Outline Code";

// установить значение, указывающее, должны ли новые коды иметь все уровни. Недоступно для корпоративных кодов.
outline.AllLevelsRequired = true;

// установить значение, указывающее, является ли пользовательский код структуры корпоративным пользовательским кодом структуры
outline.Enterprise = false;

// установить ссылку на другое пользовательское поле, для которого это определение кода структуры является псевдонимом
outline.EnterpriseOutlineCodeAlias = 0;

// добавить маску структуры
var mask = new OutlineMask();
mask.Type = MaskType.Characters;
outline.Masks.Add(mask);

// установить значение, указывающее, должны ли указанные значения поступать из таблицы значений
outline.OnlyTableValuesAllowed = false;

// установить значение, указывающее, может ли пользовательский код структуры использоваться
// в мастере замены ресурсов в Microsoft Project
outline.ResourceSubstitutionEnabled = false;

// установить значение, указывающее, должны ли отступы этого кода структуры отображаться.
outline.ShowIndent = false;

project.OutlineCodes.Add(outline);

var value = new OutlineValue();
value.Value = "Text value 1";
value.ValueId = 1;
value.Type = OutlineValueType.Text;
value.Description = "Text value descr 1";
outline.Values.Add(value);

// ...
```

### См. также

* class [OutlineCodeDefinition](../)
* namespace [Aspose.Tasks](../../outlinecodedefinition/)
* assembly [Aspose.Tasks](../../../)


