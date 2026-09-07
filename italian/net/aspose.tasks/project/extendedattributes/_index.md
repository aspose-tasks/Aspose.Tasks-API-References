---
title: "Project.ExtendedAttributes"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà Project. Ottiene l'oggetto ExtendedAttributeDefinitionCollection. La collezione delle definizioni dei campi personalizzati di attributi estesi associati a un progetto"
type: docs
weight: 410
url: /it/net/aspose.tasks/project/extendedattributes/
---
## Project.ExtendedAttributes property

Ottiene l'oggetto ExtendedAttributeDefinitionCollection. La raccolta delle definizioni di attributi estesi (campi personalizzati) associati a un progetto.

```csharp
public ExtendedAttributeDefinitionCollection ExtendedAttributes { get; }
```

## Esempi

Mostra come lavorare con gli attributi estesi.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var definition = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Text1);

// Se il campo Custom non esiste in Project, crealo
if (definition == null)
{
    definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, "My text field");
    project.ExtendedAttributes.Add(definition);
}

// Genera attributo esteso dalla definizione
var attribute = definition.CreateExtendedAttribute();
attribute.TextValue = "Text attribute value";

// Aggiungi attributo esteso al task
var task = project.RootTask.Children.Add("Task 1");
task.ExtendedAttributes.Add(attribute);

project.Save(OutDir + "CreateExtendedAttributes_out.mpp", SaveFileFormat.Mpp);
```

### Vedi anche

* class [ExtendedAttributeDefinitionCollection](../../extendedattributedefinitioncollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


