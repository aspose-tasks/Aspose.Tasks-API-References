---
title: OutlineValueCollection.CopyTo
second_title: Aspose.Tasks for .NET API Reference
description: OutlineValueCollection method. Copies the elements of this collection to the specified array starting at the specified array index
type: docs
weight: 70
url: /net/aspose.tasks/outlinevaluecollection/copyto/
---
## OutlineValueCollection.CopyTo method

Copies the elements of this collection to the specified array, starting at the specified array index.

```csharp
public void CopyTo(OutlineValue[] array, int arrayIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| array | OutlineValue[] | the specified one-dimensional array to copy elements to |
| arrayIndex | Int32 | the zero-based index of the specified array at which copying begins. |

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

* class [OutlineValue](../../outlinevalue/)
* class [OutlineValueCollection](../)
* namespace [Aspose.Tasks](../../outlinevaluecollection/)
* assembly [Aspose.Tasks](../../../)


