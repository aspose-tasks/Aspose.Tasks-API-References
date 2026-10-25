---
title: "TableTextStyle.TableTextStyle"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Costruttore TableTextStyle. Inizializza una nuova istanza della classe TableTextStyle"
type: docs
weight: 10
url: /it/net/aspose.tasks.visualization/tabletextstyle/tabletextstyle/
---
## TableTextStyle(int) {#constructor}

Inizializza una nuova istanza della classe [`TableTextStyle`](../).

```csharp
public TableTextStyle(int rowUid)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowUid | Int32 | Un ID univoco di riga specificato. |

## Esempi

Mostra come personalizzare gli stili di testo della tabella che sono usati per formattare diversi elementi di testo in un progetto.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.NewTasksAreManual, false);

var view = (GanttChartView)project.Views.ToList()[0];

// imposta lo stile di testo del nome del primo task
var style1 = new TableTextStyle(1);
// imposta un campo a cui applicare lo stile.
style1.Field = Field.TaskName;
// imposta <see cref="P:Aspose.Tasks.Visualization.TextStyle.Font" /> dello stile di testo.
style1.Font = new FontDescriptor("Impact", 12F, FontStyles.Bold | FontStyles.Italic);
// imposta la dimensione in punti del carattere dello stile di testo.

// imposta lo stile di testo della durata del secondo task
var style2 = new TableTextStyle(2);
style2.Field = Field.TaskDurationText;
style2.Font = new FontDescriptor("Impact", 16F, FontStyles.Underline);

view.TableTextStyles.Add(style1);
view.TableTextStyles.Add(style2);

SimpleSaveOptions options = new MPPSaveOptions
{
    // imposta un flag che indica che i dati della vista devono essere scritti
    WriteViewData = true
};
project.Save(OutDir + "WorkWithTableTextStyle_out.mpp", options);
```

### Vedi anche

* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TableTextStyle(int, FontDescriptor) {#constructor_1}

Inizializza una nuova istanza della classe [`TableTextStyle`](../) con il font specificato.

```csharp
public TableTextStyle(int rowUid, FontDescriptor font)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowUid | Int32 | Un ID univoco di riga specificato. |
| font | FontDescriptor | Un font su cui si basa uno stile di testo. |

### Vedi anche

* class [FontDescriptor](../../fontdescriptor/)
* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TableTextStyle(int, float, FontStyles) {#constructor_3}

Inizializza una nuova istanza della classe [`TableTextStyle`](../) con la dimensione del font e lo stile del font specificati.

```csharp
public TableTextStyle(int rowUid, float fontSize, FontStyles fontStyle)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowUid | Int32 | Un ID univoco di riga specificato. |
| fontSize | Single | Dimensione di un font su cui si basa uno stile di testo. |
| fontStyle | FontStyles | Stile di un font su cui si basa uno stile di testo. |

### Vedi anche

* enum [FontStyles](../../fontstyles/)
* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TableTextStyle(int, FontStyles) {#constructor_2}

Inizializza una nuova istanza della classe [`TableTextStyle`](../) con le impostazioni predefinite del font e lo stile del font specificato.

```csharp
public TableTextStyle(int rowUid, FontStyles fontStyle)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowUid | Int32 | Un ID univoco di riga specificato. |
| fontStyle | FontStyles | Stile di un font su cui si basa uno stile di testo. |

### Vedi anche

* enum [FontStyles](../../fontstyles/)
* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)


