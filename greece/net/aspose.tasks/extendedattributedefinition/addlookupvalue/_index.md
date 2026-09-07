---
title: "ExtendedAttributeDefinition.AddLookupValue"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος ExtendedAttributeDefinition. Προσθέτει μια τιμή στη εσωτερική λίστα αναζήτησης. Αυτός είναι ο προτιμώμενος τρόπος για χειρισμούς με το ValueList"
type: docs
weight: 300
url: /el/net/aspose.tasks/extendedattributedefinition/addlookupvalue/
---
## ExtendedAttributeDefinition.AddLookupValue method

Προσθέτει μια τιμή στη εσωτερική λίστα αναζήτησης. Αυτός είναι ο προτιμώμενος τρόπος για χειρισμούς με το [`ValueList`](../valuelist/).

```csharp
public void AddLookupValue(Value value)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | Τιμή | Τιμή προς προσθήκη στην αναζήτηση. |

## Παρατηρήσεις

Αυτή η μέθοδος λειτουργεί μόνο για στιγμιότυπα του [`ExtendedAttributeDefinition`](../) που έχουν το [`CalculationType`](../calculationtype/) ίσο με Lookup.

## Παραδείγματα

Χρησιμοποιήστε αυτόν τον κώδικα για να προσθέσετε νέα τιμή στη λίστα αναζήτησης:

```csharp
taskTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
```

Δείχνει πώς να προσθέσετε εκτεταμένα χαρακτηριστικά με αναζητήσεις για αναθέσεις.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// Αναθέστε τον πόρο "1 TRG: Trade Group" στο "TASK 1" δημιουργώντας ένα αντικείμενο ResourceAssignment.
var resource = project.Resources.GetById(1);
var task = project.RootTask.Children.GetById(1);
var assignment = project.ResourceAssignments.Add(task, resource);

// Δημιουργήστε ορισμό προσαρμοσμένου χαρακτηριστικού με αναζήτηση.
var resExtendedAttributeDefinition = ExtendedAttributeDefinition.CreateLookupResourceDefinition(
    CustomFieldType.Cost,
    ExtendedAttributeResource.Cost5,
    "My lookup resource cost");
project.ExtendedAttributes.Add(resExtendedAttributeDefinition);

var firstValue = new Value { NumericValue = 1500, Description = "Val 1", Id = 1, Val = "1500" };
var secondValue = new Value { NumericValue = 2500, Description = "Val 2", Id = 2 };
resExtendedAttributeDefinition.AddLookupValue(firstValue);
resExtendedAttributeDefinition.AddLookupValue(secondValue);

// Αυτή η τιμή μπορεί να εμφανιστεί στην προβολή "Resource usage" του MS Project.
var attributeValue = resExtendedAttributeDefinition.CreateExtendedAttribute(firstValue);
assignment.ExtendedAttributes.Add(attributeValue);

// Δημιουργήστε ορισμό προσαρμοσμένου χαρακτηριστικού με αναζήτηση.
var taskCostAttr = ExtendedAttributeDefinition.CreateLookupTaskDefinition(CustomFieldType.Cost, ExtendedAttributeTask.Cost4, "My lookup task cost");
project.ExtendedAttributes.Add(taskCostAttr);
var taskFirstValue = new Value { NumericValue = 18, Description = "Task val 1", Id = 3, Val = "18" };
var resSecondValue = new Value { NumericValue = 30, Description = "Task val 2", Id = 4 };
var taskWrongValue = new Value { NumericValue = 99, Description = "Task val Wrong", Id = 5, Val = "18" };

taskCostAttr.AddLookupValue(taskFirstValue);
resExtendedAttributeDefinition.AddLookupValue(resSecondValue);

// Αυτή η τιμή μπορεί να εμφανιστεί στην προβολή "Task usage" του MS Project.
assignment.ExtendedAttributes.Add(taskCostAttr.CreateExtendedAttribute(taskFirstValue));

// Μπορούν να αφαιρεθούν αργότερα λανθασμένες τιμές
taskCostAttr.RemoveLookupValue(taskWrongValue);

// εργασία με το έργο...
```

### Δείτε επίσης

* class [Value](../../value/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


