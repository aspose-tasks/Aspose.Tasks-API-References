---
title: "Rsc.NotesText"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. Texte brut des notes extrait des données RTF"
type: docs
weight: 480
url: /fr/net/aspose.tasks/rsc/notestext/
---
## Rsc.NotesText field

Texte brut des notes extrait des données RTF.

```csharp
public static readonly Key<string, RscKey> NotesText;
```

## Exemples

Montre comment lire/écrire la propriété Rsc.NotesText.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.NotesText, "Resource Notes");

Console.WriteLine("Notes text: " + resource.Get(Rsc.NotesText));
Console.WriteLine("Notes RTF: " + resource.Get(Rsc.NotesRTF));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


