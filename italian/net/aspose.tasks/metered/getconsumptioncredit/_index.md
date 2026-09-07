---
title: "Metered.GetConsumptionCredit"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo Metered. Ottiene il credito di consumo"
type: docs
weight: 50
url: /it/net/aspose.tasks/metered/getconsumptioncredit/
---
## Metered.GetConsumptionCredit method

Ottiene il credito di consumo.

```csharp
public static decimal GetConsumptionCredit()
```

### Valore di ritorno

Restituisce il numero di punti credito consumati.

## Esempi

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

* class [Metered](../)
* namespace [Aspose.Tasks](../../metered/)
* assembly [Aspose.Tasks](../../../)


