---
title: "ExtendedAttributeDefinition.CreateExtendedAttribute"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método ExtendedAttributeDefinition. Crea un nuevo atributo extendido con el ID de campo que es igual al valor del ID de campo de este objeto"
type: docs
weight: 310
url: /es/net/aspose.tasks/extendedattributedefinition/createextendedattribute/
---
## CreateExtendedAttribute() {#createextendedattribute}

Crea un nuevo atributo extendido con el ID de campo que es igual al valor del ID de campo de este objeto.

```csharp
public ExtendedAttribute CreateExtendedAttribute()
```

### Valor devuelto

devuelve la instancia creada de la clase [`ExtendedAttribute`](../../extendedattribute/) con el fieldID que es igual al fieldID de este objeto.

## Ejemplos

Muestra cómo crear atributos extendidos.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var definition = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Text1);

// Si el campo personalizado no existe en Project, créalo
if (definition == null)
{
    definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, "My text field");
    project.ExtendedAttributes.Add(definition);
}

// Generar atributo extendido a partir de la definición
var attribute = definition.CreateExtendedAttribute();
attribute.TextValue = "Text attribute value";

// Agregar atributo extendido a la tarea
var task = project.RootTask.Children.Add("Task 1");
task.ExtendedAttributes.Add(attribute);

project.Save(OutDir + "CreateExtendedAttributes_out.mpp", SaveFileFormat.Mpp);
```

### Ver también

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(string) {#createextendedattribute_6}

Crea un nuevo atributo extendido con el ID de campo que es igual al valor del ID de campo de este objeto y el valor de texto especificado.

```csharp
public ExtendedAttribute CreateExtendedAttribute(string textValue)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| textValue | Cadena | El valor de texto especificado. |

### Valor devuelto

devuelve la instancia creada de la clase [`ExtendedAttribute`](../../extendedattribute/) con el fieldID que es igual al fieldID de este objeto.

### Excepciones

| excepción | condición |
| --- | --- |
| InvalidOperationException | Si el [`CfType`](../cftype/) actual no es 'Text' |

## Ejemplos

Muestra cómo crear una definición de atributo extendido y establecer un valor de cadena del atributo mientras se construye.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, "My Text");
project.ExtendedAttributes.Add(definition);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 22, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// crear atributo extendido con un valor igual a 'Common Info'
var extendedAttribute = definition.CreateExtendedAttribute("Common Info");

// agregar atributo extendido inicializado con el valor 'Common Info'
task.ExtendedAttributes.Add(extendedAttribute);
```

### Ver también

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(decimal) {#createextendedattribute_5}

Crea un nuevo atributo extendido con el ID de campo que es igual al valor del ID de campo de este objeto y el valor numérico especificado.

```csharp
public ExtendedAttribute CreateExtendedAttribute(decimal numericValue)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| numericValue | Decimal | El valor numérico especificado. |

### Valor devuelto

devuelve la instancia creada de la clase [`ExtendedAttribute`](../../extendedattribute/) con el fieldID que es igual al fieldID de este objeto.

### Excepciones

| excepción | condición |
| --- | --- |
| InvalidOperationException | Si el [`CfType`](../cftype/) actual no es 'Number' o 'Cost' |

## Ejemplos

Muestra cómo crear una definición de atributo extendido y establecer un valor decimal del atributo mientras se construye.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Cost1, "My Cost");
project.ExtendedAttributes.Add(definition);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 22, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// crear atributo extendido con un valor igual a 999m 
var extendedAttribute = definition.CreateExtendedAttribute(999m);

// agregar atributo extendido inicializado con el valor 999m
task.ExtendedAttributes.Add(extendedAttribute);
```

### Ver también

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(DateTime) {#createextendedattribute_4}

Crea un nuevo atributo extendido con el ID de campo que es igual al valor del ID de campo de este objeto y el valor de fecha especificado.

```csharp
public ExtendedAttribute CreateExtendedAttribute(DateTime dateTimeValue)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| dateTimeValue | DateTime | El valor de fecha y hora especificado. |

### Valor devuelto

devuelve la instancia creada de la clase [`ExtendedAttribute`](../../extendedattribute/) con el fieldID que es igual al fieldID de este objeto.

### Excepciones

| excepción | condición |
| --- | --- |
| InvalidOperationException | Si el [`CfType`](../cftype/) actual no es 'Date', 'Start' o 'Finish' |

## Ejemplos

Muestra cómo crear la definición de atributo extendido y establecer un valor de fecha y hora del atributo mientras se construye.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var definitionWithDate = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Date1, "My Date");
project.ExtendedAttributes.Add(definitionWithDate);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 22, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// crear atributo extendido con un valor igual a DateTime.Now 
var extendedAttribute = definitionWithDate.CreateExtendedAttribute(DateTime.Now);

