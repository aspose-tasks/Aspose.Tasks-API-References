---
title: "ExtendedAttributeCollection.CopyTo"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo ExtendedAttributeCollection. Copia gli elementi di questa collezione nell'array specificato a partire dall'indice di array specificato"
type: docs
weight: 70
url: /it/net/aspose.tasks/extendedattributecollection/copyto/
---
## ExtendedAttributeCollection.CopyTo method

Copia gli elementi di questa collezione nell'array specificato, a partire dall'indice dell'array specificato.

```csharp
public void CopyTo(ExtendedAttribute[] array, int arrayIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| array | ExtendedAttribute[] | l'array monodimensionale specificato a cui copiare gli elementi |
| arrayIndex | Int32 | l'indice basato su zero dell'array specificato al quale inizia la copia. |

## Esempi

Mostra come utilizzare le raccolte di attributi estesi.

```csharp
var project = new Project(DataDir + "ReadTaskExtendedAttributes.mpp");

// Ottieni l'attività all'indice zero
var task = project.RootTask.Children.GetById(1);

if (!task.ExtendedAttributes.IsReadOnly && task.ExtendedAttributes.Count > 0)
{
    // cancella gli attributi estesi
    task.ExtendedAttributes.Clear();
}

// crea la definizione di attributo esteso per un'attività
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

// Aggiungi attributo esteso 1
var extendedAttribute1 = taskDefinition1.CreateExtendedAttribute();
extendedAttribute1.DateValue = new DateTime(2020, 4, 14, 8, 0, 0);
if (task.ExtendedAttributes.IndexOf(extendedAttribute1) < 0)
{
    task.ExtendedAttributes.Insert(0, extendedAttribute1);
}

// Aggiungi attributo esteso 2
var extendedAttribute2 = taskDefinition2.CreateExtendedAttribute();
extendedAttribute2.DateValue = new DateTime(2020, 4, 14, 17, 0, 0);
task.ExtendedAttributes.Add(extendedAttribute2);

// lavora con gli attributi estesi...

// rimuovi l'attributo esteso per indice
task.ExtendedAttributes.RemoveAt(0);

Console.WriteLine("Count of task's extended attributes: " + task.ExtendedAttributes.Count);

// usa l'accesso per indice della raccolta
Console.WriteLine("Attribute 1 Value: " + task.ExtendedAttributes[0].DateValue);

var otherProject = new Project();
var otherTask = otherProject.RootTask.Children.Add("Other task");

// copia gli attributi in un altro progetto
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

// rimuovi tutte le definizioni di attributi estesi
while (otherTask.ExtendedAttributes.Count > 0)
{
    otherTask.ExtendedAttributes.Remove(otherTask.ExtendedAttributes[0]);
}
```

### Vedi anche

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeCollection](../)
* namespace [Aspose.Tasks](../../extendedattributecollection/)
* assembly [Aspose.Tasks](../../../)


