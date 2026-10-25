---
title: "Metered.GetConsumptionQuantity"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Metered methode. Haalt consumptiebestandsgrootte op"
type: docs
weight: 60
url: /nl/net/aspose.tasks/metered/getconsumptionquantity/
---
## Metered.GetConsumptionQuantity method

Haalt de bestandsgrootte van het verbruik op.

```csharp
public static decimal GetConsumptionQuantity()
```

### Retourwaarde

Retourneert het aantal verbruikte bytes.

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


