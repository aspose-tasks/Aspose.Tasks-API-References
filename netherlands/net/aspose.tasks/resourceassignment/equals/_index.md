---
title: "ResourceAssignment.Equals"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ResourceAssignment-methode. Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven instantie van de ResourceAssignment-klasse"
type: docs
weight: 690
url: /nl/net/aspose.tasks/resourceassignment/equals/
---
## Equals(ResourceAssignment) {#equals}

Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven instantie van de [`ResourceAssignment`](../) klasse.

```csharp
public bool Equals(ResourceAssignment other)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| other | ResourceAssignment | De opgegeven instantie van de [`ResourceAssignment`](../) klasse om te vergelijken met deze instantie. |

### Retourwaarde

**True** if the specified instance of the [`ResourceAssignment`](../) class has the same UID value as this instance; otherwise, **false**.

## Voorbeelden

Toont hoe de gelijkheid van resource‑toewijzingen gecontroleerd kan worden.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");

var resourceAssignment1 = project.ResourceAssignments.GetByUid(1);
var resourceAssignment2 = project.ResourceAssignments.GetByUid(1);

Console.WriteLine("Are resource assignments equal: " + resourceAssignment1.Equals(resourceAssignment2));
```

### Zie ook

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
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

**True** if o is a ResourceAssignment that assign the same resource and task as this instance; otherwise, **false**.

## Voorbeelden

Toont hoe de gelijkheid van resource‑toewijzingen gecontroleerd kan worden.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");

var resourceAssignment1 = project.ResourceAssignments.GetByUid(1);
var resourceAssignment2 = project.ResourceAssignments.GetByUid(1);

Console.WriteLine("Are resource assignments equal: " + resourceAssignment1.Equals(resourceAssignment2));
```

### Zie ook

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


