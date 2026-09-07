---
title: "Classe OutlineCode"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.OutlineCode. Rappresenta un valore di un codice di outline"
type: docs
weight: 1150
url: /it/net/aspose.tasks/outlinecode/
---
## OutlineCode class

Rappresenta un valore di un codice di contorno.

```csharp
public class OutlineCode
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [OutlineCode](outlinecode/#constructor)() | Inizializza una nuova istanza della classe `OutlineCode`. |
| [OutlineCode](outlinecode/#constructor_1)(OutlineCodeDefinition, OutlineValue) | Inizializza una nuova istanza della classe `OutlineCode` utilizzando il codice di outline specificato e uno dei suoi valori. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [FieldId](../../aspose.tasks/outlinecode/fieldid/) { get; set; } | Ottiene o imposta il valore numerico del campo personalizzato Id del progetto. |
| [ValueGuid](../../aspose.tasks/outlinecode/valueguid/) { get; set; } | Ottiene o imposta il GUID del valore nella lista dei valori. Il ValueGuid corrisponde al FieldGuid nella lista dei valori. |
| [ValueId](../../aspose.tasks/outlinecode/valueid/) { get; set; } | Ottiene o imposta l'Id nella lista dei valori associato alla definizione nella collezione di codici di outline. |

## Osservazioni

Sono necessari due dati: un puntatore alla tabella dei codici di outline specificata dal FieldId e il valore specificato sia dal ValueId sia dal puntatore ValueGuid alla lista dei valori.

## Esempi

Mostra come leggere i codici di outline delle attività.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

// leggi i codici di outline
foreach (var task in project.RootTask.SelectAllChildTasks())
{
    if (task.OutlineCodes.Count <= 0)
    {
        continue;
    }

    Console.WriteLine("Print outline codes of the task: " + task.Get(Tsk.Name));
    foreach (var value in task.OutlineCodes)
    {
        Console.WriteLine("  Field Id: " + value.FieldId);
        Console.WriteLine("  Value Guid: " + value.ValueGuid);
        Console.WriteLine("  Value Id: " + value.ValueId);
    }
}
```

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


