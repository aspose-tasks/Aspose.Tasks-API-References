---
title: "ExtendedAttributeDefinition.CreateTaskDefinition"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método ExtendedAttributeDefinition. Método de fábrica que crea una definición simple de atributo extendido que Microsoft Project muestra como None. Tiene CalculationType igual a None y solo puede usarse en Tareas. Se requiere especificar customFieldType, fieldId y alias al llamar a este método."
type: docs
weight: 40
url: /es/net/aspose.tasks/extendedattributedefinition/createtaskdefinition/
---
## CreateTaskDefinition(CustomFieldType, ExtendedAttributeTask, string) {#createtaskdefinition}

Método de fábrica que crea una definición simple de atributo extendido, que Microsoft Project muestra como "None". Tiene [`CalculationType`](../calculationtype/) igual a None y solo puede usarse en Tareas. Se requiere especificar *customFieldType*, *fieldId* y *alias* al llamar a este método.

```csharp
public static ExtendedAttributeDefinition CreateTaskDefinition(CustomFieldType customFieldType, 
    ExtendedAttributeTask fieldId, string alias)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| customFieldType | CustomFieldType | El tipo [`CustomFieldType`](../../customfieldtype/) especificado. |
| fieldId | ExtendedAttributeTask | El ID de campo especificado de [`ExtendedAttributeTask`](../../extendedattributetask/). |
| alias | Cadena | El alias de tipo String especificado. |

### Valor devuelto

Instancia creada de la clase [`ExtendedAttributeDefinition`](../) con *customFieldType*, *fieldId* y *alias* especificados.

## Ejemplos

Utilice este ejemplo para crear una definición de campo de texto personalizado:

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text27, "My custom field");
project.ExtendedAttributes.Add(taskTextAttr);
```

Muestra cómo crear los atributos extendidos de la tarea.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// Crear una Definición de Atributo Extendido del tipo Text1
var taskExtendedAttributeText1Definition =
    ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text1, "Task City Name");

// Añádalo a la colección de Atributos Extendidos del proyecto
project.ExtendedAttributes.Add(taskExtendedAttributeText1Definition);

// Agregar una tarea al proyecto
var task = project.RootTask.Children.Add("Task 1");

// Crear un Atributo Extendido a partir de la Definición de Atributo
var taskExtendedAttributeText1 = taskExtendedAttributeText1Definition.CreateExtendedAttribute();

// Asignar un valor al Atributo Extendido generado. El tipo del atributo es "Text", se debe usar la propiedad "TextValue".
taskExtendedAttributeText1.TextValue = "London";

// Agregar el Atributo Extendido a la tarea
task.ExtendedAttributes.Add(taskExtendedAttributeText1);

project.Save(OutDir + "PlainTextExtendedAttribute_out.mpp", SaveFileFormat.Mpp);

var project4 = new Project(DataDir + "Blank2010.mpp");

// Crear una Definición de Atributo Extendido del tipo Text2
var taskExtendedAttributeText2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Text,
    ExtendedAttributeTask.Text2,
    "Task Towns Name");

// Agregar valores de búsqueda para la definición de atributo extendido
taskExtendedAttributeText2Definition.AddLookupValue(new Value { Id = 1, StringValue = "Town1", Description = "This is Town1" });
taskExtendedAttributeText2Definition.AddLookupValue(new Value { Id = 2, StringValue = "Town2", Description = "This is Town2" });

// Añádalo a la colección de Atributos Extendidos del proyecto
project4.ExtendedAttributes.Add(taskExtendedAttributeText2Definition);

// Agregar una tarea al proyecto
var task2 = project4.RootTask.Children.Add("Task 2");

// Crear un Atributo Extendido a partir de la Definición de Búsqueda Text2 para el Id 1
var taskExtendedAttributeText2 = taskExtendedAttributeText2Definition.CreateExtendedAttribute(taskExtendedAttributeText2Definition.ValueList[1]);

// Agregar el Atributo Extendido a la tarea
task2.ExtendedAttributes.Add(taskExtendedAttributeText2);

project4.Save(OutDir + "TextExtendedAttributeWithLookup_out.mpp", SaveFileFormat.Mpp);

var project2 = new Project(DataDir + "Blank2010.mpp");

