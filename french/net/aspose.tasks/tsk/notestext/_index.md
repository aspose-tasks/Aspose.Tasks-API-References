---
title: "Tsk.NotesText"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. Texte brut des notes extrait des données RTF"
type: docs
weight: 830
url: /fr/net/aspose.tasks/tsk/notestext/
---
## Tsk.NotesText field

Texte brut des notes extrait des données RTF.

```csharp
public static readonly Key<string, TaskKey> NotesText;
```

## Exemples

Montre comment lire/écrire la propriété Tsk.NotesText.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.NotesText, "Notes");

Console.WriteLine("Notes Text: " + task.Get(Tsk.NotesText));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


