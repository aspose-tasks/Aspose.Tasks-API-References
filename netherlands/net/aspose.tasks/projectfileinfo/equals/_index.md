---
title: "ProjectFileInfo.Equals"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ProjectFileInfo methode. Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object"
type: docs
weight: 50
url: /nl/net/aspose.tasks/projectfileinfo/equals/
---
## Equals(ProjectFileInfo) {#equals}

Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object.

```csharp
public bool Equals(ProjectFileInfo other)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| anders | ProjectFileInfo | Het opgegeven object om te vergelijken met deze instantie. |

### Retourwaarde

retourneert true als de opgegeven ProjectFileInfo en deze instantie een gelijk bestandsformaat en applicatie‑informatie hebben.

## Voorbeelden

Toont hoe je projectbestandsinformatie kunt lezen.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### Zie ook

* class [ProjectFileInfo](../)
* namespace [Aspose.Tasks](../../projectfileinfo/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object.

```csharp
public override bool Equals(object obj)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| obj | Object | Het opgegeven object om te vergelijken met deze instantie. |

### Retourwaarde

retourneert true als de opgegeven ProjectFileInfo en deze instantie een gelijk bestandsformaat en applicatie‑informatie hebben.

## Voorbeelden

Toont hoe je projectbestandsinformatie kunt lezen.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### Zie ook

* class [ProjectFileInfo](../)
* namespace [Aspose.Tasks](../../projectfileinfo/)
* assembly [Aspose.Tasks](../../../)


