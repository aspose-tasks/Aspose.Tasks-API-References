---
title: Metered.SetMeteredKey
second_title: Aspose.Tasks for .NET API Reference
description: Metered method. Sets metered public and private keys
type: docs
weight: 40
url: /net/aspose.tasks/metered/setmeteredkey/
---
## Metered.SetMeteredKey method

Sets metered public and private keys.

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| Parameter | Type | Description |
| --- | --- | --- |
| publicKey | String | The public key. |
| privateKey | String | The private key. |

## Remarks

If you purchase metered license, this API should be called on application startup, normally, this is enough. However, if metered fails to upload consumption data during 24 hours period, the license will be set to evaluation status. To avoid such case, you should regularly check the license status If it is evaluation status, call this API again.

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


