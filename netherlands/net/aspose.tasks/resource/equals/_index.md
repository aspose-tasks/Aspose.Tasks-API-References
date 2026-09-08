---
title: "Resource.Equals"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Resource-methode. Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven instantie van de Resource-klasse."
type: docs
weight: 820
url: /nl/net/aspose.tasks/resource/equals/
---
## Equals(Resource) {#equals}

Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven instantie van de [`Resource`](../) klasse.

```csharp
public bool Equals(Resource other)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| other | Resource | De opgegeven instantie van de [`Resource`](../) klasse om te vergelijken met deze instantie. |

### Retourwaarde

**True** if the specified instance of the [`Resource`](../) class has the same Uid value as this instance; otherwise, **false**.

## Voorbeelden

Toont hoe resource-gelijkheid gecontroleerd kan worden.

```csharp
var project = new Project(DataDir + "Baselines2010.mpp");

var resource1 = project.Resources.GetById(1);
var resource2 = project.Resources.GetById(1);

Console.WriteLine("Are resources equal: " + resource1.Equals(resource2));
```

### Zie ook

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object.

```csharp
public override bool Equals(object obj)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| obj | Object | Het object om te vergelijken met deze instantie. |

### Retourwaarde

**True** if the specified object is a Resource that has the same Uid value as this instance; otherwise, **false**.

## Voorbeelden

Toont hoe resource-gelijkheid gecontroleerd kan worden.

```csharp
var project = new Project(DataDir + "Baselines2010.mpp");

var resource1 = project.Resources.GetById(1);
var resource2 = project.Resources.GetById(1);

Console.WriteLine("Are resources equal: " + resource1.Equals(resource2));
```

### Zie ook

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


