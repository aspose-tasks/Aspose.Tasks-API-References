---
title: "ExtendedAttributeDefinition.CreateTaskDefinition"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ExtendedAttributeDefinition yöntemi. Microsoft Project'in \"None\" olarak gösterdiği basit bir genişletilmiş nitelik tanımı oluşturan fabrika yöntemi. CalculationType değeri None olarak ayarlanmıştır ve yalnızca Görevlerde kullanılabilir. Bu yöntemi çağırırken customFieldType, fieldId ve alias belirtmeniz gerekir."
type: docs
weight: 40
url: /tr/net/aspose.tasks/extendedattributedefinition/createtaskdefinition/
---
## CreateTaskDefinition(CustomFieldType, ExtendedAttributeTask, string) {#createtaskdefinition}

Basit bir genişletilmiş nitelik tanımı oluşturan fabrika yöntemi, Microsoft Project'in "None" olarak gösterdiği gibi. [`CalculationType`](../calculationtype/) değeri None olarak ayarlanmıştır ve yalnızca Görevlerde kullanılabilir. Bu yöntemi çağırırken *customFieldType*, *fieldId* ve *alias* belirtmeniz gerekir.

```csharp
public static ExtendedAttributeDefinition CreateTaskDefinition(CustomFieldType customFieldType, 
    ExtendedAttributeTask fieldId, string alias)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| customFieldType | CustomFieldType | Belirtilen [`CustomFieldType`](../../customfieldtype/) türü. |
| fieldId | ExtendedAttributeTask | Belirtilen [`ExtendedAttributeTask`](../../extendedattributetask/) alan kimliği. |
| alias | Dize | Belirtilen String alias. |

### Dönüş Değeri

Belirtilen *customFieldType*, *fieldId* ve *alias* ile [`ExtendedAttributeDefinition`](../) sınıfının bir örneği oluşturuldu.

## Örnekler

Bu örneği kullanarak özel bir metin alanı tanımı oluşturun:

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text27, "My custom field");
project.ExtendedAttributes.Add(taskTextAttr);
```

Görevlerin genişletilmiş özniteliklerinin nasıl oluşturulacağını gösterir.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// Text1 türünde bir Genişletilmiş Öznitelik Tanımı oluşturun
var taskExtendedAttributeText1Definition =
    ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text1, "Task City Name");

// Bunu projenin Genişletilmiş Öznitelikler koleksiyonuna ekleyin
project.ExtendedAttributes.Add(taskExtendedAttributeText1Definition);

// Projeye bir görev ekleyin
var task = project.RootTask.Children.Add("Task 1");

// Öznitelik Tanımından bir Genişletilmiş Öznitelik oluşturun
var taskExtendedAttributeText1 = taskExtendedAttributeText1Definition.CreateExtendedAttribute();

// Oluşturulan Genişletilmiş Özniteliğe bir değer atayın. Öznitelik tipi "Text" olup, "TextValue" özelliği kullanılmalıdır.
taskExtendedAttributeText1.TextValue = "London";

// Genişletilmiş Özniteliği göreve ekleyin
task.ExtendedAttributes.Add(taskExtendedAttributeText1);

project.Save(OutDir + "PlainTextExtendedAttribute_out.mpp", SaveFileFormat.Mpp);

var project4 = new Project(DataDir + "Blank2010.mpp");

// Text2 türünde bir Genişletilmiş Öznitelik Tanımı oluşturun
var taskExtendedAttributeText2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Text,
    ExtendedAttributeTask.Text2,
    "Task Towns Name");

// Genişletilmiş öznitelik tanımı için arama değerleri ekleyin
taskExtendedAttributeText2Definition.AddLookupValue(new Value { Id = 1, StringValue = "Town1", Description = "This is Town1" });
taskExtendedAttributeText2Definition.AddLookupValue(new Value { Id = 2, StringValue = "Town2", Description = "This is Town2" });

// Bunu projenin Genişletilmiş Öznitelikler koleksiyonuna ekleyin
project4.ExtendedAttributes.Add(taskExtendedAttributeText2Definition);

// Projeye bir görev ekleyin
var task2 = project4.RootTask.Children.Add("Task 2");

// Id 1 için Text2 Arama Tanımından bir Genişletilmiş Öznitelik oluşturun
var taskExtendedAttributeText2 = taskExtendedAttributeText2Definition.CreateExtendedAttribute(taskExtendedAttributeText2Definition.ValueList[1]);

// Genişletilmiş Özniteliği göreve ekleyin
task2.ExtendedAttributes.Add(taskExtendedAttributeText2);

project4.Save(OutDir + "TextExtendedAttributeWithLookup_out.mpp", SaveFileFormat.Mpp);

var project2 = new Project(DataDir + "Blank2010.mpp");

// Duration2 türünde bir Genişletilmiş Öznitelik Tanımı oluşturun
var taskExtendedAttributeDuration2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Duration,
    ExtendedAttributeTask.Duration2,
    "Some duration");

