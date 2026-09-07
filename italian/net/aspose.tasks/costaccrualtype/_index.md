---
title: "Enum CostAccrualType"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Aspose.Tasks.CostAccrualType enum. Specifica il tipo di costo di accantonamento."
type: docs
weight: 350
url: /it/net/aspose.tasks/costaccrualtype/
---
## CostAccrualType enumeration

Specifica il tipo di costo di accumulo.

```csharp
public enum CostAccrualType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Undefined | `-1` | Indica che il valore non definito significa che il campo non era definito nel file di progetto originale. |
| Start | `0` | Indica il tipo di accantonamento del costo di avvio. |
| Prorated | `1` | Indica il tipo di accantonamento del costo proporzionale. |
| End | `2` | Indica il tipo di accantonamento del costo di fine. |
| Invalid | `3` | Indica un tipo di accantonamento del costo non valido. |

## Osservazioni

Durante l'esportazione in XML i valori Undefined verranno eliminati dall'XML risultante.

## Esempi

Mostra come e quando i costi standard e gli straordinari delle risorse devono essere addebitati o accantonati (metodo di accantonamento: determina quando il costo per una risorsa è sostenuto e quando i costi effettivi sono addebitati a un progetto. È possibile sostenere i costi all'inizio [Start] o alla fine [End] di un'attività o proporzionarli [Prorated] durante l'attività.), al costo di un'attività (CostAccrualType.End).

```csharp
var project = new Project(DataDir + "Project2.mpp");
var resource = project.Resources.GetById(1);
// imposta tipo di accantonamento del costo
// se selezioni l'opzione End, i costi non vengono accantonati finché il lavoro rimanente non è zero.
resource.Set(Rsc.AccrueAt, CostAccrualType.End);
// lavorare con il progetto...
```

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


