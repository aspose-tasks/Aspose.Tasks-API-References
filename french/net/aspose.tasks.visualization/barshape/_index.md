---
title: "Enum BarShape"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Aspose.Tasks.Visualization.BarShape enum. Forme d'un rectangle de barre"
type: docs
weight: 2950
url: /fr/net/aspose.tasks.visualization/barshape/
---
## BarShape enumeration

Forme du rectangle de la barre.

```csharp
public enum BarShape
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Full | `0` | Indique la forme de barre rectangle pleine. |
| HalfHeight | `1` | Indique la forme de barre rectangle demi‑hauteur alignée en haut. |
| HalfHeightBottom | `2` | Indique la forme de barre rectangle demi‑hauteur alignée en bas. |
| Thin | `3` | Indique la forme de ligne alignée au centre. |
| None | `4` | Indique la forme de barre Aucun. |
| Middle | `5` | Indique la forme de ligne alignée au centre. |
| LineBottom | `6` | Indique la forme de ligne alignée en bas. |
| LineTop | `7` | Indique la forme de ligne alignée en haut. |

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


