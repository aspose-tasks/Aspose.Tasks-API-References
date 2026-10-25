---
title: "Classe Metered"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Aspose.Tasks.Metered classe. Fornisce metodi per impostare la chiave metered"
type: docs
weight: 1020
url: /it/net/aspose.tasks/metered/
---
## Metered class

Fornisce metodi per impostare la chiave a consumo.

```csharp
public class Metered
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [Metered](metered/)() | Il costruttore predefinito. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [IsLicensed](../../aspose.tasks/metered/islicensed/)() | Verifica se il prodotto è stato licenziato correttamente utilizzando una licenza Metered. |
| [ResetMeteredKey](../../aspose.tasks/metered/resetmeteredkey/)() | Rimuove la licenza precedentemente configurata. |
| [SetMeteredKey](../../aspose.tasks/metered/setmeteredkey/)(string, string) | Imposta le chiavi pubbliche e private metered. |
| static [GetConsumptionCredit](../../aspose.tasks/metered/getconsumptioncredit/)() | Ottiene il credito di consumo. |
| static [GetConsumptionQuantity](../../aspose.tasks/metered/getconsumptionquantity/)() | Ottiene la dimensione del file di consumo. |

## Esempi

In questo esempio, verrà tentato di impostare la chiave pubblica e privata metered

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

Mostra come utilizzare il tipo di licenza &lt;see cref="Aspose.Tasks.Metered" /&gt; con Aspose.Tasks.

```csharp
// Utilizziamo la licenza a consumo (vedi https://purchase.aspose.com/faqs/licensing/metered)
// imposta licenza a consumo
var metered = new Metered();
metered.SetMeteredKey("<public key>", "<private key>");

var project = new Project(DataDir + "Project2.mpp");
Console.WriteLine("Project Name: " + project.Get(Prj.Name));

// ...
// lavorare con il progetto...
// ...

// Possiamo ottenere i crediti attuali e il consumo di byte.

try
{
    Console.WriteLine("Credits spent: {0}", Metered.GetConsumptionCredit());
    Console.WriteLine("Bytes consumed: {0}", Metered.GetConsumptionQuantity());
}
catch (WebException)
{
    // log eccezione
}

// di recente l'utente può reimpostare una licenza a consumo e interrompere il conteggio dei byte
metered.ResetMeteredKey();
```

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


