---
title: "TableTextStyle.TableTextStyle"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Constructor TableTextStyle. Inicializa una nueva instancia de la clase TableTextStyle."
type: docs
weight: 10
url: /es/net/aspose.tasks.visualization/tabletextstyle/tabletextstyle/
---
## TableTextStyle(int) {#constructor}

Inicializa una nueva instancia de la clase [`TableTextStyle`](../).

```csharp
public TableTextStyle(int rowUid)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowUid | Int32 | Un ID único de fila especificado. |

## Ejemplos

Muestra cómo personalizar los estilos de texto de tabla que se utilizan para dar estilo a diferentes elementos de texto en un proyecto.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.NewTasksAreManual, false);

var view = (GanttChartView)project.Views.ToList()[0];

// establecer estilo de texto del nombre de la primera tarea
var style1 = new TableTextStyle(1);
// establecer un campo al que se aplicará el estilo.
style1.Field = Field.TaskName;
// establecer <see cref=\"P:Aspose.Tasks.Visualization.TextStyle.Font\" /> del estilo de texto.
style1.Font = new FontDescriptor("Impact", 12F, FontStyles.Bold | FontStyles.Italic);
// establecer el tamaño en puntos de la fuente del estilo de texto.

// establecer estilo de texto de la duración de la segunda tarea
var style2 = new TableTextStyle(2);
style2.Field = Field.TaskDurationText;
style2.Font = new FontDescriptor("Impact", 16F, FontStyles.Underline);

view.TableTextStyles.Add(style1);
view.TableTextStyles.Add(style2);

SimpleSaveOptions options = new MPPSaveOptions
{
    // establecer una bandera que indique que los datos de vista deben escribirse
    WriteViewData = true
};
project.Save(OutDir + "WorkWithTableTextStyle_out.mpp", options);
```

### Ver también

* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TableTextStyle(int, FontDescriptor) {#constructor_1}

Inicializa una nueva instancia de la clase [`TableTextStyle`](../) con la fuente especificada.

```csharp
public TableTextStyle(int rowUid, FontDescriptor font)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowUid | Int32 | Un ID único de fila especificado. |
| font | FontDescriptor | Una fuente sobre la cual se basa un estilo de texto. |

### Ver también

* class [FontDescriptor](../../fontdescriptor/)
* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TableTextStyle(int, float, FontStyles) {#constructor_3}

Inicializa una nueva instancia de la clase [`TableTextStyle`](../) con el tamaño de fuente y el estilo de fuente especificados.

```csharp
public TableTextStyle(int rowUid, float fontSize, FontStyles fontStyle)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowUid | Int32 | Un ID único de fila especificado. |
| fontSize | Single | Tamaño de una fuente sobre la cual se basa un estilo de texto. |
| fontStyle | FontStyles | Estilo de una fuente sobre la cual se basa un estilo de texto. |

### Ver también

* enum [FontStyles](../../fontstyles/)
* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TableTextStyle(int, FontStyles) {#constructor_2}

Inicializa una nueva instancia de la clase [`TableTextStyle`](../) con la configuración de fuente predeterminada y el estilo de fuente especificado.

```csharp
public TableTextStyle(int rowUid, FontStyles fontStyle)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowUid | Int32 | Un ID único de fila especificado. |
| fontStyle | FontStyles | Estilo de una fuente sobre la cual se basa un estilo de texto. |

### Ver también

* enum [FontStyles](../../fontstyles/)
* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)


