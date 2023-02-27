---
title: Class Metered
second_title: Riferimento all'API di Aspose.Tasks per .NET
description: Aspose.Tasks.Metered classe. Fornisce metodi per impostare la chiave misurata.
type: docs
weight: 890
url: /it/net/aspose.tasks/metered/
---
## Metered class

Fornisce metodi per impostare la chiave misurata.

```csharp
public class Metered
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [Metered](metered/)() | Default_Costruttore |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [ResetMeteredKey](../../aspose.tasks/metered/resetmeteredkey/)() | Rimuove la licenza precedentemente configurata. |
| [SetMeteredKey](../../aspose.tasks/metered/setmeteredkey/)(string, string) | Imposta chiavi pubbliche e private misurate. |
| static [GetConsumptionCredit](../../aspose.tasks/metered/getconsumptioncredit/)() | Ottiene credito a consumo. |
| static [GetConsumptionQuantity](../../aspose.tasks/metered/getconsumptionquantity/)() | Ottiene la dimensione del file di consumo. |

### Esempi

In questo esempio, verrà effettuato un tentativo di impostare la chiave pubblica e privata misurata

```csharp
[C#]

Metered metered = new Metered();
metered.SetMeteredKey("PublicKey", "PrivateKey");


[Visual Basic]

Dim metered As Metered = New Metered
metered.SetMeteredKey("PublicKey", "PrivateKey")
```

il file jar del componente:

```csharp
Metered metered = new Metered();
metered.setMeteredKey("PublicKey", "PrivateKey");
```

### Guarda anche

* spazio dei nomi [Aspose.Tasks](../../aspose.tasks/)
* assemblea [Aspose.Tasks](../../)


