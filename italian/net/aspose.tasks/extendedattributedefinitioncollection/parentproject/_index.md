---
title: "ExtendedAttributeDefinitionCollection.ParentProject"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà ExtendedAttributeDefinitionCollection. Restituisce un progetto genitore per l'istanza di ExtendedAttributeDefinitionCollection. restituisce un progetto genitore per questa collezione"
type: docs
weight: 40
url: /it/net/aspose.tasks/extendedattributedefinitioncollection/parentproject/
---
## ExtendedAttributeDefinitionCollection.ParentProject property

Restituisce un progetto genitore per l'istanza di [`ExtendedAttributeDefinitionCollection`](../). restituisce un progetto genitore per questa collezione.

```csharp
public Project ParentProject { get; }
```

## Esempi

Mostra come utilizzare le collezioni di definizioni di attributi estesi.

```csharp
var project = new Project(DataDir + "ReadTaskExtendedAttributes.mpp");

if (!project.ExtendedAttributes.IsReadOnly)
{
    if (project.ExtendedAttributes.Count > 0)
    {
        // cancella le definizioni di attributi estesi
        project.ExtendedAttributes.Clear();
    }
}

// crea la definizione di attributo esteso per un'attività
var taskDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Start, ExtendedAttributeTask.Start7, "Start 7");
project.ExtendedAttributes.Add(taskDefinition);

Console.WriteLine("Iterate over extended attributes of " + project.ExtendedAttributes.ParentProject.Get(Prj.Name) + " project: ");
foreach (var attribute in project.ExtendedAttributes)
{
    Console.WriteLine("Attribute Alias: " + attribute.Alias);
    Console.WriteLine("Attribute CfType: " + attribute.CfType);
    Console.WriteLine();
}

Console.WriteLine();

// lavora con le definizioni di attributi estesi...
var resourceDefinition = ExtendedAttributeDefinition.CreateResourceDefinition(CustomFieldType.Cost, ExtendedAttributeResource.Cost5, "My cost");

if (!project.ExtendedAttributes.Contains(resourceDefinition))
{
    project.ExtendedAttributes.Add(resourceDefinition);
}

// lavora con le definizioni di attributi estesi...
var resourceDefinition2 = ExtendedAttributeDefinition.CreateResourceDefinition(CustomFieldType.Number, ExtendedAttributeResource.Cost1, "My Cost 2");

if (project.ExtendedAttributes.IndexOf(resourceDefinition2) < 0)
{
    project.ExtendedAttributes.Insert(0, resourceDefinition2);
}

// lavora con le definizioni di attributi estesi...

// rimuovi l'attributo esteso per indice
project.ExtendedAttributes.RemoveAt(0);

Console.WriteLine("Print project's extended attributes: ");
Console.WriteLine("Count of project's extended attribute definitions: " + project.ExtendedAttributes.Count);

// usa l'accesso per indice della raccolta
Console.WriteLine("Attribute 1 Alias: " + project.ExtendedAttributes[0].Alias);
Console.WriteLine("Attribute 1 CfType: " + project.ExtendedAttributes[0].CfType);
Console.WriteLine("Attribute 2 Alias: " + project.ExtendedAttributes[1].Alias);
Console.WriteLine("Attribute 2 CfType: " + project.ExtendedAttributes[1].CfType);

var otherProject = new Project();

// copia gli attributi in un altro progetto
var attributes = new ExtendedAttributeDefinition[project.ExtendedAttributes.Count];
project.ExtendedAttributes.CopyTo(attributes, 0);

foreach (var attribute in attributes)
{
    otherProject.ExtendedAttributes.Add(attribute);
}

Console.WriteLine();
Console.WriteLine("Iterate over other project's extended attributes: ");
foreach (var attribute in otherProject.ExtendedAttributes)
{
    Console.WriteLine("Attribute Alias: " + attribute.Alias);
    Console.WriteLine("Attribute CfType: " + attribute.CfType);
    Console.WriteLine();
}

// rimuovi tutte le definizioni di attributi estesi
List<ExtendedAttributeDefinition> definitions = project.ExtendedAttributes.ToList();
foreach (var definition in definitions)
{
    project.ExtendedAttributes.Remove(definition);
}
```

### Vedi anche

* class [Project](../../project/)
* class [ExtendedAttributeDefinitionCollection](../)
* namespace [Aspose.Tasks](../../extendedattributedefinitioncollection/)
* assembly [Aspose.Tasks](../../../)


