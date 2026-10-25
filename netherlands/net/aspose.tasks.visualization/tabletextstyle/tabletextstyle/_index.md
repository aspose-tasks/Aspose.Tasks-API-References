---
title: "TableTextStyle.TableTextStyle"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "TableTextStyle constructor. Initialiseert een nieuwe instantie van de TableTextStyle‑klasse."
type: docs
weight: 10
url: /nl/net/aspose.tasks.visualization/tabletextstyle/tabletextstyle/
---
## TableTextStyle(int) {#constructor}

Initialiseert een nieuwe instantie van de [`TableTextStyle`](../) klasse.

```csharp
public TableTextStyle(int rowUid)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| rowUid | Int32 | Een opgegeven unieke rij‑id. |

## Voorbeelden

Toont hoe tabeltekststijlen kunnen worden aangepast die worden gebruikt om verschillende tekstitems in een project te stijlen.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.NewTasksAreManual, false);

var view = (GanttChartView)project.Views.ToList()[0];

// stel eerste taaknaam tekststijl in
var style1 = new TableTextStyle(1);
// stel een veld in waarop de stijl moet worden toegepast.
style1.Field = Field.TaskName;
// stel <see cref="P:Aspose.Tasks.Visualization.TextStyle.Font" /> van de tekststijl in.
style1.Font = new FontDescriptor("Impact", 12F, FontStyles.Bold | FontStyles.Italic);
// stel grootte in punten van het lettertype van de tekststijl in.

// stel tweede taakduur tekststijl in
var style2 = new TableTextStyle(2);
style2.Field = Field.TaskDurationText;
style2.Font = new FontDescriptor("Impact", 16F, FontStyles.Underline);

view.TableTextStyles.Add(style1);
view.TableTextStyles.Add(style2);

SimpleSaveOptions options = new MPPSaveOptions
{
    // stel een vlag in die aangeeft dat weergavegegevens moeten worden geschreven
    WriteViewData = true
};
project.Save(OutDir + "WorkWithTableTextStyle_out.mpp", options);
```

### Zie ook

* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TableTextStyle(int, FontDescriptor) {#constructor_1}

Initialiseert een nieuwe instantie van de [`TableTextStyle`](../) klasse met het opgegeven lettertype.

```csharp
public TableTextStyle(int rowUid, FontDescriptor font)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| rowUid | Int32 | Een opgegeven unieke rij‑id. |
| font | FontDescriptor | Een lettertype waarop een tekststijl is gebaseerd. |

### Zie ook

* class [FontDescriptor](../../fontdescriptor/)
* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TableTextStyle(int, float, FontStyles) {#constructor_3}

Initialiseert een nieuwe instantie van de [`TableTextStyle`](../) klasse met de opgegeven lettergrootte en lettertype‑stijl.

```csharp
public TableTextStyle(int rowUid, float fontSize, FontStyles fontStyle)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| rowUid | Int32 | Een opgegeven unieke rij‑id. |
| fontSize | Single | Grootte van een lettertype waarop een tekststijl is gebaseerd. |
| fontStyle | FontStyles | Stijl van een lettertype waarop een tekststijl is gebaseerd. |

### Zie ook

* enum [FontStyles](../../fontstyles/)
* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TableTextStyle(int, FontStyles) {#constructor_2}

Initialiseert een nieuwe instantie van de [`TableTextStyle`](../) klasse met de standaard lettertype‑instellingen en de opgegeven lettertype‑stijl.

```csharp
public TableTextStyle(int rowUid, FontStyles fontStyle)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| rowUid | Int32 | Een opgegeven unieke rij‑id. |
| fontStyle | FontStyles | Stijl van een lettertype waarop een tekststijl is gebaseerd. |

### Zie ook

* enum [FontStyles](../../fontstyles/)
* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)


