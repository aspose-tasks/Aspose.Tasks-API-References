---
title: "Project.GetWork"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo del progetto. Ottiene l'oggetto Duration con il valore Double specificato e il formato di lavoro predefinito"
type: docs
weight: 1130
url: /it/net/aspose.tasks/project/getwork/
---
## Project.GetWork method

Ottiene l'oggetto [`Duration`](../../duration/) con il valore Double specificato e il formato di lavoro predefinito.

```csharp
public Duration GetWork(double val)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| val | Double | valore double specificato. |

### Valore di ritorno

Oggetto Duration.

## Osservazioni

Questo metodo dovrebbe essere usato con cautela perché restituisce durate diverse a seconda dell'impostazione Project.WorkFormat. Per esempio, GetWork(1.0) restituirà 1 ora quando Project.WorkFormat è TimeUnitType.Hour o 1 giorno se Project.WorkFormat è TimeUnitType.Day.

## Esempi

Mostra come ottenere un lavoro con il formato di lavoro predefinito.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

Console.WriteLine("Project's work format: " + project.Get(Prj.WorkFormat));

// crea un valore di lavoro con il formato di lavoro predefinito del progetto
var work = project.GetWork(2);
Console.WriteLine("Work: " + work.TimeSpan);
Console.WriteLine("Time unit: " + work.TimeUnit);
```

### Vedi anche

* struct [Duration](../../duration/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


