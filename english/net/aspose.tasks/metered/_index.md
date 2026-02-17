---
title: Class Metered
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Metered class. Provides methods to set metered key
type: docs
weight: 1010
url: /net/aspose.tasks/metered/
---
## Metered class

Provides methods to set metered key.

```csharp
public class Metered
```

## Constructors

| Name | Description |
| --- | --- |
| [Metered](metered/)() | The default constructor. |

## Methods

| Name | Description |
| --- | --- |
| [IsLicensed](../../aspose.tasks/metered/islicensed/)() | Checks whether the product is successfully licensed using Metered license. |
| [ResetMeteredKey](../../aspose.tasks/metered/resetmeteredkey/)() | Removes previously setup license. |
| [SetMeteredKey](../../aspose.tasks/metered/setmeteredkey/)(string, string) | Sets metered public and private keys. |
| static [GetConsumptionCredit](../../aspose.tasks/metered/getconsumptioncredit/)() | Gets consumption credit. |
| static [GetConsumptionQuantity](../../aspose.tasks/metered/getconsumptionquantity/)() | Gets consumption file size. |

## Examples

In this example, an attempt will be made to set metered public and private key

```csharp
[C#]

Metered metered = new Metered();
metered.SetMeteredKey("PublicKey", "PrivateKey");


[Visual Basic]

Dim metered As Metered = New Metered
metered.SetMeteredKey("PublicKey", "PrivateKey")
```

the component jar file:

```csharp
Metered metered = new Metered();
metered.setMeteredKey("PublicKey", "PrivateKey");
```

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


