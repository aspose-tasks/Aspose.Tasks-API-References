---
title: "Task.ExtendedAttributes"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα Task. Λαμβάνει το αντικείμενο ExtendedAttributeCollection που περιέχει τις τιμές μιας επεκταμένης ιδιότητας"
type: docs
weight: 400
url: /el/net/aspose.tasks/task/extendedattributes/
---
## Task.ExtendedAttributes property

Λαμβάνει το αντικείμενο ExtendedAttributeCollection που περιέχει τις τιμές μιας εκτεταμένης ιδιότητας.

```csharp
public ExtendedAttributeCollection ExtendedAttributes { get; }
```

## Παρατηρήσεις

Απαιτούνται δύο κομμάτια δεδομένων - ένας δείκτης πίσω στον πίνακα εκτεταμένων χαρακτηριστικών που καθορίζεται είτε από το μοναδικό ID είτε από το Field ID, και η τιμή που καθορίζεται είτε με την τιμή, είτε με έναν δείκτη πίσω στη λίστα τιμών.

## Παραδείγματα

Δείχνει πώς να διαβάσετε τις επεκταμένες ιδιότητες του έργου.

```csharp
var project = new Project(DataDir + "ReadTaskExtendedAttributes.mpp");

// Δημιουργήστε τον ορισμό εκτεταμένου χαρακτηριστικού
var definition = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Start, ExtendedAttributeTask.Start7, "Start 7");
project.ExtendedAttributes.Add(definition);

// Λάβετε εργασία με δείκτη μηδέν
var tsk = project.RootTask.Children.GetById(1);

// Προσθέστε εκτεταμένο χαρακτηριστικό
var extendedAttribute = definition.CreateExtendedAttribute();
extendedAttribute.DateValue = DateTime.Now;

// Επίσης μπορεί να χρησιμοποιηθεί η ακόλουθη σύντομη σύνταξη: ExtendedAttribute attribute = attributeDefinition.CreateExtendedAttribute(DateTime.Now);
tsk.ExtendedAttributes.Add(extendedAttribute);

// Δημιουργήστε έναν ορισμό εκτεταμένης ιδιότητας τύπου Text1
var taskExtendedAttributeText1Definition =
    ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text1, "Task City Name");

// Προσθέστε το στη συλλογή Εκτεταμένων Ιδιοτήτων του έργου
project.ExtendedAttributes.Add(taskExtendedAttributeText1Definition);

var newTask = project.RootTask.Children.Add("Task 1");

// Δημιουργήστε μια εκτεταμένη ιδιότητα από τον ορισμό ιδιότητας
var taskExtendedAttributeText1 = taskExtendedAttributeText1Definition.CreateExtendedAttribute();

// Αναθέστε μια τιμή στην παραγόμενη εκτεταμένη ιδιότητα. Ο τύπος της ιδιότητας είναι "Text", πρέπει να χρησιμοποιηθεί η ιδιότητα "TextValue".
taskExtendedAttributeText1.TextValue = "London";

// Προσθέστε την εκτεταμένη ιδιότητα στην εργασία
newTask.ExtendedAttributes.Add(taskExtendedAttributeText1);

// Δημιουργήστε έναν ορισμό εκτεταμένης ιδιότητας τύπου Text2
var taskExtendedAttributeText2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Text,
    ExtendedAttributeTask.Text2,
    "Task Towns Name");

// Προσθέστε τιμές αναζήτησης για τον ορισμό εκτεταμένου χαρακτηριστικού
taskExtendedAttributeText2Definition.AddLookupValue(new Value { Id = 1, StringValue = "Town1", Description = "This is Town1" });
taskExtendedAttributeText2Definition.AddLookupValue(new Value { Id = 2, StringValue = "Town2", Description = "This is Town2" });

// Προσθέστε το στη συλλογή Εκτεταμένων Ιδιοτήτων του έργου
project.ExtendedAttributes.Add(taskExtendedAttributeText2Definition);

var task2 = project.RootTask.Children.Add("Task 2");

// Δημιουργήστε μια εκτεταμένη ιδιότητα από τον ορισμό αναζήτησης Text2 για το Id 1
var taskExtendedAttributeText2 = taskExtendedAttributeText2Definition.CreateExtendedAttribute(taskExtendedAttributeText2Definition.ValueList[1]);

// Προσθέστε την εκτεταμένη ιδιότητα στην εργασία
task2.ExtendedAttributes.Add(taskExtendedAttributeText2);

// Δημιουργήστε έναν ορισμό εκτεταμένης ιδιότητας τύπου Duration2
var taskExtendedAttributeDuration2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Duration,
    ExtendedAttributeTask.Duration2,
    "Some duration");

// Προσθέστε τιμές αναζήτησης για τον ορισμό εκτεταμένης ιδιότητας
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 3, Duration = project.GetDuration(4, TimeUnitType.Hour), Description = "4 hours" });
taskExtendedAttributeDuration2Definition.AddLookupValue(new Value { Id = 4, Duration = project.GetDuration(1, TimeUnitType.Day), Description = "1 day" });
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 5, Duration = project.GetDuration(1, TimeUnitType.Hour), Description = "1 hour" });
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 6, Duration = project.GetDuration(10, TimeUnitType.Day), Description = "10 days" });

// Προσθέστε τον ορισμό στη συλλογή Εκτεταμένων Ιδιοτήτων του έργου
project.ExtendedAttributes.Add(taskExtendedAttributeDuration2Definition);

var task3 = project.RootTask.Children.Add("Task 3");

// Δημιουργήστε μια εκτεταμένη ιδιότητα από τον ορισμό αναζήτησης Duration2 για το Id 3
var taskExtendedAttributeDuration2 =
    taskExtendedAttributeDuration2Definition.CreateExtendedAttribute(taskExtendedAttributeDuration2Definition.ValueList[3]);

// Προσθέστε την εκτεταμένη ιδιότητα στην εργασία
task3.ExtendedAttributes.Add(taskExtendedAttributeDuration2);

// Δημιουργήστε έναν ορισμό εκτεταμένης ιδιότητας τύπου Finish2
var taskExtendedAttributeFinish2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Finish,
    ExtendedAttributeTask.Finish2,
    "Some finish");

// Προσθέστε τιμές αναζήτησης για τον ορισμό εκτεταμένης ιδιότητας
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 7, DateTimeValue = new DateTime(1984, 01, 01, 00, 00, 01), Description = "This is Value2" });
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 8, DateTimeValue = new DateTime(1994, 01, 01, 00, 01, 01), Description = "This is Value3" });
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 9, DateTimeValue = new DateTime(2009, 12, 31, 00, 00, 00), Description = "This is Value4" });
taskExtendedAttributeFinish2Definition.AddLookupValue(new Value { Id = 10, DateTimeValue = DateTime.Now, Description = "This is Value6" });

// Προσθέστε τον ορισμό στη συλλογή Εκτεταμένων Ιδιοτήτων του έργου
project.ExtendedAttributes.Add(taskExtendedAttributeFinish2Definition);

var task4 = project.RootTask.Children.Add("Task 4");

// Δημιουργήστε μια εκτεταμένη ιδιότητα από τον ορισμό αναζήτησης Finish2 για το Id 3
var taskExtendedAttributeFinish2 = taskExtendedAttributeFinish2Definition.CreateExtendedAttribute(taskExtendedAttributeFinish2Definition.ValueList[3]);

// Προσθέστε την εκτεταμένη ιδιότητα στην εργασία
task4.ExtendedAttributes.Add(taskExtendedAttributeFinish2);

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Ανάγνωση εκτεταμένων χαρακτηριστικών για εργασίες
foreach (var task in collector.Tasks)
{
    foreach (var attribute in task.ExtendedAttributes)
    {
        Console.WriteLine(attribute.FieldId);
        Console.WriteLine(attribute.ValueGuid);

        switch (attribute.AttributeDefinition.CfType)
        {
            case CustomFieldType.Date:
            case CustomFieldType.Start:
            case CustomFieldType.Finish:
                Console.WriteLine(attribute.DateValue);
                break;
            case CustomFieldType.Text:
                Console.WriteLine(attribute.TextValue);
                break;
            case CustomFieldType.Duration:
                Console.WriteLine(attribute.DurationValue.ToString());
                break;
            case CustomFieldType.Cost:
            case CustomFieldType.Number:
                Console.WriteLine(attribute.NumericValue);
                break;
            case CustomFieldType.Flag:
                Console.WriteLine(attribute.FlagValue);
                break;
            case CustomFieldType.Null:
            case CustomFieldType.RBS:
            case CustomFieldType.OutlineCode:
                return;
            default:
                return;
        }
    }
}

project.Save(OutDir + "ReadWriteTaskExtendedAttributes_out.mpp", SaveFileFormat.Mpp);
```

### Δείτε επίσης

* class [ExtendedAttributeCollection](../../extendedattributecollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