// Crear una Definición de Atributo Extendido del tipo Duration2
var taskExtendedAttributeDuration2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Duration,
    ExtendedAttributeTask.Duration2,
    "Some duration");

// Agregar valores de búsqueda para la definición de atributo extendido
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 2, Duration = project2.GetDuration(4, TimeUnitType.Hour), Description = "4 hours" });
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 3, Duration = project2.GetDuration(1, TimeUnitType.Day), Description = "1 day" });
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 4, Duration = project2.GetDuration(1, TimeUnitType.Hour), Description = "1 hour" });
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 7, Duration = project2.GetDuration(10, TimeUnitType.Day), Description = "10 days" });

// Agregar la definición a la colección de Atributos Extendidos del proyecto
project2.ExtendedAttributes.Add(taskExtendedAttributeDuration2Definition);

// Agregar una tarea al proyecto
var task3 = project2.RootTask.Children.Add("Task 3");

// Crear un Atributo Extendido a partir de la Definición de Búsqueda Duration2 para el Id 3
var taskExtendedAttributeDuration2 =
    taskExtendedAttributeDuration2Definition.CreateExtendedAttribute(taskExtendedAttributeDuration2Definition.ValueList[3]);

// Agregar el Atributo Extendido a la tarea
task3.ExtendedAttributes.Add(taskExtendedAttributeDuration2);

project2.Save(OutDir + "DurationExtendedAttributeWithLookup_out.mpp", SaveFileFormat.Mpp);

var project3 = new Project(DataDir + "Blank2010.mpp");

// Crear una Definición de Atributo Extendido del tipo Finish2
var taskExtendedAttributeFinish2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Finish,
    ExtendedAttributeTask.Finish2,
    "Some finish");

// Agregar valores de búsqueda para la definición de atributo extendido
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 2, DateTimeValue = new DateTime(1984, 01, 01, 00, 00, 01), Description = "This is Value2" });
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 3, DateTimeValue = new DateTime(1994, 01, 01, 00, 01, 01), Description = "This is Value3" });
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 4, DateTimeValue = new DateTime(2009, 12, 31, 00, 00, 00), Description = "This is Value4" });
taskExtendedAttributeFinish2Definition.AddLookupValue(new Value { Id = 7, DateTimeValue = DateTime.Now, Description = "This is Value6" });

// Agregar la definición a la colección de Atributos Extendidos del proyecto
project3.ExtendedAttributes.Add(taskExtendedAttributeFinish2Definition);

// Agregar una tarea al proyecto
var task4 = project3.RootTask.Children.Add("Task 4");

// Crear un Atributo Extendido a partir de la Definición de Búsqueda Finish2 para el Id 3
var taskExtendedAttributeFinish2 = taskExtendedAttributeFinish2Definition.CreateExtendedAttribute(taskExtendedAttributeFinish2Definition.ValueList[3]);

// Agregar el Atributo Extendido a la tarea
task4.ExtendedAttributes.Add(taskExtendedAttributeFinish2);

project3.Save(OutDir + "FinishExtendedAttributeWithLookup_out.mpp", SaveFileFormat.Mpp);
```

### Ver también

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateTaskDefinition(ExtendedAttributeTask, string) {#createtaskdefinition_1}

Método de fábrica que crea una definición de atributo extendido simple, que Microsoft Project muestra como "None". Tiene [`CalculationType`](../calculationtype/) igual a None y solo puede usarse en Tareas. Se requiere especificar *fieldId* y *alias* al llamar a este método. El tipo de campo se infiere del id del campo.

```csharp
public static ExtendedAttributeDefinition CreateTaskDefinition(ExtendedAttributeTask fieldId, 
    string alias)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fieldId | ExtendedAttributeTask | El ID de campo especificado de [`ExtendedAttributeTask`](../../extendedattributetask/). |
| alias | Cadena | El alias de tipo String especificado. |

### Valor devuelto

Instancia creada de la clase [`ExtendedAttributeDefinition`](../) con *fieldId* y *alias* especificados.

## Ejemplos

Utilice este ejemplo para crear una definición de campo de texto personalizado:

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text27, "My custom field");
project.ExtendedAttributes.Add(taskTextAttr);
```

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

* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


