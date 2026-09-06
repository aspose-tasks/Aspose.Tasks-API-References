---
title: "View.Table"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété View. Obtient ou définit une table de la vue unique"
type: docs
weight: 100
url: /fr/net/aspose.tasks/view/table/
---
## View.Table property

Obtient ou définit une table de la vue unique.

```csharp
public Table Table { get; set; }
```

## Exemples

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

Montre comment travailler avec les vues de MS Project.

```csharp
// créer un projet vide sans vues
var project = new Project();
project.Set(Prj.Name, "Test View Project");

// créez une vue de diagramme de Gantt standard
View view = new GanttChartView();

// définissez certaines propriétés de la vue
// définissez une valeur indiquant si Microsoft Project affiche le nom de la vue unique dans la liste déroulante Vue ou Autres Vues dans le ruban
view.ShowInMenu = true;
// définissez une valeur indiquant si Microsoft Project met en évidence le filtre pour une vue unique
view.HighlightFilter = true;

// l'écriture des propriétés suivantes n'est pas prise en charge
// définit le filtre utilisé dans une vue unique
view.Filter = null;
// définit le groupe de la vue unique
view.Group = null;
// définit le tableau de la vue unique
view.Table = null;

// ajustons certains paramètres de la vue
// définissez le nombre de premières colonnes à imprimer sur toutes les pages
view.PageInfo.PageViewSettings.FirstColumnsCount = 4;
// définissez une valeur indiquant s'il faut imprimer un nombre spécifié de premières colonnes sur toutes les pages
view.PageInfo.PageViewSettings.PrintFirstColumnsCountOnAllPages = true;

// ajoutez la vue à notre projet
project.Views.Add(view);

// Le drapeau WriteViewData doit être utilisé pour persister les modifications de project.Views.
project.Save(OutDir + "WorkWithView_output.mpp", new Saving.MPPSaveOptions
{
    WriteViewData = true
});
// vérifions certaines propriétés de la vue nouvellement ajoutée
// affichez l'identifiant unique d'une vue
Console.WriteLine("View Uid: " + view.Uid);
// affichez le type d'écran pour la vue unique
Console.WriteLine("View Screen: " + view.Screen);
Console.WriteLine("View Type: " + view.Type);
Console.WriteLine("Parent Project of the view: " + view.ParentProject.Get(Prj.Name));
```

### Voir aussi

* class [Table](../../table/)
* class [View](../)
* namespace [Aspose.Tasks](../../view/)
* assembly [Aspose.Tasks](../../../)


