---
title: "Duration.Equals"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode Duration. Renvoie une valeur indiquant si cette instance est égale à un objet spécifié."
type: docs
weight: 80
url: /fr/net/aspose.tasks/duration/equals/
---
## Equals(Duration) {#equals}

Renvoie une valeur indiquant si cette instance est égale à un objet spécifié.

```csharp
public bool Equals(Duration other)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| autre | Duration | L'objet à comparer avec cette instance. |

### Valeur de retour

Renvoie **True** si l'autre instance Duration possède les mêmes valeurs TimeSpan et TimeUnit que cette instance ; sinon, **false**.

## Exemples

Montre comment vérifier l'égalité des durées.

```csharp
var project = new Project();

var duration1 = project.GetDuration(1, TimeUnitType.Day);
var duration2 = project.GetDuration(1, TimeUnitType.Day);
var duration3 = project.GetDuration(1, TimeUnitType.Hour);

// l'égalité de la durée est vérifiée par rapport au timespan sous-jacent
Console.WriteLine("Duration 1: " + duration1.TimeSpan);
Console.WriteLine("Duration 2: " + duration2.TimeSpan);
Console.WriteLine("Duration 3: " + duration3.TimeSpan);
Console.WriteLine("Are durations 1 and 2 equal: " + duration1.Equals(duration2));
Console.WriteLine("Are durations 1 and 3 equal: " + duration1.Equals(duration3));
```

### Voir aussi

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

Renvoie une valeur indiquant si cette instance est égale à un objet spécifié.

```csharp
public override bool Equals(object obj)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| obj | Objet | L'objet à comparer avec cette instance. |

### Valeur de retour

**True** if the specified object is a Duration that has the same TimeSpan and TimeUnit values as this instance; otherwise, **false**.

## Exemples

Montre comment vérifier l'égalité des durées.

```csharp
var project = new Project();

var duration1 = project.GetDuration(1, TimeUnitType.Day);
var duration2 = project.GetDuration(1, TimeUnitType.Day);
var duration3 = project.GetDuration(1, TimeUnitType.Hour);

// l'égalité de la durée est vérifiée par rapport au timespan sous-jacent
Console.WriteLine("Duration 1: " + duration1.TimeSpan);
Console.WriteLine("Duration 2: " + duration2.TimeSpan);
Console.WriteLine("Duration 3: " + duration3.TimeSpan);
Console.WriteLine("Are durations 1 and 2 equal: " + duration1.Equals(duration2));
Console.WriteLine("Are durations 1 and 3 equal: " + duration1.Equals(duration3));
```

### Voir aussi

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


