---
title: "ExtendedAttributeDefinition.CreateTaskDefinition"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "ExtendedAttributeDefinition method. Μέθοδος κατασκευής που δημιουργεί έναν απλό ορισμό εκτεταμένου χαρακτηριστικού που το Microsoft Project εμφανίζει ως None. Έχει CalculationType ίσο με None και μπορεί να χρησιμοποιηθεί μόνο σε Tasks. Απαιτείται να καθορίσετε customFieldType, fieldId και alias όταν καλείτε αυτή τη μέθοδο"
type: docs
weight: 40
url: /el/net/aspose.tasks/extendedattributedefinition/createtaskdefinition/
---
## CreateTaskDefinition(CustomFieldType, ExtendedAttributeTask, string) {#createtaskdefinition}

Μέθοδος κατασκευής που δημιουργεί έναν απλό ορισμό εκτεταμένου χαρακτηριστικού, που το Microsoft Project εμφανίζει ως "None". Έχει [`CalculationType`](../calculationtype/) ίσο με None και μπορεί να χρησιμοποιηθεί μόνο σε Tasks. Απαιτείται να καθορίσετε *customFieldType*, *fieldId* και *alias* όταν καλείτε αυτή τη μέθοδο.

```csharp
public static ExtendedAttributeDefinition CreateTaskDefinition(CustomFieldType customFieldType, 
    ExtendedAttributeTask fieldId, string alias)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| customFieldType | CustomFieldType | Ο καθορισμένος τύπος του [`CustomFieldType`](../../customfieldtype/). |
| fieldId | ExtendedAttributeTask | Το καθορισμένο πεδίο ID του [`ExtendedAttributeTask`](../../extendedattributetask/). |
| alias | String | Το καθορισμένο ψευδώνυμο τύπου String. |

### Τιμή Επιστροφής

Δημιουργήθηκε ένα στιγμιότυπο της κλάσης [`ExtendedAttributeDefinition`](../) με καθορισμένο *customFieldType*, *fieldId* και *alias*.

## Παραδείγματα

Χρησιμοποιήστε αυτό το παράδειγμα για να δημιουργήσετε έναν ορισμό προσαρμοσμένου πεδίου κειμένου:

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text27, "My custom field");
project.ExtendedAttributes.Add(taskTextAttr);
```

Δείχνει πώς να δημιουργήσετε τις εκτεταμένες ιδιότητες της εργασίας.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// Δημιουργήστε έναν ορισμό εκτεταμένης ιδιότητας τύπου Text1
var taskExtendedAttributeText1Definition =
    ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text1, "Task City Name");

// Προσθέστε το στη συλλογή Εκτεταμένων Ιδιοτήτων του έργου
project.ExtendedAttributes.Add(taskExtendedAttributeText1Definition);

// Προσθέστε μια εργασία στο έργο
var task = project.RootTask.Children.Add("Task 1");

// Δημιουργήστε μια εκτεταμένη ιδιότητα από τον ορισμό ιδιότητας
var taskExtendedAttributeText1 = taskExtendedAttributeText1Definition.CreateExtendedAttribute();

// Αναθέστε μια τιμή στην παραγόμενη εκτεταμένη ιδιότητα. Ο τύπος της ιδιότητας είναι "Text", πρέπει να χρησιμοποιηθεί η ιδιότητα "TextValue".
taskExtendedAttributeText1.TextValue = "London";

// Προσθέστε την εκτεταμένη ιδιότητα στην εργασία
task.ExtendedAttributes.Add(taskExtendedAttributeText1);

project.Save(OutDir + "PlainTextExtendedAttribute_out.mpp", SaveFileFormat.Mpp);

var project4 = new Project(DataDir + "Blank2010.mpp");

// Δημιουργήστε έναν ορισμό εκτεταμένης ιδιότητας τύπου Text2
var taskExtendedAttributeText2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Text,
    ExtendedAttributeTask.Text2,
    "Task Towns Name");

// Προσθέστε τιμές αναζήτησης για τον ορισμό εκτεταμένου χαρακτηριστικού
taskExtendedAttributeText2Definition.AddLookupValue(new Value { Id = 1, StringValue = "Town1", Description = "This is Town1" });
taskExtendedAttributeText2Definition.AddLookupValue(new Value { Id = 2, StringValue = "Town2", Description = "This is Town2" });

// Προσθέστε το στη συλλογή Εκτεταμένων Ιδιοτήτων του έργου
project4.ExtendedAttributes.Add(taskExtendedAttributeText2Definition);

// Προσθέστε μια εργασία στο έργο
var task2 = project4.RootTask.Children.Add("Task 2");

// Δημιουργήστε μια εκτεταμένη ιδιότητα από τον ορισμό αναζήτησης Text2 για το Id 1
var taskExtendedAttributeText2 = taskExtendedAttributeText2Definition.CreateExtendedAttribute(taskExtendedAttributeText2Definition.ValueList[1]);

// Προσθέστε την εκτεταμένη ιδιότητα στην εργασία
task2.ExtendedAttributes.Add(taskExtendedAttributeText2);

project4.Save(OutDir + "TextExtendedAttributeWithLookup_out.mpp", SaveFileFormat.Mpp);

var project2 = new Project(DataDir + "Blank2010.mpp");

// Δημιουργήστε έναν ορισμό εκτεταμένης ιδιότητας τύπου Duration2
var taskExtendedAttributeDuration2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Duration,
    ExtendedAttributeTask.Duration2,
    "Some duration");

