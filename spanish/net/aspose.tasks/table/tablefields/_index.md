---
title: "Table.TableFields"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad Table. Obtiene una colección TableFields que representa los campos de la tabla."
type: docs
weight: 90
url: /es/net/aspose.tasks/table/tablefields/
---
## Table.TableFields property

Obtiene una colección TableFields que representa los campos de la tabla.

```csharp
public TableFieldCollection TableFields { get; }
```

## Ejemplos

Muestra cómo trabajar con las tablas del proyecto.

```csharp
var project = new Project(DataDir + "Project5.mpp");
var task = project.RootTask.Children.Add("New Activity");

// Definir nuevo atributo personalizado
var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, null);
project.ExtendedAttributes.Add(definition);

// Agregar atributo de texto personalizado a la tarea creada.
task.ExtendedAttributes.Add(definition.CreateExtendedAttribute("Activity attribute"));

// Personaliza la tabla añadiendo un campo de atributo de texto
var field = new TableField();
field.Field = Field.TaskText1;
field.Width = 20;
field.Title = "Custom attribute";
field.AlignTitle = HorizontalStringAlignment.Center;
field.AlignData = HorizontalStringAlignment.Center;

var table = project.Tables.ToList()[0];
table.TableFields.Insert(3, field);

project.Save(OutDir + "ConfigureGanttChart_out.mpp", new MPPSaveOptions { WriteViewData = true });
```

### Ver también

* class [TableFieldCollection](../../tablefieldcollection/)
* class [Table](../)
* namespace [Aspose.Tasks](../../table/)
* assembly [Aspose.Tasks](../../../)


