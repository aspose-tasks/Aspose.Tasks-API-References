---
title: Class Metered
second_title: Aspose.Tasks för .NET API-referens
description: Aspose.Tasks.Metered klass. Tillhandahåller metoder för att ställa in mätnyckel.
type: docs
weight: 890
url: /sv/net/aspose.tasks/metered/
---
## Metered class

Tillhandahåller metoder för att ställa in mätnyckel.

```csharp
public class Metered
```

## Konstruktörer

| namn | Beskrivning |
| --- | --- |
| [Metered](metered/)() | Default_Constructor |

## Metoder

| namn | Beskrivning |
| --- | --- |
| [ResetMeteredKey](../../aspose.tasks/metered/resetmeteredkey/)() | Tar bort tidigare installationslicens. |
| [SetMeteredKey](../../aspose.tasks/metered/setmeteredkey/)(string, string) | Ställer in mätta offentliga och privata nycklar. |
| static [GetConsumptionCredit](../../aspose.tasks/metered/getconsumptioncredit/)() | Får konsumtionskredit. |
| static [GetConsumptionQuantity](../../aspose.tasks/metered/getconsumptionquantity/)() | Får förbrukningsfilstorlek. |

### Exempel

I det här exemplet kommer ett försök att göras att ställa in mätt offentlig och privat nyckel

```csharp
[C#]

Metered metered = new Metered();
metered.SetMeteredKey("PublicKey", "PrivateKey");


[Visual Basic]

Dim metered As Metered = New Metered
metered.SetMeteredKey("PublicKey", "PrivateKey")
```

komponentjarfilen:

```csharp
Metered metered = new Metered();
metered.setMeteredKey("PublicKey", "PrivateKey");
```

### Se även

* namnutrymme [Aspose.Tasks](../../aspose.tasks/)
* hopsättning [Aspose.Tasks](../../)


