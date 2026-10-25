---
title: "OutlineValue.Value"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "OutlineValue propiedad. Obtiene o establece el valor real"
type: docs
weight: 70
url: /es/net/aspose.tasks/outlinevalue/value/
---
## OutlineValue.Value property

Obtiene o establece el valor real.

```csharp
public string Value { get; set; }
```

## Ejemplos

Muestra cómo trabajar con valores de esquema.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

var outline = new OutlineCodeDefinition();
outline.FieldId = ExtendedAttributeTask.OutlineCode7.ToString("D");
outline.Alias = "My Outline Code";
var outline2 = new OutlineCodeDefinition();
outline2.FieldId = ExtendedAttributeTask.OutlineCode7.ToString("D");
outline2.Alias = "My Outline Code 2";

project.OutlineCodes.Add(outline);

var mask = new OutlineMask();
mask.Type = MaskType.Characters;
outline.Masks.Add(mask);

// crear un valor de esquema
var value = new OutlineValue();

// establecer el valor real
value.Value = "Text value 1";

// establecer el Id único de un valor de código de esquema dentro de un proyecto
value.ValueId = 1;

// obtener un GUID que identifica este valor entre los demás en todo el proyecto
Console.WriteLine("Check value GUID: " + value.ValueGuid);

// establecer el tipo de código de esquema
value.Type = OutlineValueType.Text;

// establecer la descripción de un valor de esquema
value.Description = "Text value descr 1";

// establecer un valor que indique si el valor de esquema está colapsado o no
value.IsCollapsed = false;

// comprobar el id del valor padre
Console.WriteLine("Check parent value id: " + value.ParentValueId);
outline.Values.Add(value);

// crear un valor de esquema con duración
var value2 = new OutlineValue();

// establecer el valor de duración
value2.DurationValue = project.GetDuration(1, TimeUnitType.Hour);

// establecer el Id único de un valor de código de esquema dentro de un proyecto
value2.ValueId = 2;
outline2.Values.Add(value2);

// ...
```

### Ver también

* class [OutlineValue](../)
* namespace [Aspose.Tasks](../../outlinevalue/)
* assembly [Aspose.Tasks](../../../)


