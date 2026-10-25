---
title: "ExtendedAttributeDefinition.CreateLookupTaskDefinition"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ExtendedAttributeDefinition yöntemi. Arama (lookup) içeren bir genişletilmiş öznitelik tanımı oluşturan fabrika yöntemi. CalculationType değeri Lookup'tir ve yalnızca Görevlerde (Tasks) kullanılabilir. Bu yöntemi çağırırken fieldId ve alias belirtmeniz gerekir. Alan türü alan kimliğinden çıkarılır."
type: docs
weight: 20
url: /tr/net/aspose.tasks/extendedattributedefinition/createlookuptaskdefinition/
---
## CreateLookupTaskDefinition(ExtendedAttributeTask, string) {#createlookuptaskdefinition_1}

Arama içeren bir genişletilmiş öznitelik tanımı oluşturan fabrika yöntemi. [`CalculationType`](../calculationtype/) değeri Lookup'tir ve yalnızca Görevlerde (Tasks) kullanılabilir. Bu yöntemi çağırırken *fieldId* ve *alias* belirtmeniz gerekir. Alan türü alan kimliğinden çıkarılır.

```csharp
public static ExtendedAttributeDefinition CreateLookupTaskDefinition(ExtendedAttributeTask fieldId, 
    string alias)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fieldId | ExtendedAttributeTask | Belirtilen [`ExtendedAttributeTask`](../../extendedattributetask/) alan kimliği. |
| alias | Dize | Belirtilen String alias. |

### Dönüş Değeri

Belirtilen *fieldId* ve *alias* ile [`ExtendedAttributeDefinition`](../) sınıfının bir örneği oluşturuldu.

## Örnekler

Arama içeren bir görev için özel alan tanımı oluşturmak ve ardından metin değerleriyle doldurmak için bu örneği kullanın:

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateLookupTaskDefinition(ExtendedAttributeTask.Text27, "My custom field");
taskTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
taskTextAttr.AddLookupValue(new Value { Id = 2, Val = "Text value 2", Description = "Text value description 2" });
project.ExtendedAttributes.Add(taskTextAttr);
```

Güncellenmiş genişletilmiş öznitelik tanımlarının nasıl yazılacağını gösterir.

```csharp
var project = new Project(DataDir + "WriteUpdatedExtendedAttributeDefinitions.mpp");

// Bir arama ve bir arama değeri ile yeni text3 genişletilmiş özniteliği ekle
var definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(ExtendedAttributeTask.Text3, "New text3 attribute");
definition.ElementType = ElementType.Task;
project.ExtendedAttributes.Add(definition);

var textVal = new Value
{
    Id = 1,
    Description = "Text value descr",
    Val = "Text value1"
};

definition.AddLookupValue(textVal);

// Bir arama ve iki maliyet değeri ile yeni cost1 genişletilmiş özniteliği ekle
var taskCostAttributeDefinition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(ExtendedAttributeTask.Cost1, "New cost1 attribute");
project.ExtendedAttributes.Add(taskCostAttributeDefinition);

var costVal1 = new Value
{
    Id = 2,
    Description = "Cost value 1 descr",
    Val = "99900"
};

var costVal2 = new Value
{
    Id = 3,
    Description = "Cost value 2 descr",
    Val = "11100"
};

taskCostAttributeDefinition.AddLookupValue(costVal1);
taskCostAttributeDefinition.AddLookupValue(costVal2);

// Yeni bir görev ekle ve öznitelik arama değerini ata.
var task = project.RootTask.Children.Add("New task");

var taskAttr = taskCostAttributeDefinition.CreateExtendedAttribute(costVal1);
task.ExtendedAttributes.Add(taskAttr);

var taskStartAttributeDefinition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(ExtendedAttributeTask.Start7, "New start 7 attribute");

var startVal = new Value
{
    Id = 4,
    DateTimeValue = DateTime.Now,
    Description = "Start 7 value description"
};

taskStartAttributeDefinition.AddLookupValue(startVal);

project.ExtendedAttributes.Add(taskStartAttributeDefinition);

var taskFinishAttributeDefinition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(ExtendedAttributeTask.Finish4, "New finish 4 attribute");

var finishVal = new Value
{
    Id = 5,
    DateTimeValue = DateTime.Now,
    Description = "Finish 4 value description"
};

taskFinishAttributeDefinition.ValueList.Add(finishVal);

project.ExtendedAttributes.Add(taskFinishAttributeDefinition);

var numberAttributeDefinition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(ExtendedAttributeTask.Number20, "New number attribute");

var val1 = new Value
{
    Id = 6,
    Val = "1",
    Description = "Number 1 value"
};
var val2 = new Value
{
    Id = 7,
    Val = "2",
    Description = "Number 2 value"
};
var val3 = new Value();
val2.Id = 8;
val3.Val = "3";
val3.Description = "Number 3 value";

numberAttributeDefinition.AddLookupValue(val1);
numberAttributeDefinition.AddLookupValue(val2);
numberAttributeDefinition.AddLookupValue(val3);

project.ExtendedAttributes.Add(numberAttributeDefinition);

var rscStartAttributeDefinition = ExtendedAttributeDefinition.CreateLookupResourceDefinition(ExtendedAttributeResource.Start5, "New start5 attribute");

var value = new Value
{
    Id = 9,
    DateTimeValue = DateTime.Now,
    Description = "this is start5 value descr"
};

rscStartAttributeDefinition.AddLookupValue(value);

project.ExtendedAttributes.Add(rscStartAttributeDefinition);

// Arama olmadan bir süre özniteliği tanımla.
var taskDurationAttributeDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Duration1, "New Duration");
project.ExtendedAttributes.Add(taskDurationAttributeDefinition);

// Yeni bir görev ekle ve daha önce tanımlanmış süre özniteliğine süre değerini ata.
var timeTask = project.RootTask.Children.Add("New task");

var durationExtendedAttribute = taskDurationAttributeDefinition.CreateExtendedAttribute();

durationExtendedAttribute.DurationValue = project.GetDuration(3.0, TimeUnitType.Hour);
timeTask.ExtendedAttributes.Add(durationExtendedAttribute);

var options = new MPPSaveOptions
{
    WriteViewData = true
};

project.Save(OutDir + "WriteUpdatedExtendedAttributeDefinitions_out.mpp", options);
```

