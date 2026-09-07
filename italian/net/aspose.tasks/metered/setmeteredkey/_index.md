---
title: "Metered.SetMeteredKey"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo Metered. Imposta le chiavi pubbliche e private metered"
type: docs
weight: 40
url: /it/net/aspose.tasks/metered/setmeteredkey/
---
## Metered.SetMeteredKey method

Imposta le chiavi pubbliche e private metered.

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| publicKey | Stringa | La chiave pubblica. |
| privateKey | Stringa | La chiave privata. |

## Osservazioni

Se acquisti una licenza a consumo, questa API dovrebbe essere chiamata all'avvio dell'applicazione; normalmente è sufficiente. Tuttavia, se il meccanismo a consumo non riesce a caricare i dati di consumo durante un periodo di 24 ore, la licenza verrà impostata allo stato di valutazione. Per evitare tale caso, dovresti controllare regolarmente lo stato della licenza; se è in stato di valutazione, chiama nuovamente questa API.

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


