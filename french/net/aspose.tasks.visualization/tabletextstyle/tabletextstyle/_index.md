---
title: "TableTextStyle.TableTextStyle"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Constructeur TableTextStyle. Initialise une nouvelle instance de la classe TableTextStyle."
type: docs
weight: 10
url: /fr/net/aspose.tasks.visualization/tabletextstyle/tabletextstyle/
---
## TableTextStyle(int) {#constructor}

Initialise une nouvelle instance de la classe [`TableTextStyle`](../).

```csharp
public TableTextStyle(int rowUid)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| rowUid | Int32 | Un identifiant unique de ligne spécifié. |

## Exemples

Montre comment personnaliser les styles de texte de tableau qui sont utilisés pour styliser différents éléments de texte dans un projet.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.NewTasksAreManual, false);

var view = (GanttChartView)project.Views.ToList()[0];

// définir le style de texte du premier nom de tâche
var style1 = new TableTextStyle(1);
// définir un champ auquel le style doit être appliqué.
style1.Field = Field.TaskName;
// définir <see cref=\"P:Aspose.Tasks.Visualization.TextStyle.Font\" /> du style de texte.
style1.Font = new FontDescriptor("Impact", 12F, FontStyles.Bold | FontStyles.Italic);
// définir la taille en points de la police du style de texte.

// définir le style de texte de la durée de la deuxième tâche
var style2 = new TableTextStyle(2);
style2.Field = Field.TaskDurationText;
style2.Font = new FontDescriptor("Impact", 16F, FontStyles.Underline);

view.TableTextStyles.Add(style1);
view.TableTextStyles.Add(style2);

SimpleSaveOptions options = new MPPSaveOptions
{
    // définir un indicateur indiquant que les données de vue doivent être écrites
    WriteViewData = true
};
project.Save(OutDir + "WorkWithTableTextStyle_out.mpp", options);
```

### Voir aussi

* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TableTextStyle(int, FontDescriptor) {#constructor_1}

Initialise une nouvelle instance de la classe [`TableTextStyle`](../) avec la police spécifiée.

```csharp
public TableTextStyle(int rowUid, FontDescriptor font)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| rowUid | Int32 | Un identifiant unique de ligne spécifié. |
| font | FontDescriptor | Une police sur laquelle un style de texte est basé. |

### Voir aussi

* class [FontDescriptor](../../fontdescriptor/)
* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TableTextStyle(int, float, FontStyles) {#constructor_3}

Initialise une nouvelle instance de la classe [`TableTextStyle`](../) avec la taille de police et le style de police spécifiés.

```csharp
public TableTextStyle(int rowUid, float fontSize, FontStyles fontStyle)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| rowUid | Int32 | Un identifiant unique de ligne spécifié. |
| fontSize | Single | Taille d'une police sur laquelle un style de texte est basé. |
| fontStyle | FontStyles | Style d'une police sur laquelle un style de texte est basé. |

### Voir aussi

* enum [FontStyles](../../fontstyles/)
* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TableTextStyle(int, FontStyles) {#constructor_2}

Initialise une nouvelle instance de la classe [`TableTextStyle`](../) avec les paramètres de police par défaut et le style de police spécifié.

```csharp
public TableTextStyle(int rowUid, FontStyles fontStyle)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| rowUid | Int32 | Un identifiant unique de ligne spécifié. |
| fontStyle | FontStyles | Style d'une police sur laquelle un style de texte est basé. |

### Voir aussi

* enum [FontStyles](../../fontstyles/)
* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)


