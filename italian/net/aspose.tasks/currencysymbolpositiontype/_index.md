---
title: "Enum CurrencySymbolPositionType"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Enum Aspose.Tasks.CurrencySymbolPositionType. Specifica la posizione di un simbolo di valuta."
type: docs
weight: 370
url: /it/net/aspose.tasks/currencysymbolpositiontype/
---
## CurrencySymbolPositionType enumeration

Specifica la posizione del simbolo di valuta.

```csharp
public enum CurrencySymbolPositionType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Undefined | `-1` | Indica che il valore non definito significa che il campo non era definito nel file di progetto originale. |
| Before | `0` | Indica il tipo di posizione del simbolo di valuta Before. |
| After | `1` | Indica il tipo di posizione del simbolo di valuta After. |
| BeforeWithSpace | `2` | Indica il tipo di posizione del simbolo di valuta BeforeWithSpace. |
| AfterWithSpace | `3` | Indica il tipo di posizione del simbolo di valuta AfterWithSpace. |

## Osservazioni

Durante l'esportazione in XML i valori Undefined verranno eliminati dall'XML risultante.

## Esempi

Mostra come specificare la posizione del simbolo di valuta (CurrencySymbolPositionType.Before).

```csharp
var project = new Project(DataDir + "Project2.mpp");
// imposta la posizione del simbolo di valuta
// Before, senza spazio ($0).
project.Set(Prj.CurrencySymbolPosition, CurrencySymbolPositionType.Before);
// lavorare con il progetto...
```

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


