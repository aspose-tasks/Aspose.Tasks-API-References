---
title: "Project.DefaultView"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété du projet. Obtient ou définit la vue par défaut du projet"
type: docs
weight: 360
url: /fr/net/aspose.tasks/project/defaultview/
---
## Project.DefaultView property

Obtient ou définit la vue par défaut du projet.

```csharp
public View DefaultView { get; set; }
```

## Exemples

Montre comment travailler avec la vue par défaut d'un projet.

```csharp
var project = new Project(DataDir + "TaskUsageViewWithDetails.mpp");

// Obtenir la vue par défaut
UsageView view = (TaskUsageView)project.DefaultView;

// La colonne d'en-tête des détails ne sera pas affichée
view.DisplayDetailsHeaderColumn = false;
view.RepeatDetailsHeaderOnAllRows = false;
view.AlignDetailsData = HorizontalStringAlignment.Near;
project.Save(OutDir + "task usage1_out.pdf", SaveFileFormat.Pdf);

// Afficher la colonne d'en-tête des détails
view.DisplayDetailsHeaderColumn = true;

// Répéter l'en-tête des détails sur toutes les lignes d'affectations
view.RepeatDetailsHeaderOnAllRows = true;
view.AlignDetailsData = HorizontalStringAlignment.Far;
project.Save(OutDir + "task usage2_out.pdf", SaveFileFormat.Pdf);
```

Montre comment travailler avec la vue du projet et ajouter une colonne à la vue par défaut (qui est affichée lorsque le fichier MPP est ouvert dans MS Project).

```csharp
// créer un projet vide sans vues
var project = new Project();
project.Set(Prj.Name, "Test View Project");

// Modifier la vue par défaut (c’est une vue de diagramme de Gantt).
// Ou vous pouvez sélectionner la vue par son nom ou via l’écran de vue en utilisant la collection project.View.
var view = (GanttChartView) project.DefaultView;

TableField newColumn = new TableField()
{
    AlignData = HorizontalStringAlignment.Center,
    Title = "My new column",
    Width = 30,
    Field = Field.TaskActualDuration
};

view.Table.TableFields.Add(newColumn);

// Le drapeau WriteViewData doit être utilisé pour persister les modifications des propriétés de la vue.
project.Save(OutDir + "ModifyView_output.mpp", new Saving.MPPSaveOptions
{
    WriteViewData = true
});
```

### Voir aussi

* class [View](../../view/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


