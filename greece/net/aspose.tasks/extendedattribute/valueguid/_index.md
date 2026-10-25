---
title: "ExtendedAttribute.ValueGuid"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα ExtendedAttribute. Λαμβάνει το guid μιας τιμής αναζήτησης."
type: docs
weight: 90
url: /el/net/aspose.tasks/extendedattribute/valueguid/
---
## ExtendedAttribute.ValueGuid property

Λαμβάνει το guid μιας τιμής αναζήτησης.

```csharp
public string ValueGuid { get; }
```

## Παρατηρήσεις

Δεν πρέπει να οριστεί άμεσα· αντίθετα, χρησιμοποιήστε ExtendedAttributeDefinition.CreateExtendedAttribute(Value lookupValue) για να δημιουργήσετε ένα εκτεταμένο χαρακτηριστικό με μια τιμή αναζήτησης.

## Παραδείγματα

Δείχνει πώς να εργαστείτε με ένα GUID εκτεταμένου χαρακτηριστικού.

```csharp
var project = new Project();
var definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(CustomFieldType.Cost, ExtendedAttributeTask.Cost1, "My lookup cost");
var finished = project.RootTask.Children.Add("Task");
finished.Set(Tsk.Start, new DateTime(2020, 4, 21, 8, 0, 0));
finished.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
finished.Set(Tsk.Finish, new DateTime(2020, 4, 21, 17, 0, 0));

var value1 = new Value { NumericValue = 10000, Description = "Val 1", Id = 1 };
var value2 = new Value { NumericValue = 25000, Description = "Val 2", Id = 2 };

definition.AddLookupValue(value1);
definition.AddLookupValue(value2);

var attribute = definition.CreateExtendedAttribute(value1);

// Το εκτεταμένο χαρακτηριστικό έχει ένα GUID το οποίο είναι 
// ίσο με το GUID του δεσμού 'Value' από την αναζήτηση.
Console.WriteLine("Extended attribute GUID: " + attribute.ValueGuid);
Console.WriteLine("GUID of the first value in the lookup: " + value1.ValueGuid.ToString().ToUpper());
var guidFromString = Guid.Parse(attribute.ValueGuid);
Console.WriteLine("Are these GUIDs equal: " + guidFromString.Equals(value1.ValueGuid));
```

### Δείτε επίσης

* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


