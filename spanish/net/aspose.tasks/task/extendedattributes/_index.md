---
title: "Task.ExtendedAttributes"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad Task. Obtiene el objeto ExtendedAttributeCollection que contiene los valores de un atributo extendido"
type: docs
weight: 400
url: /es/net/aspose.tasks/task/extendedattributes/
---
## Task.ExtendedAttributes property

Obtiene el objeto ExtendedAttributeCollection que contiene los valores de un atributo extendido.

```csharp
public ExtendedAttributeCollection ExtendedAttributes { get; }
```

## Observaciones

Se requieren dos piezas de datos: un puntero a la tabla de atributos extendidos que se especifica ya sea por el ID único o el ID de campo, y el valor que se especifica ya sea con el valor, o un puntero a la lista de valores.

## Ejemplos

Muestra cómo leer los atributos extendidos de la tarea.

```csharp
var project = new Project(DataDir + "ReadTaskExtendedAttributes.mpp");

// Crear definición de atributo extendido
var definition = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Start, ExtendedAttributeTask.Start7, "Start 7");
project.ExtendedAttributes.Add(definition);

// Obtener tarea de índice cero
var tsk = project.RootTask.Children.GetById(1);

// Agregar atributo extendido
var extendedAttribute = definition.CreateExtendedAttribute();
extendedAttribute.DateValue = DateTime.Now;

// También se puede usar la siguiente sintaxis corta: ExtendedAttribute attribute = attributeDefinition.CreateExtendedAttribute(DateTime.Now);
tsk.ExtendedAttributes.Add(extendedAttribute);

// Crear una Definición de Atributo Extendido del tipo Text1
var taskExtendedAttributeText1Definition =
    ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text1, "Task City Name");

// Añádalo a la colección de Atributos Extendidos del proyecto
project.ExtendedAttributes.Add(taskExtendedAttributeText1Definition);

var newTask = project.RootTask.Children.Add("Task 1");

// Crear un Atributo Extendido a partir de la Definición de Atributo
var taskExtendedAttributeText1 = taskExtendedAttributeText1Definition.CreateExtendedAttribute();

// Asignar un valor al Atributo Extendido generado. El tipo del atributo es "Text", se debe usar la propiedad "TextValue".
taskExtendedAttributeText1.TextValue = "London";

// Agregar el Atributo Extendido a la tarea
newTask.ExtendedAttributes.Add(taskExtendedAttributeText1);

// Crear una Definición de Atributo Extendido del tipo Text2
var taskExtendedAttributeText2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Text,
    ExtendedAttributeTask.Text2,
    "Task Towns Name");

// Agregar valores de búsqueda para la definición de atributo extendido
taskExtendedAttributeText2Definition.AddLookupValue(new Value { Id = 1, StringValue = "Town1", Description = "This is Town1" });
taskExtendedAttributeText2Definition.AddLookupValue(new Value { Id = 2, StringValue = "Town2", Description = "This is Town2" });

// Añádalo a la colección de Atributos Extendidos del proyecto
project.ExtendedAttributes.Add(taskExtendedAttributeText2Definition);

var task2 = project.RootTask.Children.Add("Task 2");

// Crear un Atributo Extendido a partir de la Definición de Búsqueda Text2 para el Id 1
var taskExtendedAttributeText2 = taskExtendedAttributeText2Definition.CreateExtendedAttribute(taskExtendedAttributeText2Definition.ValueList[1]);

// Agregar el Atributo Extendido a la tarea
task2.ExtendedAttributes.Add(taskExtendedAttributeText2);

// Crear una Definición de Atributo Extendido del tipo Duration2
var taskExtendedAttributeDuration2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Duration,
    ExtendedAttributeTask.Duration2,
    "Some duration");

// Agregar valores de búsqueda para la definición de atributo extendido
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 3, Duration = project.GetDuration(4, TimeUnitType.Hour), Description = "4 hours" });
taskExtendedAttributeDuration2Definition.AddLookupValue(new Value { Id = 4, Duration = project.GetDuration(1, TimeUnitType.Day), Description = "1 day" });
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 5, Duration = project.GetDuration(1, TimeUnitType.Hour), Description = "1 hour" });
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 6, Duration = project.GetDuration(10, TimeUnitType.Day), Description = "10 days" });

// Agregar la definición a la colección de Atributos Extendidos del proyecto
project.ExtendedAttributes.Add(taskExtendedAttributeDuration2Definition);

var task3 = project.RootTask.Children.Add("Task 3");

// Crear un Atributo Extendido a partir de la Definición de Búsqueda Duration2 para el Id 3
var taskExtendedAttributeDuration2 =
    taskExtendedAttributeDuration2Definition.CreateExtendedAttribute(taskExtendedAttributeDuration2Definition.ValueList[3]);

// Agregar el Atributo Extendido a la tarea
task3.ExtendedAttributes.Add(taskExtendedAttributeDuration2);

// Crear una Definición de Atributo Extendido del tipo Finish2
var taskExtendedAttributeFinish2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Finish,
    ExtendedAttributeTask.Finish2,
    "Some finish");

// Agregar valores de búsqueda para la definición de atributo extendido
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 7, DateTimeValue = new DateTime(1984, 01, 01, 00, 00, 01), Description = "This is Value2" });
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 8, DateTimeValue = new DateTime(1994, 01, 01, 00, 01, 01), Description = "This is Value3" });
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 9, DateTimeValue = new DateTime(2009, 12, 31, 00, 00, 00), Description = "This is Value4" });
taskExtendedAttributeFinish2Definition.AddLookupValue(new Value { Id = 10, DateTimeValue = DateTime.Now, Description = "This is Value6" });

// Agregar la definición a la colección de Atributos Extendidos del proyecto
project.ExtendedAttributes.Add(taskExtendedAttributeFinish2Definition);

var task4 = project.RootTask.Children.Add("Task 4");

// Crear un Atributo Extendido a partir de la Definición de Búsqueda Finish2 para el Id 3
var taskExtendedAttributeFinish2 = taskExtendedAttributeFinish2Definition.CreateExtendedAttribute(taskExtendedAttributeFinish2Definition.ValueList[3]);

// Agregar el Atributo Extendido a la tarea
task4.ExtendedAttributes.Add(taskExtendedAttributeFinish2);

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Leer atributos extendidos para tareas
foreach (var task in collector.Tasks)
{
    foreach (var attribute in task.ExtendedAttributes)
    {
        Console.WriteLine(attribute.FieldId);
        Console.WriteLine(attribute.ValueGuid);

        switch (attribute.AttributeDefinition.CfType)
        {
            case CustomFieldType.Date:
            case CustomFieldType.Start:
            case CustomFieldType.Finish:
                Console.WriteLine(attribute.DateValue);
                break;
            case CustomFieldType.Text:
                Console.WriteLine(attribute.TextValue);
                break;
            case CustomFieldType.Duration:
                Console.WriteLine(attribute.DurationValue.ToString());
                break;
            case CustomFieldType.Cost:
            case CustomFieldType.Number:
                Console.WriteLine(attribute.NumericValue);
                break;
            case CustomFieldType.Flag:
                Console.WriteLine(attribute.FlagValue);
                break;
            case CustomFieldType.Null:
            case CustomFieldType.RBS:
            case CustomFieldType.OutlineCode:
                return;
            default:
                return;
        }
    }
}

project.Save(OutDir + "ReadWriteTaskExtendedAttributes_out.mpp", SaveFileFormat.Mpp);
```

### Ver también

* class [ExtendedAttributeCollection](../../extendedattributecollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


