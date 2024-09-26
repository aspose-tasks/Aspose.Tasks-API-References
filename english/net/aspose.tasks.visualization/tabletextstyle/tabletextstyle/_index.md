---
title: TableTextStyle.TableTextStyle
second_title: Aspose.Tasks for .NET API Reference
description: TableTextStyle constructor. Initializes a new instance of the TableTextStyle class
type: docs
weight: 10
url: /net/aspose.tasks.visualization/tabletextstyle/tabletextstyle/
---
## TableTextStyle(int) {#constructor}

Initializes a new instance of the [`TableTextStyle`](../) class.

```csharp
public TableTextStyle(int rowUid)
```

| Parameter | Type | Description |
| --- | --- | --- |
| rowUid | Int32 | A specified row unique id. |

## Examples

Shows how to customize table text styles which are used to style different text items in a project.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.NewTasksAreManual, false);

var view = (GanttChartView)project.Views.ToList()[0];

// set first task name text style
var style1 = new TableTextStyle(1);
// set a field the style is to be applied to.
style1.Field = Field.TaskName;
// set <see cref="P:Aspose.Tasks.Visualization.TextStyle.Font" /> of the text style.
style1.Font = new FontDescriptor("Impact", 12F, FontStyles.Bold | FontStyles.Italic);
// set size in points of the text style font.

// set second task duration text style
var style2 = new TableTextStyle(2);
style2.Field = Field.TaskDurationText;
style2.Font = new FontDescriptor("Impact", 16F, FontStyles.Underline);

view.TableTextStyles.Add(style1);
view.TableTextStyles.Add(style2);

SimpleSaveOptions options = new MPPSaveOptions
{
    // set a flag indicating that view data must be written
    WriteViewData = true
};
project.Save(OutDir + "WorkWithTableTextStyle_out.mpp", options);
```

### See Also

* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TableTextStyle(int, FontDescriptor) {#constructor_1}

Initializes a new instance of the [`TableTextStyle`](../) class with the specified font.

```csharp
public TableTextStyle(int rowUid, FontDescriptor font)
```

| Parameter | Type | Description |
| --- | --- | --- |
| rowUid | Int32 | A specified row unique id. |
| font | FontDescriptor | A font on which a text style is based on. |

### See Also

* class [FontDescriptor](../../fontdescriptor/)
* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TableTextStyle(int, float, FontStyles) {#constructor_3}

Initializes a new instance of the [`TableTextStyle`](../) class with the specified font size and font style.

```csharp
public TableTextStyle(int rowUid, float fontSize, FontStyles fontStyle)
```

| Parameter | Type | Description |
| --- | --- | --- |
| rowUid | Int32 | A specified row unique id. |
| fontSize | Single | Size of a font on which a text style is based on. |
| fontStyle | FontStyles | Style of a font on which a text style is based on. |

### See Also

* enum [FontStyles](../../fontstyles/)
* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TableTextStyle(int, FontStyles) {#constructor_2}

Initializes a new instance of the [`TableTextStyle`](../) class with the default font settings and the specified font style.

```csharp
public TableTextStyle(int rowUid, FontStyles fontStyle)
```

| Parameter | Type | Description |
| --- | --- | --- |
| rowUid | Int32 | A specified row unique id. |
| fontStyle | FontStyles | Style of a font on which a text style is based on. |

### See Also

* enum [FontStyles](../../fontstyles/)
* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)


