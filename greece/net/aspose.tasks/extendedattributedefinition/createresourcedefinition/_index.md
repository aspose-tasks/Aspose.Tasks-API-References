---
title: "ExtendedAttributeDefinition.CreateResourceDefinition"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος ExtendedAttributeDefinition. Μέθοδος κατασκευής που δημιουργεί έναν απλό ορισμό εκτεταμένης ιδιότητας που το Microsoft Project εμφανίζει ως None. Έχει CalculationType ίσο με None και μπορεί να χρησιμοποιηθεί μόνο σε Resource. Απαιτείται να καθορίσετε τα πεδία customFieldType, fieldId και alias όταν καλείτε αυτή τη μέθοδο."
type: docs
weight: 30
url: /el/net/aspose.tasks/extendedattributedefinition/createresourcedefinition/
---
## CreateResourceDefinition(CustomFieldType, ExtendedAttributeResource, string) {#createresourcedefinition}

Μέθοδος κατασκευής που δημιουργεί έναν απλό ορισμό εκτεταμένης ιδιότητας, ο οποίος εμφανίζεται στο Microsoft Project ως "None". Έχει [`CalculationType`](../calculationtype/) ίσο με None και μπορεί να χρησιμοποιηθεί μόνο σε Resource. Απαιτείται να καθορίσετε *customFieldType*, *fieldId* και *alias* όταν καλείτε αυτή τη μέθοδο.

```csharp
public static ExtendedAttributeDefinition CreateResourceDefinition(CustomFieldType customFieldType, 
    ExtendedAttributeResource fieldId, string alias)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| customFieldType | CustomFieldType | Ο καθορισμένος τύπος του [`CustomFieldType`](../../customfieldtype/). |
| fieldId | ExtendedAttributeResource | Το καθορισμένο πεδίο ID του [`ExtendedAttributeResource`](../../extendedattributeresource/). |
| alias | String | Το καθορισμένο ψευδώνυμο τύπου String. |

### Τιμή Επιστροφής

Δημιουργήθηκε ένα στιγμιότυπο της κλάσης [`ExtendedAttributeDefinition`](../) με καθορισμένο *customFieldType*, *fieldId* και *alias*.

## Παραδείγματα

Χρησιμοποιήστε αυτό το παράδειγμα για να δημιουργήσετε έναν ορισμό προσαρμοσμένου πεδίου κειμένου:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateResourceDefinition(CustomFieldType.Text, ExtendedAttributeResource.Text27, "My custom field");
project.ExtendedAttributes.Add(resourceTextAttr);
```

Δείχνει πώς να προσθέσετε εκτεταμένη ιδιότητα σε μια ανάθεση πόρου.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// Προσθήκη νέας εργασίας και πόρου
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Rsc");
var assignment = project.ResourceAssignments.Add(task, resource);
{
    // Προσαρμοσμένες ιδιότητες που είναι ορατές στην προβολή "Resource Usage" μπορούν να δημιουργηθούν με τη μέθοδο ExtendedAttributeDefinition.CreateResourceDefinition.
    var resCostAttributeDefinition = ExtendedAttributeDefinition.CreateResourceDefinition(
        CustomFieldType.Cost,
        ExtendedAttributeResource.Cost5,
        "My cost");

    project.ExtendedAttributes.Add(resCostAttributeDefinition);

    var value = resCostAttributeDefinition.CreateExtendedAttribute();

    // Ο τύπος της ιδιότητας είναι "Cost", επομένως πρέπει να χρησιμοποιήσουμε την ιδιότητα "NumericValue".
    value.NumericValue = 1500;

    assignment.ExtendedAttributes.Add(value);
}

{
    // Προσαρμοσμένες ιδιότητες που είναι ορατές στην προβολή "Task Usage" μπορούν να δημιουργηθούν με τη μέθοδο ExtendedAttributeDefinition.CreateTaskDefinition.
    var taskCostAttributeDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(
        CustomFieldType.Cost,
        ExtendedAttributeTask.Cost5,
        "My cost for task");

    project.ExtendedAttributes.Add(taskCostAttributeDefinition);

    var value = taskCostAttributeDefinition.CreateExtendedAttribute();

    // Ο τύπος της ιδιότητας είναι "Cost", επομένως πρέπει να χρησιμοποιήσουμε την ιδιότητα "NumericValue".
    value.NumericValue = 2300;

    assignment.ExtendedAttributes.Add(value);
}

project.Save(OutDir + "AddExtendedAttributesToResourceAssignment_out.mpp", SaveFileFormat.Mpp);
```

### Δείτε επίσης

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateResourceDefinition(ExtendedAttributeResource, string) {#createresourcedefinition_1}

Μέθοδος κατασκευής που δημιουργεί έναν απλό ορισμό εκτεταμένης ιδιότητας, ο οποίος εμφανίζεται στο Microsoft Project ως "None". Έχει [`CalculationType`](../calculationtype/) ίσο με None και μπορεί να χρησιμοποιηθεί μόνο σε Resource. Απαιτείται να καθορίσετε *fieldId* και *alias* όταν καλείτε αυτή τη μέθοδο. Ο τύπος του πεδίου προκύπτει από το fieldId.

```csharp
public static ExtendedAttributeDefinition CreateResourceDefinition(
    ExtendedAttributeResource fieldId, string alias)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fieldId | ExtendedAttributeResource | Το καθορισμένο πεδίο ID του [`ExtendedAttributeResource`](../../extendedattributeresource/). |
| alias | String | Το καθορισμένο ψευδώνυμο τύπου String. |

### Τιμή Επιστροφής

Δημιουργήθηκε ένα στιγμιότυπο της κλάσης [`ExtendedAttributeDefinition`](../) με καθορισμένο *fieldId* και *alias*.

## Παραδείγματα

Χρησιμοποιήστε αυτό το παράδειγμα για να δημιουργήσετε έναν ορισμό προσαρμοσμένου πεδίου κειμένου:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateResourceDefinition(ExtendedAttributeResource.Text27, "My custom field");
project.ExtendedAttributes.Add(resourceTextAttr);
```

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

* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


