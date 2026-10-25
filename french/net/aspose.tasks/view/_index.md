---
title: "Classe View"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.View. Représente une vue dans Project"
type: docs
weight: 2890
url: /fr/net/aspose.tasks/view/
---
## View class

Représente une vue dans Project.

```csharp
public class View : IComparable<View>
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [View](view/#constructor)() | Initialise une nouvelle instance de la classe `View`. |
| [View](view/#constructor_1)(ViewScreen) | Initialise une nouvelle instance de la classe `View`. |

## Propriétés

| Nom | Description |
| --- | --- |
| [Filter](../../aspose.tasks/view/filter/) { get; set; } | Obtient ou définit un filtre utilisé dans une vue unique. |
| [Group](../../aspose.tasks/view/group/) { get; set; } | Obtient ou définit un groupe de la vue unique. |
| [HighlightFilter](../../aspose.tasks/view/highlightfilter/) { get; set; } | Obtient ou définit une valeur indiquant si Microsoft Project met en évidence le filtre pour une vue unique. |
| [Name](../../aspose.tasks/view/name/) { get; set; } | Obtient ou définit le nom d’un objet View. |
| [PageInfo](../../aspose.tasks/view/pageinfo/) { get; } | Obtient une instance de la classe [`PageInfo`](./pageinfo/). Représente les données de configuration de page présentes dans le format de fichier mpp. |
| [ParentProject](../../aspose.tasks/view/parentproject/) { get; } | Obtient le parent de l’objet View. Lecture seule [`Project`](../project/). |
| [Screen](../../aspose.tasks/view/screen/) { get; } | Obtient le type d’écran pour la vue unique. Lecture seule [`ViewScreen`](../viewscreen/). |
| [ShowInMenu](../../aspose.tasks/view/showinmenu/) { get; set; } | Obtient ou définit une valeur indiquant si Microsoft Project affiche le nom de la vue unique dans les listes déroulantes Vue ou Autres Vues du Ruban. |
| [Table](../../aspose.tasks/view/table/) { get; set; } | Obtient ou définit une table de la vue unique. |
| [Type](../../aspose.tasks/view/type/) { get; } | Obtient le type d’élément dans la vue unique, tel que les tâches ou les ressources. Lecture seule [`ItemType`](../itemtype/). |
| [Uid](../../aspose.tasks/view/uid/) { get; } | Obtient l’identifiant unique d’une vue. |
| [VisualObjectsPlacements](../../aspose.tasks/view/visualobjectsplacements/) { get; } | Obtient une collection d’objets représentant le placement et l’apparence de [`OleObject`](../oleobject/) dans la vue. |

## Méthodes

| Nom | Description |
| --- | --- |
| [CompareTo](../../aspose.tasks/view/compareto/)(View) | Compare l’instance actuelle avec un autre objet du même type et renvoie un entier indiquant si l’instance actuelle précède, suit ou se trouve à la même position dans l’ordre de tri que l’autre objet. |
| override [Equals](../../aspose.tasks/view/equals/)(object) | Renvoie une valeur indiquant si cette instance est égale à un objet spécifié. |
| override [GetHashCode](../../aspose.tasks/view/gethashcode/)() | Renvoie une valeur de code de hachage pour l’instance de la classe [`Resource`](../resource/). |
| [operator ==](../../aspose.tasks/view/op_equality/) | Renvoie une valeur indiquant si cette instance est égale à un objet spécifié. |
| [operator &gt;](../../aspose.tasks/view/op_greaterthan/) | Renvoie une valeur indiquant si cette instance est supérieure à un objet spécifié. |
| [operator &gt;=](../../aspose.tasks/view/op_greaterthanorequal/) | Renvoie une valeur indiquant si cette instance est supérieure ou égale à un objet spécifié. |
| [operator !=](../../aspose.tasks/view/op_inequality/) | Renvoie une valeur indiquant si cette instance n'est pas égale à un objet spécifié. |
| [operator &lt;](../../aspose.tasks/view/op_lessthan/) | Renvoie une valeur indiquant si cette instance est inférieure à un objet spécifié. |
| [operator &lt;=](../../aspose.tasks/view/op_lessthanorequal/) | Renvoie une valeur indiquant si cette instance est inférieure ou égale à un objet spécifié. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


