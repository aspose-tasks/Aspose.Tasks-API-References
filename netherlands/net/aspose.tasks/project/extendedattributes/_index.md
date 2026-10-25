---
title: "Project.ExtendedAttributes"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Projecteigenschap. Haalt het ExtendedAttributeDefinitionCollection-object op. De collectie van definities van aangepaste velden voor uitgebreide attributen die aan een project zijn gekoppeld."
type: docs
weight: 410
url: /nl/net/aspose.tasks/project/extendedattributes/
---
## Project.ExtendedAttributes property

Haalt het ExtendedAttributeDefinitionCollection‑object op. De verzameling van definities van uitgebreide attributen (aangepaste velden) die aan een project zijn gekoppeld.

```csharp
public ExtendedAttributeDefinitionCollection ExtendedAttributes { get; }
```

## Voorbeelden

Toont hoe te werken met uitgebreide attributen.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var definition = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Text1);

// Als het aangepaste veld niet bestaat in Project, maak het dan aan.
if (definition == null)
{
    definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, "My text field");
    project.ExtendedAttributes.Add(definition);
}

// Genereer uitgebreid attribuut vanuit definitie
var attribute = definition.CreateExtendedAttribute();
attribute.TextValue = "Text attribute value";

// Voeg uitgebreid attribuut toe aan taak
var task = project.RootTask.Children.Add("Task 1");
task.ExtendedAttributes.Add(attribute);

project.Save(OutDir + "CreateExtendedAttributes_out.mpp", SaveFileFormat.Mpp);
```

### Zie ook

* class [ExtendedAttributeDefinitionCollection](../../extendedattributedefinitioncollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


