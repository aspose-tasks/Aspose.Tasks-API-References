---
title: "Класс OutlineCodeDefinition"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.OutlineCodeDefinition. Представляет определение кода структуры."
type: docs
weight: 1170
url: /ru/net/aspose.tasks/outlinecodedefinition/
---
## OutlineCodeDefinition class

Представляет определение кода структуры.

```csharp
public sealed class OutlineCodeDefinition
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [OutlineCodeDefinition](outlinecodedefinition/)() | Инициализирует новый экземпляр класса `OutlineCodeDefinition`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [Alias](../../aspose.tasks/outlinecodedefinition/alias/) { get; set; } | Возвращает или задает псевдоним пользовательского кода структуры. |
| [AllLevelsRequired](../../aspose.tasks/outlinecodedefinition/alllevelsrequired/) { get; set; } | Возвращает или задает значение, указывающее, должны ли новые коды иметь все уровни. Недоступно для корпоративных кодов. |
| [Enterprise](../../aspose.tasks/outlinecodedefinition/enterprise/) { get; set; } | Возвращает или задает значение, указывающее, является ли пользовательский код структуры корпоративным пользовательским кодом структуры. |
| [EnterpriseOutlineCodeAlias](../../aspose.tasks/outlinecodedefinition/enterpriseoutlinecodealias/) { get; set; } | Возвращает или задает ссылку на другое пользовательское поле, для которого это определение кода структуры является псевдонимом. |
| [FieldId](../../aspose.tasks/outlinecodedefinition/fieldid/) { get; set; } | Возвращает или задает номер поля кода структуры. |
| [FieldName](../../aspose.tasks/outlinecodedefinition/fieldname/) { get; set; } | Возвращает или задает имя пользовательского кода структуры. |
| [Guid](../../aspose.tasks/outlinecodedefinition/guid/) { get; set; } | Возвращает или задает Guid кода структуры. |
| [LeafOnly](../../aspose.tasks/outlinecodedefinition/leafonly/) { get; set; } | Возвращает или задает значение, указывающее, должны ли значения, указанные в этом поле кода структуры, быть конечными (leaf) значениями. |
| [Masks](../../aspose.tasks/outlinecodedefinition/masks/) { get; } | Возвращает объект OutlineMaskCollection. Таблица записей, определяющих маску кода структуры. Экземпляр только для чтения [`OutlineMaskCollection`](../outlinemaskcollection/) . |
| [OnlyTableValuesAllowed](../../aspose.tasks/outlinecodedefinition/onlytablevaluesallowed/) { get; set; } | Возвращает или задает значение, указывающее, должны ли указанные значения поступать из таблицы значений. |
| [PhoneticAlias](../../aspose.tasks/outlinecodedefinition/phoneticalias/) { get; set; } | Возвращает или задает фонетическое произношение псевдонима пользовательского кода структуры. |
| [ResourceSubstitutionEnabled](../../aspose.tasks/outlinecodedefinition/resourcesubstitutionenabled/) { get; set; } | Возвращает или задает значение, указывающее, может ли пользовательский код структуры использоваться мастером подстановки ресурсов в Microsoft Project. |
| [ShowIndent](../../aspose.tasks/outlinecodedefinition/showindent/) { get; set; } | Возвращает или задает значение, указывающее, должны ли отступы этого кода структуры отображаться. |
| [Values](../../aspose.tasks/outlinecodedefinition/values/) { get; } | Получает объект OutlineValueCollection. Значения таблицы, связанные с этим кодом структуры. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


