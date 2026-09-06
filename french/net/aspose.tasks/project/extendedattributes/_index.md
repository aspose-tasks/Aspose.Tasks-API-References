---
title: "Project.ExtendedAttributes"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété Project. Obtient l'objet ExtendedAttributeDefinitionCollection. La collection des définitions de champs personnalisés d'attributs étendus associés à un projet"
type: docs
weight: 410
url: /fr/net/aspose.tasks/project/extendedattributes/
---
## Project.ExtendedAttributes property

Obtient l'objet ExtendedAttributeDefinitionCollection. La collection des définitions d'attributs étendus (champs personnalisés) associées à un projet.

```csharp
public ExtendedAttributeDefinitionCollection ExtendedAttributes { get; }
```

## Exemples

Montre comment travailler avec les attributs étendus.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var definition = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Text1);

// Si le champ personnalisé n'existe pas dans le projet, créez-le
if (definition == null)
{
    definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, "My text field");
    project.ExtendedAttributes.Add(definition);
}

// Générer un attribut étendu à partir de la définition
var attribute = definition.CreateExtendedAttribute();
attribute.TextValue = "Text attribute value";

// Ajouter un attribut étendu à la tâche
var task = project.RootTask.Children.Add("Task 1");
task.ExtendedAttributes.Add(attribute);

project.Save(OutDir + "CreateExtendedAttributes_out.mpp", SaveFileFormat.Mpp);
```

### Voir aussi

* class [ExtendedAttributeDefinitionCollection](../../extendedattributedefinitioncollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


