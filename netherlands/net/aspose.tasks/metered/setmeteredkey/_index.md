---
title: "Metered.SetMeteredKey"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Metered-methode. Stelt de openbare en privé-sleutels voor Metered in"
type: docs
weight: 40
url: /nl/net/aspose.tasks/metered/setmeteredkey/
---
## Metered.SetMeteredKey method

Stelt metered publieke en private sleutels in.

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| publicKey | String | De openbare sleutel. |
| privateKey | String | De privésleutel. |

## Opmerkingen

Als u een metered‑licentie aanschaft, moet deze API bij het opstarten van de applicatie worden aangeroepen; normaal is dit voldoende. Als de metered‑licentie echter faalt bij het uploaden van consumptiegegevens gedurende een periode van 24 uur, wordt de licentie ingesteld op evaluatiestatus. Om zo’n geval te voorkomen, moet u regelmatig de licentiestatus controleren. Als deze evaluatiestatus is, roept u deze API opnieuw aan.

## Voorbeelden

Toont hoe &lt;see cref=\"Aspose.Tasks.Metered\" /&gt; licentietype met Aspose.Tasks.

```csharp
// Laten we een meterlicentie gebruiken (see https://purchase.aspose.com/faqs/licensing/metered)
// stel meterlicentie in
var metered = new Metered();
metered.SetMeteredKey("<public key>", "<private key>");

var project = new Project(DataDir + "Project2.mpp");
Console.WriteLine("Project Name: " + project.Get(Prj.Name));

// ...
// werken met project...
// ...

// We kunnen de huidige credits en het byteverbruik ophalen.

try
{
    Console.WriteLine("Credits spent: {0}", Metered.GetConsumptionCredit());
    Console.WriteLine("Bytes consumed: {0}", Metered.GetConsumptionQuantity());
}
catch (WebException)
{
    // log uitzondering
}

// recentelijk kan de gebruiker een meterlicentie resetten en het tellen van bytes stoppen
metered.ResetMeteredKey();
```

### Zie ook

* class [Metered](../)
* namespace [Aspose.Tasks](../../metered/)
* assembly [Aspose.Tasks](../../../)


