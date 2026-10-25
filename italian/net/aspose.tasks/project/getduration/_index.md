---
title: "Project.GetDuration"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo Project. Ottiene un oggetto Duration con il numero specificato di unità e il formato di durata predefinito definito nelle impostazioni del progetto DurationFormat."
type: docs
weight: 1100
url: /it/net/aspose.tasks/project/getduration/
---
## GetDuration(double) {#getduration}

Ottiene l'oggetto [`Duration`](../../duration/) con il numero specificato di unità e il formato di durata predefinito definito nelle impostazioni del progetto [`DurationFormat`](../../prj/durationformat/).

```csharp
public Duration GetDuration(double val)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| val | Double | numero specificato di unità. |

### Valore di ritorno

Oggetto Duration.

## Osservazioni

Questo metodo dovrebbe essere usato con cautela perché restituisce durate diverse a seconda dell'impostazione Project.DurationFormat. Ad esempio, GetWork(1.0) restituirà 1 ora quando Project.DurationFormat è TimeUnitType.Hour o 1 giorno se Project.DurationFormat è TimeUnitType.Day.

## Esempi

Mostra come creare un'istanza &lt;see cref=\"Aspose.Tasks.Duration\" /&gt; con il formato di durata predefinito del progetto utilizzando i metodi di fabbrica del progetto.

```csharp
var project = new Project();

// ottieni una durata con il formato predefinito del progetto.
var duration = project.GetDuration(1);

Console.WriteLine("Default project duration time unit type: " + project.Get(Prj.DurationFormat));
Console.WriteLine("Created duration time unit type: " + duration.TimeUnit);
```

### Vedi anche

* struct [Duration](../../duration/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetDuration(double, TimeUnitType) {#getduration_1}

Ottiene l'oggetto [`Duration`](../../duration/) con il numero specificato di unità [`TimeUnitType`](../../timeunittype/).

```csharp
public Duration GetDuration(double val, TimeUnitType timeUnit)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| val | Double | numero specificato di unità. |
| timeUnit | TimeUnitType | valore TimeUnitType specificato. |

### Valore di ritorno

Oggetto Duration.

## Esempi

Mostra come creare un'istanza &lt;see cref=\"Aspose.Tasks.Duration\" /&gt; utilizzando i metodi di fabbrica del progetto.

```csharp
var project = new Project();

// ottieni una durata con il formato predefinito del progetto.
var duration = project.GetDuration(1, TimeUnitType.Minute);

Console.WriteLine("Created duration: " + duration);
```

### Vedi anche

* struct [Duration](../../duration/)
* enum [TimeUnitType](../../timeunittype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetDuration(TimeSpan, TimeUnitType) {#getduration_2}

Ottiene l'oggetto [`Duration`](../../duration/) con il valore TimeSpan specificato e il valore [`TimeUnitType`](../../timeunittype/) specificato.

```csharp
public Duration GetDuration(TimeSpan timeSpan, TimeUnitType timeUnit)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| timeSpan | TimeSpan | valore TimeSpan specificato. |
| timeUnit | TimeUnitType | valore TimeUnitType specificato. |

### Valore di ritorno

Oggetto Duration.

### Vedi anche

* struct [Duration](../../duration/)
* enum [TimeUnitType](../../timeunittype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