// Προσθέστε τιμές αναζήτησης για τον ορισμό εκτεταμένης ιδιότητας
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 2, Duration = project2.GetDuration(4, TimeUnitType.Hour), Description = "4 hours" });
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 3, Duration = project2.GetDuration(1, TimeUnitType.Day), Description = "1 day" });
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 4, Duration = project2.GetDuration(1, TimeUnitType.Hour), Description = "1 hour" });
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 7, Duration = project2.GetDuration(10, TimeUnitType.Day), Description = "10 days" });

// Προσθέστε τον ορισμό στη συλλογή Εκτεταμένων Ιδιοτήτων του έργου
project2.ExtendedAttributes.Add(taskExtendedAttributeDuration2Definition);

// Προσθέστε μια εργασία στο έργο
var task3 = project2.RootTask.Children.Add("Task 3");

// Δημιουργήστε μια εκτεταμένη ιδιότητα από τον ορισμό αναζήτησης Duration2 για το Id 3
var taskExtendedAttributeDuration2 =
    taskExtendedAttributeDuration2Definition.CreateExtendedAttribute(taskExtendedAttributeDuration2Definition.ValueList[3]);

// Προσθέστε την εκτεταμένη ιδιότητα στην εργασία
task3.ExtendedAttributes.Add(taskExtendedAttributeDuration2);

project2.Save(OutDir + "DurationExtendedAttributeWithLookup_out.mpp", SaveFileFormat.Mpp);

var project3 = new Project(DataDir + "Blank2010.mpp");

// Δημιουργήστε έναν ορισμό εκτεταμένης ιδιότητας τύπου Finish2
var taskExtendedAttributeFinish2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Finish,
    ExtendedAttributeTask.Finish2,
    "Some finish");

// Προσθέστε τιμές αναζήτησης για τον ορισμό εκτεταμένης ιδιότητας
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 2, DateTimeValue = new DateTime(1984, 01, 01, 00, 00, 01), Description = "This is Value2" });
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 3, DateTimeValue = new DateTime(1994, 01, 01, 00, 01, 01), Description = "This is Value3" });
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 4, DateTimeValue = new DateTime(2009, 12, 31, 00, 00, 00), Description = "This is Value4" });
taskExtendedAttributeFinish2Definition.AddLookupValue(new Value { Id = 7, DateTimeValue = DateTime.Now, Description = "This is Value6" });

// Προσθέστε τον ορισμό στη συλλογή Εκτεταμένων Ιδιοτήτων του έργου
project3.ExtendedAttributes.Add(taskExtendedAttributeFinish2Definition);

// Προσθέστε μια εργασία στο έργο
var task4 = project3.RootTask.Children.Add("Task 4");

// Δημιουργήστε μια εκτεταμένη ιδιότητα από τον ορισμό αναζήτησης Finish2 για το Id 3
var taskExtendedAttributeFinish2 = taskExtendedAttributeFinish2Definition.CreateExtendedAttribute(taskExtendedAttributeFinish2Definition.ValueList[3]);

// Προσθέστε την εκτεταμένη ιδιότητα στην εργασία
task4.ExtendedAttributes.Add(taskExtendedAttributeFinish2);

project3.Save(OutDir + "FinishExtendedAttributeWithLookup_out.mpp", SaveFileFormat.Mpp);
```

### Δείτε επίσης

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateTaskDefinition(ExtendedAttributeTask, string) {#createtaskdefinition_1}

Μέθοδος κατασκευής που δημιουργεί έναν απλό ορισμό εκτεταμένης ιδιότητας, ο οποίος εμφανίζεται στο Microsoft Project ως "None". Διαθέτει το [`CalculationType`](../calculationtype/) ίσο με None και μπορεί να χρησιμοποιηθεί μόνο σε Εργασίες. Απαιτείται να καθορίσετε *fieldId* και *alias* κατά την κλήση αυτής της μεθόδου. Ο τύπος του πεδίου προκύπτει από το πεδίο ID.

```csharp
public static ExtendedAttributeDefinition CreateTaskDefinition(ExtendedAttributeTask fieldId, 
    string alias)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fieldId | ExtendedAttributeTask | Το καθορισμένο πεδίο ID του [`ExtendedAttributeTask`](../../extendedattributetask/). |
| alias | String | Το καθορισμένο ψευδώνυμο τύπου String. |

### Τιμή Επιστροφής

Δημιουργήθηκε ένα στιγμιότυπο της κλάσης [`ExtendedAttributeDefinition`](../) με καθορισμένο *fieldId* και *alias*.

## Παραδείγματα

Χρησιμοποιήστε αυτό το παράδειγμα για να δημιουργήσετε έναν ορισμό προσαρμοσμένου πεδίου κειμένου:

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text27, "My custom field");
project.ExtendedAttributes.Add(taskTextAttr);
```

Δείχνει πώς να δημιουργήσετε ορισμό εκτεταμένου χαρακτηριστικού και να ορίσετε μια τιμή συμβολοσειράς για το χαρακτηριστικό κατά τη δημιουργία του.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, "My Text");
project.ExtendedAttributes.Add(definition);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 22, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// δημιουργήστε εκτεταμένο χαρακτηριστικό με τιμή ίση με το 'Common Info'
var extendedAttribute = definition.CreateExtendedAttribute("Common Info");

// προσθέστε εκτεταμένο χαρακτηριστικό που αρχικοποιείται με την τιμή 'Common Info'
task.ExtendedAttributes.Add(extendedAttribute);
```

### Δείτε επίσης

* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


