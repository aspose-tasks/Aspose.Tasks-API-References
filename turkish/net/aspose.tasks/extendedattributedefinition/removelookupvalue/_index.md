---
title: "ExtendedAttributeDefinition.RemoveLookupValue"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ExtendedAttributeDefinition yöntemi. İç arama listesinden bir değeri kaldırır. Bu, ValueList ile manipülasyonlar için tercih edilen bir yoldur."
type: docs
weight: 340
url: /tr/net/aspose.tasks/extendedattributedefinition/removelookupvalue/
---
## ExtendedAttributeDefinition.RemoveLookupValue method

İç arama listesinden bir değeri kaldırır. Bu, [`ValueList`](../valuelist/) ile manipülasyonlar için tercih edilen bir yoldur.

```csharp
public void RemoveLookupValue(Value value)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | Değer | Aramadan kaldırılacak değer. |

## Açıklamalar

Bu yöntem yalnızca [`ExtendedAttributeDefinition`](../) örnekleri için çalışır ve bunların [`CalculationType`](../calculationtype/) değeri Lookup'a eşittir.

## Örnekler

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

* class [Value](../../value/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


