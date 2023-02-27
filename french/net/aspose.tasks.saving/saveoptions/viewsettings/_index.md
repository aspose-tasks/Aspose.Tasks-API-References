---
title: SaveOptions.ViewSettings
second_title: Référence de l'API Aspose.Tasks pour .NET
description: SaveOptions propriété. Obtient ou définit une vue View  rendre. Vous pouvez utiliser ces options pour spécifier explicitement quelle vue doit être enregistrée aux formats PDF HTML ou Image. Si cette propriété est définiePresentationFormat La propriété est ignorée lorsque le projet est enregistré. La vue doit provenir de lun des écrans suivants Screen   Gantt Feuille de tâches Utilisation des tâches Feuille de ressources Utilisation des ressources
type: docs
weight: 240
url: /fr/net/aspose.tasks.saving/saveoptions/viewsettings/
---
## SaveOptions.ViewSettings property

Obtient ou définit une vue ([`View`](../view/) ) rendre. Vous pouvez utiliser ces options pour spécifier explicitement quelle vue doit être enregistrée aux formats PDF, HTML ou Image. Si cette propriété est définie,[`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) La propriété est ignorée lorsque le projet est enregistré. La vue doit provenir de l'un des écrans suivants (([`Screen`](../../../aspose.tasks/view/screen/) )) : (Gantt, Feuille de tâches, Utilisation des tâches, Feuille de ressources, Utilisation des ressources)

```csharp
public View ViewSettings { get; set; }
```

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | Lorsque la méthode set est appelée et qu'une instance de la classe View avec une valeur non prise en charge de la propriété Screen est fournie. |

### Voir également

* class [View](../../../aspose.tasks/view/)
* class [SaveOptions](../)
* espace de noms [Aspose.Tasks.Saving](../../saveoptions/)
* Assemblée [Aspose.Tasks](../../../)


