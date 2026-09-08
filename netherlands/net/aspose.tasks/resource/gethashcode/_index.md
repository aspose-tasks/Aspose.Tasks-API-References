---
title: "Resource.GetHashCode"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Resource-methode. Retourneert een hashcode-waarde voor de instantie van de Resource-klasse"
type: docs
weight: 840
url: /nl/net/aspose.tasks/resource/gethashcode/
---
## Resource.GetHashCode method

Retourneert een hashcode-waarde voor de instantie van de [`Resource`](../) klasse.

```csharp
public override int GetHashCode()
```

### Retourwaarde

retourneert een hashcodewaarde voor dit object.

## Voorbeelden

Toont hoe een hashcode van een resource verkregen kan worden.

```csharp
var project = new Project(DataDir + "Project.mpp");

var resource1 = project.Resources.GetById(1);
var resource2 = project.Resources.GetById(2);

// de hashcode van een resource is gelijk aan de resource-UID 
Console.WriteLine("Resource UID: {0} Hash Code: {1}", resource1.Get(Rsc.Uid), resource1.GetHashCode());
Console.WriteLine("Resource UID: {0} Hash Code: {1}", resource2.Get(Rsc.Uid), resource2.GetHashCode());
```

### Zie ook

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


