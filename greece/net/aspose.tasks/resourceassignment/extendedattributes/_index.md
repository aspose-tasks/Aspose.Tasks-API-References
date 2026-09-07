---
title: "ResourceAssignment.ExtendedAttributes"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα ResourceAssignment. Λαμβάνει ή ορίζει μια παρουσία της κλάσης ExtendedAttributeCollection για αυτό το αντικείμενο."
type: docs
weight: 250
url: /el/net/aspose.tasks/resourceassignment/extendedattributes/
---
## ResourceAssignment.ExtendedAttributes property

Λαμβάνει ή ορίζει μια παρουσία της κλάσης ExtendedAttributeCollection για αυτό το αντικείμενο.

```csharp
public ExtendedAttributeCollection ExtendedAttributes { get; set; }
```

## Παρατηρήσεις

Η ανάγνωση υποστηρίζεται μόνο για μορφή XML.

## Παραδείγματα

Δείχνει πώς να προσθέσετε εκτεταμένα χαρακτηριστικά για μια ανάθεση.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// Αναθέστε τον πόρο "1 TRG: Trade Group" στο "TASK 1" δημιουργώντας ένα αντικείμενο ResourceAssignment.
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Resource");
var assignment = project.ResourceAssignments.Add(task, resource);

// Δημιουργήστε ορισμό προσαρμοσμένου χαρακτηριστικού με αναζήτηση.
var definition = ExtendedAttributeDefinition.CreateLookupResourceDefinition(CustomFieldType.Cost, ExtendedAttributeResource.Cost5, "My lookup resource cost");
project.ExtendedAttributes.Add(definition);

var firstValue = new Value { NumericValue = 1500, Description = "Val 1", Id = 1, Val = "1500" };
var secondValue = new Value { NumericValue = 2500, Description = "Val 2", Id = 2 };
definition.AddLookupValue(firstValue);
definition.AddLookupValue(secondValue);

// Αυτή η τιμή μπορεί να εμφανιστεί στην προβολή "Resource usage" του MS Project.
var attributeValue = definition.CreateExtendedAttribute(firstValue);
assignment.ExtendedAttributes.Add(attributeValue);

Console.WriteLine("Number of assignment's extended attribute: " + assignment.ExtendedAttributes.Count);
foreach (var attribute in assignment.ExtendedAttributes)
{
    Console.WriteLine("Extended attribute alias: " + attribute.AttributeDefinition.Alias);
}
```

### Δείτε επίσης

* class [ExtendedAttributeCollection](../../extendedattributecollection/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


