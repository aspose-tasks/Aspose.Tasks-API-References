---
title: "Klasse Metered"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Metered klasse. Biedt methoden om de metered-sleutel in te stellen."
type: docs
weight: 1020
url: /nl/net/aspose.tasks/metered/
---
## Metered class

Biedt methoden om een metered‑sleutel in te stellen.

```csharp
public class Metered
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [Metered](metered/)() | De standaardconstructor. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [IsLicensed](../../aspose.tasks/metered/islicensed/)() | Controleert of het product succesvol is gelicenseerd met een Metered-licentie. |
| [ResetMeteredKey](../../aspose.tasks/metered/resetmeteredkey/)() | Verwijdert eerder ingestelde licentie. |
| [SetMeteredKey](../../aspose.tasks/metered/setmeteredkey/)(string, string) | Stelt metered publieke en private sleutels in. |
| static [GetConsumptionCredit](../../aspose.tasks/metered/getconsumptioncredit/)() | Haalt verbruikskrediet op. |
| static [GetConsumptionQuantity](../../aspose.tasks/metered/getconsumptionquantity/)() | Haalt de bestandsgrootte van het verbruik op. |

## Voorbeelden

In dit voorbeeld wordt geprobeerd de metered publieke en private sleutel in te stellen.

```csharp
[C#]

Metered metered = new Metered();
metered.SetMeteredKey("PublicKey", "PrivateKey");


[Visual Basic]

Dim metered As Metered = New Metered
metered.SetMeteredKey("PublicKey", "PrivateKey")
```

het component‑jar‑bestand:

```csharp
Metered metered = new Metered();
metered.setMeteredKey("PublicKey", "PrivateKey");
```

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


