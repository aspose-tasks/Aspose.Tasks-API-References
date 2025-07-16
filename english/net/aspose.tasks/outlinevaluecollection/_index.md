---
title: Class OutlineValueCollection
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.OutlineValueCollection class. Represents a collection of OutlineValue objects
type: docs
weight: 1200
url: /net/aspose.tasks/outlinevaluecollection/
---
## OutlineValueCollection class

Represents a collection of [`OutlineValue`](../outlinevalue/) objects.

```csharp
public class OutlineValueCollection : IList<OutlineValue>
```

## Properties

| Name | Description |
| --- | --- |
| [Count](../../aspose.tasks/outlinevaluecollection/count/) { get; } | Gets the number of elements contained in this collection. |
| [IsReadOnly](../../aspose.tasks/outlinevaluecollection/isreadonly/) { get; } | Gets a value indicating whether this collection is read-only. |
| [Item](../../aspose.tasks/outlinevaluecollection/item/) { get; set; } | Returns or sets the element at the specified index. |

## Methods

| Name | Description |
| --- | --- |
| [Add](../../aspose.tasks/outlinevaluecollection/add/)(OutlineValue) | Adds the specified item to this collection. |
| [Clear](../../aspose.tasks/outlinevaluecollection/clear/)() | Removes all items from this collection. |
| [Contains](../../aspose.tasks/outlinevaluecollection/contains/)(OutlineValue) | Returns true if the specified item is found in this collection; otherwise, false. |
| [CopyTo](../../aspose.tasks/outlinevaluecollection/copyto/)(OutlineValue[], int) | Copies the elements of this collection to the specified array, starting at the specified array index. |
| [GetEnumerator](../../aspose.tasks/outlinevaluecollection/getenumerator/)() | Returns an enumerator for this collection. |
| [IndexOf](../../aspose.tasks/outlinevaluecollection/indexof/)(OutlineValue) | Determines the index of the specified item in this collection. |
| [Insert](../../aspose.tasks/outlinevaluecollection/insert/)(int, OutlineValue) | Inserts the specified item at the specified index. |
| [Remove](../../aspose.tasks/outlinevaluecollection/remove/)(OutlineValue) | Removes the first occurrence of a specific object from this collection. |
| [RemoveAt](../../aspose.tasks/outlinevaluecollection/removeat/)(int) | Removes an item at the specified index. |

## Examples

Shows how to work with outline value collections.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

// clear value collections
foreach (var outlineCode in project.OutlineCodes)
{
    // clear outline masks
    if (outlineCode.Values.Count <= 0)
    {
        continue;
    }

    if (!outlineCode.Values.IsReadOnly)
    {
        outlineCode.Values.Clear();
    }
}

var codeDefinition = new OutlineCodeDefinition
                         {
                             Alias = "New task outline code1", FieldId = ((int)ExtendedAttributeTask.OutlineCode1).ToString(), FieldName = "Outline Code1"
                         };
var value = new OutlineValue { Description = "Value description", ValueId = 1, Value = "123456", Type = OutlineValueType.Number };
codeDefinition.Values.Add(value);
project.OutlineCodes.Add(codeDefinition);

// update value by index access
codeDefinition.Values[0].Value = "654321";

// iterate over outline values
foreach (var definitionValue in codeDefinition.Values)
{
    Console.WriteLine("Value: " + definitionValue.Value);
    Console.WriteLine("Value Id: " + definitionValue.ValueId);
    Console.WriteLine("Value Guid: " + definitionValue.ValueGuid);
    Console.WriteLine();
}

// ...
// work with outline values
// ...

// remove a value when needed
if (codeDefinition.Values.Contains(value))
{
    codeDefinition.Values.Remove(value);
}

// insert a value in the start position
codeDefinition.Values.Insert(0, value);

// check the position of inserted value
Console.WriteLine("Index of inserted value: " + codeDefinition.Values.IndexOf(value));

// ...
// work with outline values
// ...

// remove the last value from the collection
codeDefinition.Values.RemoveAt(codeDefinition.Values.Count - 1);

// one can create the another outline code definition
var codeDefinition2 = new OutlineCodeDefinition
                          {
                              Alias = "New outline code 2", FieldId = ((int)ExtendedAttributeTask.OutlineCode2).ToString(), FieldName = "Outline Code2"
                          };

// and then copy outline values
var outlineValues = new OutlineValue[codeDefinition.Values.Count];
codeDefinition.Values.CopyTo(outlineValues, 0);

foreach (var outlineValue in outlineValues)
{
    codeDefinition2.Values.Add(outlineValue);
}
```

### See Also

* class [OutlineValue](../outlinevalue/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


