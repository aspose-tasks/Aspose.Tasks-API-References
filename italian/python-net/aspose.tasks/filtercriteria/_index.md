---
title: "FilterCriteria"
second_title: "Riferimento API di Aspose.Tasks per Python via .NET"
description: 
type: docs
weight: 350
url: /it/python-net/aspose.tasks/filtercriteria/
---

## FilterCriteria class

Definisce i criteri che attività o risorse devono soddisfare per essere visualizzati nella vista MSP.

Il tipo FilterCriteria espone i seguenti membri:
## Costruttori
| Nome | Descrizione |
| :- | :- |
| FilterCriteria() | Inizializza una nuova istanza della classe FilterCriteria |
## Proprietà
| Nome | Descrizione |
| :- | :- |
| operazione | Ottiene o imposta il criterio stabilito con FieldName, Test e Value che si riferisce ad altri criteri nel filtro. |
| field | Ottiene o imposta un [field](/tasks/python-net/aspose.tasks/filtercriteria/) da modificare. |
| test | Ottiene o imposta il tipo di confronto effettuato tra FieldName e Value che funge da criterio di selezione per il filtro.<br/>            [FilterComparisonType](/tasks/python-net/aspose.tasks/filtercomparisontype/) |
| values | Ottiene i valori degli oggetti da confrontare con il valore del campo specificato con FieldName. |
| criteria_rows | Ottiene l'elenco delle righe figlio [FilterCriteria](/tasks/python-net/aspose.tasks/filtercriteria/).<br/>            Se il filtro contiene più di una riga di criterio, l'effetto dell'operatore And è che i criteri per entrambe le righe devono essere soddisfatti affinché l'attività o la risorsa venga visualizzata come risultato di questo filtro.<br/>            L'effetto dell'operatore Or è che i criteri per una delle due righe devono essere soddisfatti. |
## Methods
| Nome | Descrizione |
| :- | :- |
| is_field_value() | Ottiene se il valore a destra di FilterCriteria è un riferimento a un campo, non un valore costante. |
| set_value_field(value) | Imposta il campo il cui valore sarà confrontato con il valore del campo specificato da FieldName. |

### Vedi anche

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

