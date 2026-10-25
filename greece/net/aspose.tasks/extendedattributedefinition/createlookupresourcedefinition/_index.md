---
title: "ExtendedAttributeDefinition.CreateLookupResourceDefinition"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "ExtendedAttributeDefinition method. Μέθοδος κατασκευής που δημιουργεί έναν ορισμό εκτεταμένου χαρακτηριστικού με αναζήτηση. Έχει CalculationType ίσο με Lookup και μπορεί να χρησιμοποιηθεί μόνο σε Resources. Απαιτείται να καθορίσετε fieldId και alias όταν καλείτε αυτή τη μέθοδο. Ο τύπος του πεδίου προκύπτει από το field id."
type: docs
weight: 10
url: /el/net/aspose.tasks/extendedattributedefinition/createlookupresourcedefinition/
---
## CreateLookupResourceDefinition(ExtendedAttributeResource, string) {#createlookupresourcedefinition_1}

Μέθοδος κατασκευής που δημιουργεί έναν ορισμό εκτεταμένου χαρακτηριστικού με αναζήτηση. Έχει [`CalculationType`](../calculationtype/) ίσο με Lookup και μπορεί να χρησιμοποιηθεί μόνο σε Resources. Απαιτείται να καθορίσετε *fieldId* και *alias* όταν καλείτε αυτή τη μέθοδο. Ο τύπος του πεδίου προκύπτει από το field id.

```csharp
public static ExtendedAttributeDefinition CreateLookupResourceDefinition(
    ExtendedAttributeResource fieldId, string alias)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fieldId | ExtendedAttributeResource | Το καθορισμένο πεδίο ID του [`ExtendedAttributeResource`](../../extendedattributeresource/). |
| alias | String | Το καθορισμένο ψευδώνυμο τύπου String. |

### Τιμή Επιστροφής

Δημιουργήθηκε ένα στιγμιότυπο της κλάσης [`ExtendedAttributeDefinition`](../) με καθορισμένο *fieldId* και *alias*.

## Παραδείγματα

Χρησιμοποιήστε αυτό το παράδειγμα για να δημιουργήσετε έναν ορισμό προσαρμοσμένου πεδίου για έναν πόρο με αναζήτηση και στη συνέχεια να το γεμίσετε με τιμές κειμένου:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateLookupResourceDefinition(ExtendedAttributeResource.Text27, "My custom field");
resourceTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
resourceTextAttr.AddLookupValue(new Value { Id = 2, Val = "Text value 2", Description = "Text value description 2" });
project.ExtendedAttributes.Add(resourceTextAttr);
```

Δείχνει πώς να γράψετε ενημερωμένους ορισμούς επεκταμένων χαρακτηριστικών.

```csharp
var project = new Project(DataDir + "WriteUpdatedExtendedAttributeDefinitions.mpp");

// Προσθέστε νέο επεκταμένο χαρακτηριστικό text3 με αναζήτηση και μία τιμή αναζήτησης
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

// Προσθέστε νέο επεκταμένο χαρακτηριστικό cost1 με αναζήτηση και δύο τιμές κόστους
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

// Προσθέστε νέα εργασία και εκχωρήστε τιμή αναζήτησης χαρακτηριστικού.
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

// Ορίστε χαρακτηριστικό διάρκειας χωρίς αναζήτηση.
var taskDurationAttributeDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Duration1, "New Duration");
project.ExtendedAttributes.Add(taskDurationAttributeDefinition);

// Προσθέστε νέα εργασία και εκχωρήστε τιμή διάρκειας στο προηγουμένως ορισμένο χαρακτηριστικό διάρκειας.
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

### Δείτε επίσης

* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateLookupResourceDefinition(CustomFieldType, ExtendedAttributeResource, string) {#createlookupresourcedefinition}

Μέθοδος κατασκευής που δημιουργεί έναν ορισμό εκτεταμένου χαρακτηριστικού με αναζήτηση. Έχει [`CalculationType`](../calculationtype/) ίσο με Lookup και μπορεί να χρησιμοποιηθεί μόνο σε Resources. Απαιτείται να καθορίσετε *customFieldType*, *fieldId* και *alias* όταν καλείτε αυτή τη μέθοδο.

```csharp
public static ExtendedAttributeDefinition CreateLookupResourceDefinition(
    CustomFieldType customFieldType, ExtendedAttributeResource fieldId, string alias)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| customFieldType | CustomFieldType | Ο καθορισμένος τύπος του [`CustomFieldType`](../../customfieldtype/). |
| fieldId | ExtendedAttributeResource | Το καθορισμένο πεδίο ID του [`ExtendedAttributeResource`](../../extendedattributeresource/). |
| alias | String | Το καθορισμένο ψευδώνυμο τύπου String. |

### Τιμή Επιστροφής

Δημιουργήθηκε ένα στιγμιότυπο της κλάσης [`ExtendedAttributeDefinition`](../) με καθορισμένο *customFieldType*, *fieldId* και *alias*.

## Παραδείγματα

Χρησιμοποιήστε αυτό το παράδειγμα για να δημιουργήσετε έναν ορισμό προσαρμοσμένου πεδίου για έναν πόρο με αναζήτηση και στη συνέχεια να το γεμίσετε με τιμές κειμένου:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateLookupResourceDefinition(CustomFieldType.Text, ExtendedAttributeResource.Text27, "My custom field");
resourceTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
resourceTextAttr.AddLookupValue(new Value { Id = 2, Val = "Text value 2", Description = "Text value description 2" });
project.ExtendedAttributes.Add(resourceTextAttr);
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

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


