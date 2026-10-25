---
title: "Project.Get"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Projectmethode. Retourneert de waarde waaraan de eigenschap in deze container is toegewezen."
type: docs
weight: 1080
url: /nl/net/aspose.tasks/project/get/
---
## Project.Get&lt;T&gt; method

Retourneert de waarde waaraan de eigenschap in deze container is toegewezen.

```csharp
public T Get<T>(Key<T, PrjKey> key)
```

| Parameter | Beschrijving |
| --- | --- |
| T | het type van de gekoppelde waarde. |
| key | de opgegeven eigenschapssleutel. [`Prj`](../../prj/) voor het ophalen van de eigenschapssleutel. |

### Retourwaarde

de waarde waaraan de eigenschap is toegewezen in deze container.

## Voorbeelden

Toont hoe een projectversie te controleren.

```csharp
var project = new Project(DataDir + "DetermineProjectVersion.mpp");

// Projectversie weergeven
Console.WriteLine("Project Version : " + project.Get(Prj.SaveVersion));
Console.WriteLine("Last Saved : " + project.Get(Prj.LastSaved).ToShortDateString());
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