### Ayrıca Bakınız

* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateLookupTaskDefinition(CustomFieldType, ExtendedAttributeTask, string) {#createlookuptaskdefinition}

Arama içeren bir genişletilmiş öznitelik tanımı oluşturan fabrika yöntemi. [`CalculationType`](../calculationtype/) değeri Lookup'tir ve yalnızca Görevlerde (Tasks) kullanılabilir. Bu yöntemi çağırırken *customFieldType*, *fieldId* ve *alias* belirtmeniz gerekir.

```csharp
public static ExtendedAttributeDefinition CreateLookupTaskDefinition(
    CustomFieldType customFieldType, ExtendedAttributeTask fieldId, string alias)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| customFieldType | CustomFieldType | Belirtilen [`CustomFieldType`](../../customfieldtype/) türü. |
| fieldId | ExtendedAttributeTask | Belirtilen [`ExtendedAttributeTask`](../../extendedattributetask/) alan kimliği. |
| alias | Dize | Belirtilen String alias. |

### Dönüş Değeri

Belirtilen *customFieldType*, *fieldId* ve *alias* ile [`ExtendedAttributeDefinition`](../) sınıfının bir örneği oluşturuldu.

## Örnekler

Arama içeren bir görev için özel alan tanımı oluşturmak ve ardından metin değerleriyle doldurmak için bu örneği kullanın:

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateLookupTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text27, "My custom field");
taskTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
taskTextAttr.AddLookupValue(new Value { Id = 2, Val = "Text value 2", Description = "Text value description 2" });
project.ExtendedAttributes.Add(taskTextAttr);
```

Atamalar için aramaları içeren genişletilmiş özniteliklerin nasıl ekleneceğini gösterir.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// ResourceAssignment nesnesi oluşturarak "1 TRG: Trade Group" kaynağını "TASK 1" görevine atayın.
var resource = project.Resources.GetById(1);
var task = project.RootTask.Children.GetById(1);
var assignment = project.ResourceAssignments.Add(task, resource);

// Aramayı içeren özel öznitelik tanımı oluştur.
var resExtendedAttributeDefinition = ExtendedAttributeDefinition.CreateLookupResourceDefinition(
    CustomFieldType.Cost,
    ExtendedAttributeResource.Cost5,
    "My lookup resource cost");
project.ExtendedAttributes.Add(resExtendedAttributeDefinition);

var firstValue = new Value { NumericValue = 1500, Description = "Val 1", Id = 1, Val = "1500" };
var secondValue = new Value { NumericValue = 2500, Description = "Val 2", Id = 2 };
resExtendedAttributeDefinition.AddLookupValue(firstValue);
resExtendedAttributeDefinition.AddLookupValue(secondValue);

// Bu değer, MS Project'in "Resource usage" görünümünde görülebilir.
var attributeValue = resExtendedAttributeDefinition.CreateExtendedAttribute(firstValue);
assignment.ExtendedAttributes.Add(attributeValue);

// Aramayı içeren özel öznitelik tanımı oluştur.
var taskCostAttr = ExtendedAttributeDefinition.CreateLookupTaskDefinition(CustomFieldType.Cost, ExtendedAttributeTask.Cost4, "My lookup task cost");
project.ExtendedAttributes.Add(taskCostAttr);
var taskFirstValue = new Value { NumericValue = 18, Description = "Task val 1", Id = 3, Val = "18" };
var resSecondValue = new Value { NumericValue = 30, Description = "Task val 2", Id = 4 };
var taskWrongValue = new Value { NumericValue = 99, Description = "Task val Wrong", Id = 5, Val = "18" };

taskCostAttr.AddLookupValue(taskFirstValue);
resExtendedAttributeDefinition.AddLookupValue(resSecondValue);

// Bu değer, MS Project'in "Task usage" görünümünde görülebilir.
assignment.ExtendedAttributes.Add(taskCostAttr.CreateExtendedAttribute(taskFirstValue));

// yanlış değerler daha sonra kaldırılabilir
taskCostAttr.RemoveLookupValue(taskWrongValue);

// projeyle çalışılıyor...
```

### Ayrıca Bakınız

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


