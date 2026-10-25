---
title: "ExtendedAttributeCollection.Contains"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método ExtendedAttributeCollection. Devuelve true si el elemento especificado se encuentra en esta colección, de lo contrario false"
type: docs
weight: 60
url: /es/net/aspose.tasks/extendedattributecollection/contains/
---
## ExtendedAttributeCollection.Contains method

Devuelve true si el elemento especificado se encuentra en esta colección; de lo contrario, false.

```csharp
public bool Contains(ExtendedAttribute item)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| elemento | ExtendedAttribute | el elemento especificado para buscar. |

### Valor devuelto

true si el elemento especificado se encuentra en esta colección; de lo contrario, false.

## Ejemplos

Muestra cómo usar colecciones de atributos extendidos.

```csharp
var project = new Project(DataDir + "ReadTaskExtendedAttributes.mpp");

// Obtener tarea de índice cero
var task = project.RootTask.Children.GetById(1);

if (!task.ExtendedAttributes.IsReadOnly && task.ExtendedAttributes.Count > 0)
{
    // limpiar atributos extendidos
    task.ExtendedAttributes.Clear();
}

// crear definición de atributo extendido para una tarea
var taskDefinition1 = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Start, ExtendedAttributeTask.Start7, "Start 7");
var taskDefinition2 = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Finish, ExtendedAttributeTask.Finish7, "Finish 7");
project.ExtendedAttributes.Add(taskDefinition1);
project.ExtendedAttributes.Add(taskDefinition2);

Console.WriteLine("Iterate over task extended attributes of " + task.Get(Tsk.Name) + " task: ");
foreach (var attribute in task.ExtendedAttributes)
{
    Console.WriteLine("Attribute FieldId: " + attribute.FieldId);
    Console.WriteLine("Attribute Value: " + attribute.DateValue);
    Console.WriteLine();
}

// Agregar atributo extendido 1
var extendedAttribute1 = taskDefinition1.CreateExtendedAttribute();
extendedAttribute1.DateValue = new DateTime(2020, 4, 14, 8, 0, 0);
if (task.ExtendedAttributes.IndexOf(extendedAttribute1) < 0)
{
    task.ExtendedAttributes.Insert(0, extendedAttribute1);
}

// Agregar atributo extendido 2
var extendedAttribute2 = taskDefinition2.CreateExtendedAttribute();
extendedAttribute2.DateValue = new DateTime(2020, 4, 14, 17, 0, 0);
task.ExtendedAttributes.Add(extendedAttribute2);

// trabajar con atributos extendidos...

// eliminar atributo extendido por índice
task.ExtendedAttributes.RemoveAt(0);

Console.WriteLine("Count of task's extended attributes: " + task.ExtendedAttributes.Count);

// usar acceso por índice de colección
Console.WriteLine("Attribute 1 Value: " + task.ExtendedAttributes[0].DateValue);

var otherProject = new Project();
var otherTask = otherProject.RootTask.Children.Add("Other task");

// copiar atributos a otro proyecto
var attributes = new ExtendedAttribute[task.ExtendedAttributes.Count];
task.ExtendedAttributes.CopyTo(attributes, 0);

foreach (var attribute in attributes)
{
    otherTask.ExtendedAttributes.Add(attribute);
}

Console.WriteLine();
Console.WriteLine("Iterate over other task's extended attributes: ");
foreach (var attribute in otherTask.ExtendedAttributes)
{
    Console.WriteLine("Other attribute FieldId: " + attribute.FieldId);
    Console.WriteLine("Other attribute Value: " + attribute.DateValue);
    Console.WriteLine();
}

if (task.ExtendedAttributes.Contains(extendedAttribute2))
{
    task.ExtendedAttributes.Remove(extendedAttribute2);
}

// eliminar todas las definiciones de atributos extendidos
while (otherTask.ExtendedAttributes.Count > 0)
{
    otherTask.ExtendedAttributes.Remove(otherTask.ExtendedAttributes[0]);
}
```

### Ver también

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeCollection](../)
* namespace [Aspose.Tasks](../../extendedattributecollection/)
* assembly [Aspose.Tasks](../../../)


