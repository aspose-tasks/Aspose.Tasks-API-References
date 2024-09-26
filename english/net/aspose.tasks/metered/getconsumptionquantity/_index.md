---
title: Metered.GetConsumptionQuantity
second_title: Aspose.Tasks for .NET API Reference
description: Metered method. Gets consumption file size
type: docs
weight: 60
url: /net/aspose.tasks/metered/getconsumptionquantity/
---
## Metered.GetConsumptionQuantity method

Gets consumption file size.

```csharp
public static decimal GetConsumptionQuantity()
```

### Return Value

Returns the number of consumed bytes.

## Examples

Shows how to use &lt;see cref="Aspose.Tasks.Metered" /&gt; license type with Aspose.Tasks.

```csharp
// Let's use metered license (see https://purchase.aspose.com/faqs/licensing/metered)
// set metered licence
var metered = new Metered();
metered.SetMeteredKey("<public key>", "<private key>");

var project = new Project(DataDir + "Project2.mpp");
Console.WriteLine("Project Name: " + project.Get(Prj.Name));

// ...
// work with project...
// ...

// We can get current credits and bytes consumption.

try
{
    Console.WriteLine("Credits spent: {0}", Metered.GetConsumptionCredit());
    Console.WriteLine("Bytes consumed: {0}", Metered.GetConsumptionQuantity());
}
catch (WebException)
{
    // log exception
}

// lately the user can reset a metered and stop counting of bytes
metered.ResetMeteredKey();
```

### See Also

* class [Metered](../)
* namespace [Aspose.Tasks](../../metered/)
* assembly [Aspose.Tasks](../../../)


