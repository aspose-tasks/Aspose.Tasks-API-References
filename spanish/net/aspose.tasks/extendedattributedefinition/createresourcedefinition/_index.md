---
title: "ExtendedAttributeDefinition.CreateResourceDefinition"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método ExtendedAttributeDefinition. Método de fábrica que crea una definición de atributo extendido simple que Microsoft Project muestra como None. Tiene CalculationType igual a None y solo puede usarse en Resource. Se requiere especificar los campos customFieldType, fieldId y alias al llamar a este método."
type: docs
weight: 30
url: /es/net/aspose.tasks/extendedattributedefinition/createresourcedefinition/
---
## CreateResourceDefinition(CustomFieldType, ExtendedAttributeResource, string) {#createresourcedefinition}

Método de fábrica que crea una definición de atributo extendido simple, que Microsoft Project muestra como "None". Tiene [`CalculationType`](../calculationtype/) igual a None y solo puede usarse en Resource. Se requiere especificar *customFieldType*, *fieldId* y *alias* al llamar a este método.

```csharp
public static ExtendedAttributeDefinition CreateResourceDefinition(CustomFieldType customFieldType, 
    ExtendedAttributeResource fieldId, string alias)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| customFieldType | CustomFieldType | El tipo [`CustomFieldType`](../../customfieldtype/) especificado. |
| fieldId | ExtendedAttributeResource | El ID de campo especificado de [`ExtendedAttributeResource`](../../extendedattributeresource/). |
| alias | Cadena | El alias de tipo String especificado. |

### Valor devuelto

Instancia creada de la clase [`ExtendedAttributeDefinition`](../) con *customFieldType*, *fieldId* y *alias* especificados.

## Ejemplos

Utilice este ejemplo para crear una definición de campo de texto personalizado:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateResourceDefinition(CustomFieldType.Text, ExtendedAttributeResource.Text27, "My custom field");
project.ExtendedAttributes.Add(resourceTextAttr);
```

Muestra cómo agregar un atributo extendido a una asignación de recurso.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// Agregar nueva tarea y recurso
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Rsc");
var assignment = project.ResourceAssignments.Add(task, resource);
{
    // Los atributos personalizados que son visibles en la vista "Resource Usage" pueden crearse con el método ExtendedAttributeDefinition.CreateResourceDefinition.
    var resCostAttributeDefinition = ExtendedAttributeDefinition.CreateResourceDefinition(
        CustomFieldType.Cost,
        ExtendedAttributeResource.Cost5,
        "My cost");

    project.ExtendedAttributes.Add(resCostAttributeDefinition);

    var value = resCostAttributeDefinition.CreateExtendedAttribute();

    // El tipo del atributo es "Cost", por lo que necesitamos usar la propiedad "NumericValue".
    value.NumericValue = 1500;

    assignment.ExtendedAttributes.Add(value);
}

{
    // Los atributos personalizados que son visibles en la vista "Task Usage" pueden crearse con el método ExtendedAttributeDefinition.CreateTaskDefinition.
    var taskCostAttributeDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(
        CustomFieldType.Cost,
        ExtendedAttributeTask.Cost5,
        "My cost for task");

    project.ExtendedAttributes.Add(taskCostAttributeDefinition);

    var value = taskCostAttributeDefinition.CreateExtendedAttribute();

    // El tipo del atributo es "Cost", por lo que necesitamos usar la propiedad "NumericValue".
    value.NumericValue = 2300;

    assignment.ExtendedAttributes.Add(value);
}

project.Save(OutDir + "AddExtendedAttributesToResourceAssignment_out.mpp", SaveFileFormat.Mpp);
```

### Ver también

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateResourceDefinition(ExtendedAttributeResource, string) {#createresourcedefinition_1}

Método de fábrica que crea una definición de atributo extendido simple, que Microsoft Project muestra como "None". Tiene [`CalculationType`](../calculationtype/) igual a None y solo puede usarse en Resource. Se requiere especificar *fieldId* y *alias* al llamar a este método. El tipo de campo se infiere del field id.

```csharp
public static ExtendedAttributeDefinition CreateResourceDefinition(
    ExtendedAttributeResource fieldId, string alias)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fieldId | ExtendedAttributeResource | El ID de campo especificado de [`ExtendedAttributeResource`](../../extendedattributeresource/). |
| alias | Cadena | El alias de tipo String especificado. |

### Valor devuelto

Instancia creada de la clase [`ExtendedAttributeDefinition`](../) con *fieldId* y *alias* especificados.

## Ejemplos

Utilice este ejemplo para crear una definición de campo de texto personalizado:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateResourceDefinition(ExtendedAttributeResource.Text27, "My custom field");
project.ExtendedAttributes.Add(resourceTextAttr);
```

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

* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