// agregar atributo extendido
task.ExtendedAttributes.Add(extendedAttribute);
```

### Ver también

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(Duration) {#createextendedattribute_1}

Crea un nuevo atributo extendido con el ID de campo que es igual al valor del ID de campo de este objeto y el valor de duración especificado.

```csharp
public ExtendedAttribute CreateExtendedAttribute(Duration durationValue)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| durationValue | Duración | El valor de duración especificado. |

### Valor devuelto

devuelve la instancia creada de la clase [`ExtendedAttribute`](../../extendedattribute/) con el fieldID que es igual al fieldID de este objeto.

### Excepciones

| excepción | condición |
| --- | --- |
| InvalidOperationException | Si el [`CfType`](../cftype/) actual no es 'Duration' |

## Ejemplos

Muestra cómo crear la definición de atributo extendido y establecer una duración mientras se construye.

```csharp
var project = new Project(DataDir + "Project2.mpp");
var task = project.RootTask.Children.Add("Test");
task.Set(Tsk.Start, new DateTime(2020, 4, 22, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Duration1, "Custom Duration");
project.ExtendedAttributes.Add(definition);

// atributo extendido Duration1 = 2 días
var extendedAttribute = definition.CreateExtendedAttribute(project.GetDuration(2, TimeUnitType.Day));

// agregar atributo extendido a la tarea
task.ExtendedAttributes.Add(extendedAttribute);
```

### Ver también

* class [ExtendedAttribute](../../extendedattribute/)
* struct [Duration](../../duration/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(bool) {#createextendedattribute_3}

Crea un nuevo atributo extendido con el ID de campo que es igual al valor del ID de campo de este objeto y el valor de bandera especificado.

```csharp
public ExtendedAttribute CreateExtendedAttribute(bool flagValue)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| flagValue | Boolean | El valor de bandera especificado. |

### Valor devuelto

devuelve la instancia creada de la clase [`ExtendedAttribute`](../../extendedattribute/) con el fieldID que es igual al fieldID de este objeto.

### Excepciones

| excepción | condición |
| --- | --- |
| InvalidOperationException | Si el [`CfType`](../cftype/) actual no es 'Flag' |

## Ejemplos

Muestra cómo crear una definición de atributo extendido y establecer un valor de una bandera mientras se está construyendo.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var resource = project.Resources.Add("Resource 1");
resource.Set(Rsc.Type, ResourceType.Cost);

// crear una definición para un campo personalizado booleano
var definition = ExtendedAttributeDefinition.CreateResourceDefinition(ExtendedAttributeResource.Flag7, "My Custom Flag");

// crear un atributo y establecer el valor inicial a 'true'
var attribute = definition.CreateExtendedAttribute(true);
resource.ExtendedAttributes.Add(attribute);
```

### Ver también

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(Value) {#createextendedattribute_2}

Crea un nuevo atributo extendido vinculado al elemento [`Value`](../../value/) especificado.

```csharp
public ExtendedAttribute CreateExtendedAttribute(Value lookupValue)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| lookupValue | Value | El elemento [`Value`](../../value/) especificado. |

### Valor devuelto

devuelve la instancia creada de la clase [`ExtendedAttribute`](../../extendedattribute/) vinculada al elemento [`Value`](../../value/) especificado.

## Observaciones

*lookupValue* should be previously added to the [`ExtendedAttributeDefinition`](../) using [`AddLookupValue`](../addlookupvalue/) method.

## Ejemplos

Utilice este código para crear un nuevo [`ExtendedAttribute`](../../extendedattribute/) usando un valor específico:

```csharp
taskTextAttr.AddLookupValue(value1);
taskTextAttr.AddLookupValue(value2);
var extendedAttribute = taskTextAttr.CreateExtendedAttribute(value2);
```

Muestra cómo crear la definición de atributo extendido y establecer un valor mientras se construye.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// Cree una definición de campo personalizado basada en la tabla de búsqueda, que se declaró arriba.
var customFieldDefinition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(CustomFieldType.Number, ExtendedAttributeTask.Number10, "Status");

var value1 = new Value { Id = 1, Val = "25", Description = "Active" };
var value2 = new Value { Id = 2, Val = "12", Description = "Inactive" };
customFieldDefinition.AddLookupValue(value1);
customFieldDefinition.AddLookupValue(value2);
project.ExtendedAttributes.Add(customFieldDefinition);

var task = project.RootTask.Children.Add("Task");

// crear atributo extendido para un valor 
var extendedAttribute = customFieldDefinition.CreateExtendedAttribute(value2);

// agregar atributo extendido a la tarea
task.ExtendedAttributes.Add(extendedAttribute);
```

### Ver también

* class [ExtendedAttribute](../../extendedattribute/)
* class [Value](../../value/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