// Genişletilmiş öznitelik tanımı için arama değerleri ekleyin
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 2, Duration = project2.GetDuration(4, TimeUnitType.Hour), Description = "4 hours" });
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 3, Duration = project2.GetDuration(1, TimeUnitType.Day), Description = "1 day" });
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 4, Duration = project2.GetDuration(1, TimeUnitType.Hour), Description = "1 hour" });
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 7, Duration = project2.GetDuration(10, TimeUnitType.Day), Description = "10 days" });

// Tanımı projenin Genişletilmiş Öznitelikler koleksiyonuna ekleyin
project2.ExtendedAttributes.Add(taskExtendedAttributeDuration2Definition);

// Projeye bir görev ekleyin
var task3 = project2.RootTask.Children.Add("Task 3");

// Id 3 için Duration2 Arama Tanımından bir Genişletilmiş Öznitelik oluşturun
var taskExtendedAttributeDuration2 =
    taskExtendedAttributeDuration2Definition.CreateExtendedAttribute(taskExtendedAttributeDuration2Definition.ValueList[3]);

// Genişletilmiş Özniteliği göreve ekleyin
task3.ExtendedAttributes.Add(taskExtendedAttributeDuration2);

project2.Save(OutDir + "DurationExtendedAttributeWithLookup_out.mpp", SaveFileFormat.Mpp);

var project3 = new Project(DataDir + "Blank2010.mpp");

// Finish2 türünde bir Genişletilmiş Öznitelik Tanımı oluşturun
var taskExtendedAttributeFinish2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Finish,
    ExtendedAttributeTask.Finish2,
    "Some finish");

// Genişletilmiş öznitelik tanımı için arama değerleri ekleyin
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 2, DateTimeValue = new DateTime(1984, 01, 01, 00, 00, 01), Description = "This is Value2" });
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 3, DateTimeValue = new DateTime(1994, 01, 01, 00, 01, 01), Description = "This is Value3" });
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 4, DateTimeValue = new DateTime(2009, 12, 31, 00, 00, 00), Description = "This is Value4" });
taskExtendedAttributeFinish2Definition.AddLookupValue(new Value { Id = 7, DateTimeValue = DateTime.Now, Description = "This is Value6" });

// Tanımı projenin Genişletilmiş Öznitelikler koleksiyonuna ekleyin
project3.ExtendedAttributes.Add(taskExtendedAttributeFinish2Definition);

// Projeye bir görev ekleyin
var task4 = project3.RootTask.Children.Add("Task 4");

// Id 3 için Finish2 Arama Tanımından bir Genişletilmiş Öznitelik oluşturun
var taskExtendedAttributeFinish2 = taskExtendedAttributeFinish2Definition.CreateExtendedAttribute(taskExtendedAttributeFinish2Definition.ValueList[3]);

// Genişletilmiş Özniteliği göreve ekleyin
task4.ExtendedAttributes.Add(taskExtendedAttributeFinish2);

project3.Save(OutDir + "FinishExtendedAttributeWithLookup_out.mpp", SaveFileFormat.Mpp);
```

### Ayrıca Bakınız

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateTaskDefinition(ExtendedAttributeTask, string) {#createtaskdefinition_1}

Basit bir genişletilmiş öznitelik tanımı oluşturan fabrika yöntemi, Microsoft Project'te "None" olarak gösterilir. [`CalculationType`](../calculationtype/) değeri None'dur ve yalnızca Görevlerde kullanılabilir. Bu yöntemi çağırırken *fieldId* ve *alias* belirtmeniz gerekir. Alan tipi, alan kimliğinden türetilir.

```csharp
public static ExtendedAttributeDefinition CreateTaskDefinition(ExtendedAttributeTask fieldId, 
    string alias)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fieldId | ExtendedAttributeTask | Belirtilen [`ExtendedAttributeTask`](../../extendedattributetask/) alan kimliği. |
| alias | Dize | Belirtilen String alias. |

### Dönüş Değeri

Belirtilen *fieldId* ve *alias* ile [`ExtendedAttributeDefinition`](../) sınıfının bir örneği oluşturuldu.

## Örnekler

Bu örneği kullanarak özel bir metin alanı tanımı oluşturun:

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text27, "My custom field");
project.ExtendedAttributes.Add(taskTextAttr);
```

Genişletilmiş öznitelik tanımının nasıl oluşturulacağını ve öznitelik oluşturulurken bir dize değeri ayarlanacağını gösterir.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, "My Text");
project.ExtendedAttributes.Add(definition);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 22, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// 'Common Info' değerine eşit bir genişletilmiş öznitelik oluştur
var extendedAttribute = definition.CreateExtendedAttribute("Common Info");

// 'Common Info' değeriyle başlatılan genişletilmiş özniteliği ekle
task.ExtendedAttributes.Add(extendedAttribute);
```

### Ayrıca Bakınız

* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


