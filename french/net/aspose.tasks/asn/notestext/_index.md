---
title: "Asn.NotesText"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Asn. Texte brut des notes extrait des données RTF"
type: docs
weight: 350
url: /fr/net/aspose.tasks/asn/notestext/
---
## Asn.NotesText field

Texte brut des notes extrait des données RTF.

```csharp
public static readonly Key<string, AsnKey> NotesText;
```

## Exemples

Montre comment obtenir/mettre à jour les notes d'affectation de ressources.

```csharp
var project = new Project(DataDir + "UpdateResourceAssignment.mpp");
var task = project.RootTask.Children.GetById(1);
var rsc = project.Resources.GetById(1);

// créer une affectation de ressource
var assn = project.ResourceAssignments.Add(task, rsc);

// définir les notes d'affectation de ressource 
assn.Set(Asn.NotesText, "Newly added assignment");

Console.WriteLine("Notes text: " + assn.Get(Asn.NotesText));
Console.WriteLine("Notes RTF: " + assn.Get(Asn.NotesRTF));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


