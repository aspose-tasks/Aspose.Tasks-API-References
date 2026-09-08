---
title: "Project.ExtendedAttributes"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad Project. Obtiene el objeto ExtendedAttributeDefinitionCollection. La colección de definiciones de campos personalizados de atributos extendidos asociados a un proyecto"
type: docs
weight: 410
url: /es/net/aspose.tasks/project/extendedattributes/
---
## Project.ExtendedAttributes property

Obtiene el objeto ExtendedAttributeDefinitionCollection. La colección de definiciones de atributos extendidos (campos personalizados) asociados a un proyecto.

```csharp
public ExtendedAttributeDefinitionCollection ExtendedAttributes { get; }
```

## Ejemplos

Muestra cómo trabajar con atributos extendidos.

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

* class [ExtendedAttributeDefinitionCollection](../../extendedattributedefinitioncollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


