---
title: "Class BarStyle"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Aspose.Tasks.Visualization.BarStyle class. Modifie le style visuel de la barre pour l'élément dans la vue du projet"
type: docs
weight: 2960
url: /fr/net/aspose.tasks.visualization/barstyle/
---
## BarStyle class

Modifiez le style visuel de la barre pour l'élément dans la vue du projet.

```csharp
public class BarStyle
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [BarStyle](barstyle/)() | Initialise une nouvelle instance de la classe `BarStyle`. |

## Propriétés

| Nom | Description |
| --- | --- |
| [BarColor](../../aspose.tasks.visualization/barstyle/barcolor/) { get; set; } | Obtient ou définit la couleur du style de barre. |
| [BarShape](../../aspose.tasks.visualization/barstyle/barshape/) { get; set; } | Obtient ou définit [`BarShape`](./barshape/) du style de barre. |
| [BottomBarTextConverter](../../aspose.tasks.visualization/barstyle/bottombartextconverter/) { get; set; } | Obtient ou définit le convertisseur défini par l'utilisateur pour obtenir le texte à afficher en bas de la barre de la tâche. Remplace la valeur de la propriété [`BottomField`](./bottomfield/). |
| [BottomField](../../aspose.tasks.visualization/barstyle/bottomfield/) { get; set; } | Obtient ou définit un champ à afficher en bas de la barre. |
| [EndShape](../../aspose.tasks.visualization/barstyle/endshape/) { get; set; } | Obtient ou définit [`Shape`](../shape/) à l'extrémité de la barre. |
| [EndShapeColor](../../aspose.tasks.visualization/barstyle/endshapecolor/) { get; set; } | Obtient ou définit la couleur de la forme à l'extrémité de la barre. |
| [EndShapeType](../../aspose.tasks.visualization/barstyle/endshapetype/) { get; set; } | Obtient ou définit un type de forme de fin. [`GanttBarType`](../ganttbartype/). |
| [From](../../aspose.tasks.visualization/barstyle/from/) { get; set; } | Obtient ou définit la position du point de départ de la barre Gantt. [`Field`](../../aspose.tasks/field/). |
| [InsideBarTextConverter](../../aspose.tasks.visualization/barstyle/insidebartextconverter/) { get; set; } | Obtient ou définit le convertisseur défini par l'utilisateur pour obtenir le texte à afficher à l'intérieur de la barre de la tâche. Remplace la valeur de la propriété [`InsideField`](./insidefield/). |
| [InsideField](../../aspose.tasks.visualization/barstyle/insidefield/) { get; set; } | Obtient ou définit un champ à afficher à l'intérieur de la barre. |
| [ItemType](../../aspose.tasks.visualization/barstyle/itemtype/) { get; set; } | Obtient ou définit [`BarItemType`](../baritemtype/) du style de barre. |
| [LeftBarTextConverter](../../aspose.tasks.visualization/barstyle/leftbartextconverter/) { get; set; } | Obtient ou définit un convertisseur défini par l'utilisateur pour obtenir le texte à rendre à gauche de la barre de la tâche. Remplace la valeur de la propriété [`LeftField`](./leftfield/). |
| [LeftField](../../aspose.tasks.visualization/barstyle/leftfield/) { get; set; } | Obtient ou définit un champ à afficher à gauche de la barre. |
| [RightBarTextConverter](../../aspose.tasks.visualization/barstyle/rightbartextconverter/) { get; set; } | Obtient ou définit le convertisseur défini par l'utilisateur pour obtenir le texte à afficher à droite de la barre de la tâche. Remplace la valeur de la propriété [`RightField`](./rightfield/). |
| [RightField](../../aspose.tasks.visualization/barstyle/rightfield/) { get; set; } | Obtient ou définit un champ à afficher à droite de la barre. |
| [StartShape](../../aspose.tasks.visualization/barstyle/startshape/) { get; set; } | Obtient ou définit [`Shape`](../shape/) au début de la barre. |
| [StartShapeColor](../../aspose.tasks.visualization/barstyle/startshapecolor/) { get; set; } | Obtient ou définit la couleur de la forme au début de la barre. |
| [StartShapeType](../../aspose.tasks.visualization/barstyle/startshapetype/) { get; set; } | Obtient ou définit un type de forme de départ. |
| [TextStyle](../../aspose.tasks.visualization/barstyle/textstyle/) { get; set; } | Obtient ou définit le style du texte de la barre. |
| [To](../../aspose.tasks.visualization/barstyle/to/) { get; set; } | Obtient ou définit la position du point d'arrivée de la barre Gantt. |
| [TopBarTextConverter](../../aspose.tasks.visualization/barstyle/topbartextconverter/) { get; set; } | Obtient ou définit le convertisseur défini par l'utilisateur pour obtenir le texte à afficher en haut de la barre de la tâche. Remplace la valeur de la propriété [`TopField`](./topfield/). |
| [TopField](../../aspose.tasks.visualization/barstyle/topfield/) { get; set; } | Obtient ou définit un champ à afficher en haut de la barre. |

## Exemples

Montre comment utiliser des styles de barre personnalisés.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    BarStyles = new List<BarStyle>()
};

// ajoutez un style de barre pour les tâches jalon
var style = new BarStyle();
// définissez <see cref="T:Aspose.Tasks.Visualization.BarItemType" /> du style de barre
style.ItemType = BarItemType.Milestone;
// définissez <see cref="T:System.Drawing.Color" /> du style de barre.
style.BarColor = Color.Green;
// définissez <see cref="P:Aspose.Tasks.Visualization.BarStyle.BarShape" /> du style de barre
style.BarShape = BarShape.HalfHeight;
// définir <see cref="T:Aspose.Tasks.Visualization.Shape" /> au début de la barre
style.StartShape = Shape.LeftBracket;
// définir <see cref="T:System.Drawing.Color" /> de la forme au début de la barre
style.StartShapeColor = Color.Aqua;
// définir <see cref="T:Aspose.Tasks.Visualization.Shape" /> à la fin de la barre
style.EndShape = Shape.RightBracket;
// définir <see cref="T:System.Drawing.Color" /> de la forme à la fin de la barre
style.EndShapeColor = Color.Aquamarine;
// définir le texte à afficher à droite de la barre.
style.TextStyle = new TextStyle();
style.TextStyle.BackgroundColor = Color.Black;

// il existe une fonctionnalité qui permet de convertir le texte de la barre
// définissons le convertisseur pour obtenir le texte de la barre à afficher.
style.LeftBarTextConverter = task =>
{
    if (!task.Get(Tsk.Name).StartsWith("T"))
    {
        task.Set(Tsk.Name, "T" + task.Get(Tsk.Name));
    }

    return task.Get(Tsk.Name);
};

options.BarStyles.Add(style);

// enregistrer le projet
project.Save(OutDir + "WorkWithBarStyle_out.mpp", options);
```

### Voir aussi

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


