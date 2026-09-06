---
title: "Project.GetDuration"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode Project. Obtient un objet Duration avec le nombre spécifié d'unités et le format de durée par défaut qui est défini dans les paramètres du projet DurationFormat"
type: docs
weight: 1100
url: /fr/net/aspose.tasks/project/getduration/
---
## GetDuration(double) {#getduration}

Obtient l'objet [`Duration`](../../duration/) avec le nombre spécifié d'unités et le format de durée par défaut qui est défini dans les paramètres du projet [`DurationFormat`](../../prj/durationformat/).

```csharp
public Duration GetDuration(double val)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| val | Double | nombre d'unités spécifié. |

### Valeur de retour

Objet Duration.

## Remarques

Cette méthode doit être utilisée avec précaution car elle renvoie des durées différentes selon le paramètre Project.DurationFormat. Par exemple, GetWork(1.0) renverra 1 heure lorsque Project.DurationFormat est TimeUnitType.Hour ou 1 jour si Project.DurationFormat est TimeUnitType.Day.

## Exemples

Montre comment créer une instance &lt;see cref=\"Aspose.Tasks.Duration\" /&gt; avec le format de durée par défaut du projet en utilisant les méthodes de fabrication du projet.

```csharp
var project = new Project();

// obtenir une durée avec le format de projet par défaut.
var duration = project.GetDuration(1);

Console.WriteLine("Default project duration time unit type: " + project.Get(Prj.DurationFormat));
Console.WriteLine("Created duration time unit type: " + duration.TimeUnit);
```

### Voir aussi

* struct [Duration](../../duration/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetDuration(double, TimeUnitType) {#getduration_1}

Obtient l'objet [`Duration`](../../duration/) avec le nombre spécifié d'unités [`TimeUnitType`](../../timeunittype/).

```csharp
public Duration GetDuration(double val, TimeUnitType timeUnit)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| val | Double | nombre d'unités spécifié. |
| timeUnit | TimeUnitType | valeur TimeUnitType spécifiée. |

### Valeur de retour

Objet Duration.

## Exemples

Montre comment créer une instance &lt;see cref=\"Aspose.Tasks.Duration\" /&gt; en utilisant les méthodes de fabrication du projet.

```csharp
var project = new Project();

// obtenir une durée avec le format de projet par défaut.
var duration = project.GetDuration(1, TimeUnitType.Minute);

Console.WriteLine("Created duration: " + duration);
```

### Voir aussi

* struct [Duration](../../duration/)
* enum [TimeUnitType](../../timeunittype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetDuration(TimeSpan, TimeUnitType) {#getduration_2}

Obtient l'objet [`Duration`](../../duration/) avec la valeur TimeSpan spécifiée et la valeur [`TimeUnitType`](../../timeunittype/) spécifiée.

```csharp
public Duration GetDuration(TimeSpan timeSpan, TimeUnitType timeUnit)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| timeSpan | TimeSpan | valeur TimeSpan spécifiée. |
| timeUnit | TimeUnitType | valeur TimeUnitType spécifiée. |

### Valeur de retour

Objet Duration.

### Voir aussi

* struct [Duration](../../duration/)
* enum [TimeUnitType](../../timeunittype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


