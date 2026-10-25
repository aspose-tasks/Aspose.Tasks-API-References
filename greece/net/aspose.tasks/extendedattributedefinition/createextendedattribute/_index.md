---
title: "ExtendedAttributeDefinition.CreateExtendedAttribute"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος ExtendedAttributeDefinition. Δημιουργεί ένα νέο εκτεταμένο χαρακτηριστικό με το ID πεδίου που ισούται με την τιμή του ID πεδίου αυτού του αντικειμένου"
type: docs
weight: 310
url: /el/net/aspose.tasks/extendedattributedefinition/createextendedattribute/
---
## CreateExtendedAttribute() {#createextendedattribute}

Δημιουργεί ένα νέο εκτεταμένο χαρακτηριστικό με το αναγνωριστικό πεδίου που ισούται με την τιμή του αναγνωριστικού πεδίου αυτού του αντικειμένου.

```csharp
public ExtendedAttribute CreateExtendedAttribute()
```

### Τιμή Επιστροφής

επιστρέφει τη δημιουργημένη παρουσία της κλάσης [`ExtendedAttribute`](../../extendedattribute/) με το fieldID που ισούται με το fieldID αυτού του αντικειμένου.

## Παραδείγματα

Δείχνει πώς να δημιουργήσετε εκτεταμένα χαρακτηριστικά.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var definition = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Text1);

// Εάν το προσαρμοσμένο πεδίο δεν υπάρχει στο Project, δημιουργήστε το
if (definition == null)
{
    definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, "My text field");
    project.ExtendedAttributes.Add(definition);
}

// Δημιουργία εκτεταμένου χαρακτηριστικού από τον ορισμό
var attribute = definition.CreateExtendedAttribute();
attribute.TextValue = "Text attribute value";

// Προσθήκη εκτεταμένου χαρακτηριστικού στην εργασία
var task = project.RootTask.Children.Add("Task 1");
task.ExtendedAttributes.Add(attribute);

project.Save(OutDir + "CreateExtendedAttributes_out.mpp", SaveFileFormat.Mpp);
```

### Δείτε επίσης

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(string) {#createextendedattribute_6}

Δημιουργεί ένα νέο εκτεταμένο χαρακτηριστικό με το αναγνωριστικό πεδίου που ισούται με την τιμή του αναγνωριστικού πεδίου αυτού του αντικειμένου και με την καθορισμένη τιμή κειμένου.

```csharp
public ExtendedAttribute CreateExtendedAttribute(string textValue)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| textValue | String | Η καθορισμένη τιμή κειμένου. |

### Τιμή Επιστροφής

επιστρέφει τη δημιουργημένη παρουσία της κλάσης [`ExtendedAttribute`](../../extendedattribute/) με το fieldID που ισούται με το fieldID αυτού του αντικειμένου.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| InvalidOperationException | Εάν ο τρέχων [`CfType`](../cftype/) δεν είναι 'Text' |

## Παραδείγματα

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

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(decimal) {#createextendedattribute_5}

Δημιουργεί ένα νέο εκτεταμένο χαρακτηριστικό με το αναγνωριστικό πεδίου που ισούται με την τιμή του αναγνωριστικού πεδίου αυτού του αντικειμένου και με την καθορισμένη αριθμητική τιμή.

```csharp
public ExtendedAttribute CreateExtendedAttribute(decimal numericValue)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| numericValue | Decimal | Η καθορισμένη αριθμητική τιμή. |

### Τιμή Επιστροφής

επιστρέφει τη δημιουργημένη παρουσία της κλάσης [`ExtendedAttribute`](../../extendedattribute/) με το fieldID που ισούται με το fieldID αυτού του αντικειμένου.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| InvalidOperationException | Εάν ο τρέχων [`CfType`](../cftype/) δεν είναι 'Number' ή 'Cost' |

## Παραδείγματα

Δείχνει πώς να δημιουργήσετε ορισμό εκτεταμένου χαρακτηριστικού και να ορίσετε μια δεκαδική τιμή για το χαρακτηριστικό κατά τη δημιουργία του.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Cost1, "My Cost");
project.ExtendedAttributes.Add(definition);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 22, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// δημιουργήστε εκτεταμένο χαρακτηριστικό με τιμή ίση με 999m
var extendedAttribute = definition.CreateExtendedAttribute(999m);

// προσθέστε εκτεταμένο χαρακτηριστικό που αρχικοποιείται με τιμή 999m
task.ExtendedAttributes.Add(extendedAttribute);
```

### Δείτε επίσης

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(DateTime) {#createextendedattribute_4}

Δημιουργεί ένα νέο εκτεταμένο χαρακτηριστικό με το αναγνωριστικό πεδίου που ισούται με την τιμή του αναγνωριστικού πεδίου αυτού του αντικειμένου και με την καθορισμένη τιμή ημερομηνίας.

```csharp
public ExtendedAttribute CreateExtendedAttribute(DateTime dateTimeValue)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| dateTimeValue | DateTime | Η καθορισμένη τιμή ημερομηνίας και ώρας. |

### Τιμή Επιστροφής

επιστρέφει τη δημιουργημένη παρουσία της κλάσης [`ExtendedAttribute`](../../extendedattribute/) με το fieldID που ισούται με το fieldID αυτού του αντικειμένου.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| InvalidOperationException | Εάν ο τρέχων [`CfType`](../cftype/) δεν είναι 'Date', 'Start' ή 'Finish' |

## Παραδείγματα

Δείχνει πώς να δημιουργήσετε ορισμό εκτεταμένου χαρακτηριστικού και να ορίσετε μια τιμή ημερομηνίας/ώρας του χαρακτηριστικού κατά τη δημιουργία του.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var definitionWithDate = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Date1, "My Date");
project.ExtendedAttributes.Add(definitionWithDate);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 22, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// Δημιουργήστε εκτεταμένο χαρακτηριστικό με τιμή ίση με DateTime.Now
var extendedAttribute = definitionWithDate.CreateExtendedAttribute(DateTime.Now);

// Προσθέστε εκτεταμένο χαρακτηριστικό
task.ExtendedAttributes.Add(extendedAttribute);
```

### Δείτε επίσης

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(Duration) {#createextendedattribute_1}

Δημιουργεί ένα νέο εκτεταμένο χαρακτηριστικό με το αναγνωριστικό πεδίου που ισούται με την τιμή του αναγνωριστικού πεδίου αυτού του αντικειμένου και με την καθορισμένη τιμή διάρκειας.

```csharp
public ExtendedAttribute CreateExtendedAttribute(Duration durationValue)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| durationValue | Διάρκεια | Η καθορισμένη τιμή διάρκειας. |

### Τιμή Επιστροφής

επιστρέφει τη δημιουργημένη παρουσία της κλάσης [`ExtendedAttribute`](../../extendedattribute/) με το fieldID που ισούται με το fieldID αυτού του αντικειμένου.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| InvalidOperationException | Εάν ο τρέχων [`CfType`](../cftype/) δεν είναι 'Duration' |

## Παραδείγματα

Δείχνει πώς να δημιουργήσετε ορισμό εκτεταμένου χαρακτηριστικού και να ορίσετε μια διάρκεια κατά τη δημιουργία του.

```csharp
var project = new Project(DataDir + "Project2.mpp");
var task = project.RootTask.Children.Add("Test");
task.Set(Tsk.Start, new DateTime(2020, 4, 22, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Duration1, "Custom Duration");
project.ExtendedAttributes.Add(definition);

// εκτεταμένο χαρακτηριστικό Duration1 = 2 ημέρες
var extendedAttribute = definition.CreateExtendedAttribute(project.GetDuration(2, TimeUnitType.Day));

// προσθέστε εκτεταμένο χαρακτηριστικό στην εργασία
task.ExtendedAttributes.Add(extendedAttribute);
```

### Δείτε επίσης

* class [ExtendedAttribute](../../extendedattribute/)
* struct [Duration](../../duration/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(bool) {#createextendedattribute_3}

Δημιουργεί ένα νέο εκτεταμένο χαρακτηριστικό με το αναγνωριστικό πεδίου που ισούται με την τιμή του αναγνωριστικού πεδίου αυτού του αντικειμένου και με την καθορισμένη τιμή σημαίας.

```csharp
public ExtendedAttribute CreateExtendedAttribute(bool flagValue)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| flagValue | Boolean | Η καθορισμένη τιμή σημαίας. |

### Τιμή Επιστροφής

επιστρέφει τη δημιουργημένη παρουσία της κλάσης [`ExtendedAttribute`](../../extendedattribute/) με το fieldID που ισούται με το fieldID αυτού του αντικειμένου.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| InvalidOperationException | Εάν ο τρέχων [`CfType`](../cftype/) δεν είναι 'Flag' |

## Παραδείγματα

Δείχνει πώς να δημιουργήσετε ορισμό εκτεταμένου χαρακτηριστικού και να ορίσετε μια τιμή σημαίας κατά τη δημιουργία του.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var resource = project.Resources.Add("Resource 1");
resource.Set(Rsc.Type, ResourceType.Cost);

// δημιουργήστε έναν ορισμό για ένα λογικό προσαρμοσμένο πεδίο
var definition = ExtendedAttributeDefinition.CreateResourceDefinition(ExtendedAttributeResource.Flag7, "My Custom Flag");

// δημιουργήστε ένα χαρακτηριστικό και ορίστε την αρχική τιμή σε 'true'
var attribute = definition.CreateExtendedAttribute(true);
resource.ExtendedAttributes.Add(attribute);
```

### Δείτε επίσης

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(Value) {#createextendedattribute_2}

Δημιουργεί νέο εκτεταμένο χαρακτηριστικό συνδεδεμένο με το καθορισμένο στοιχείο [`Value`](../../value/).

```csharp
public ExtendedAttribute CreateExtendedAttribute(Value lookupValue)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| lookupValue | Value | Το καθορισμένο στοιχείο [`Value`](../../value/). |

### Τιμή Επιστροφής

επιστρέφει τη δημιουργημένη παρουσία της κλάσης [`ExtendedAttribute`](../../extendedattribute/) που είναι συνδεδεμένη με το καθορισμένο στοιχείο [`Value`](../../value/).

## Παρατηρήσεις

*lookupValue* should be previously added to the [`ExtendedAttributeDefinition`](../) using [`AddLookupValue`](../addlookupvalue/) method.

## Παραδείγματα

Χρησιμοποιήστε αυτόν τον κώδικα για να δημιουργήσετε νέο [`ExtendedAttribute`](../../extendedattribute/) χρησιμοποιώντας συγκεκριμένη τιμή:

```csharp
taskTextAttr.AddLookupValue(value1);
taskTextAttr.AddLookupValue(value2);
var extendedAttribute = taskTextAttr.CreateExtendedAttribute(value2);
```

Δείχνει πώς να δημιουργήσετε ορισμό εκτεταμένου χαρακτηριστικού και να ορίσετε μια τιμή κατά τη δημιουργία του.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// Δημιουργήστε ορισμό προσαρμοσμένου πεδίου βάσει του πίνακα αναζήτησης, ο οποίος δηλώθηκε παραπάνω.
var customFieldDefinition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(CustomFieldType.Number, ExtendedAttributeTask.Number10, "Status");

var value1 = new Value { Id = 1, Val = "25", Description = "Active" };
var value2 = new Value { Id = 2, Val = "12", Description = "Inactive" };
customFieldDefinition.AddLookupValue(value1);
customFieldDefinition.AddLookupValue(value2);
project.ExtendedAttributes.Add(customFieldDefinition);

var task = project.RootTask.Children.Add("Task");

// Δημιουργήστε εκτεταμένο χαρακτηριστικό για μια τιμή
var extendedAttribute = customFieldDefinition.CreateExtendedAttribute(value2);

// προσθέστε εκτεταμένο χαρακτηριστικό στην εργασία
task.ExtendedAttributes.Add(extendedAttribute);
```

### Δείτε επίσης

* class [ExtendedAttribute](../../extendedattribute/)
* class [Value](../../value/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


