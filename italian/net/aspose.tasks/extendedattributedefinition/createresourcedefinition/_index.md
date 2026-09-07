---
title: "ExtendedAttributeDefinition.CreateResourceDefinition"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo ExtendedAttributeDefinition. Metodo di fabbrica che crea una definizione di attributo esteso semplice che Microsoft Project visualizza come None. Ha CalculationType impostato su None e può essere utilizzato solo nelle Risorse. È necessario specificare customFieldType, fieldId e alias quando si chiama questo metodo."
type: docs
weight: 30
url: /it/net/aspose.tasks/extendedattributedefinition/createresourcedefinition/
---
## CreateResourceDefinition(CustomFieldType, ExtendedAttributeResource, string) {#createresourcedefinition}

Metodo di fabbrica che crea una definizione di attributo esteso semplice, che Microsoft Project visualizza come "None". Ha [`CalculationType`](../calculationtype/) impostato su None e può essere utilizzato solo nelle Risorse. È necessario specificare *customFieldType*, *fieldId* e *alias* quando si chiama questo metodo.

```csharp
public static ExtendedAttributeDefinition CreateResourceDefinition(CustomFieldType customFieldType, 
    ExtendedAttributeResource fieldId, string alias)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| customFieldType | CustomFieldType | Il tipo [`CustomFieldType`](../../customfieldtype/) specificato. |
| fieldId | ExtendedAttributeResource | L'ID campo specificato per [`ExtendedAttributeResource`](../../extendedattributeresource/). |
| alias | Stringa | L'alias stringa specificato. |

### Valore di ritorno

Istanza creata della classe [`ExtendedAttributeDefinition`](../) con *customFieldType*, *fieldId* e *alias* specificati.

## Esempi

Utilizza questo esempio per creare una definizione di campo di testo personalizzato:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateResourceDefinition(CustomFieldType.Text, ExtendedAttributeResource.Text27, "My custom field");
project.ExtendedAttributes.Add(resourceTextAttr);
```

Mostra come aggiungere un attributo esteso a un'assegnazione di risorsa.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// Aggiungi nuovo compito e risorsa
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Rsc");
var assignment = project.ResourceAssignments.Add(task, resource);
{
    // Gli attributi personalizzati visibili nella visualizzazione "Resource Usage" possono essere creati con il metodo ExtendedAttributeDefinition.CreateResourceDefinition.
    var resCostAttributeDefinition = ExtendedAttributeDefinition.CreateResourceDefinition(
        CustomFieldType.Cost,
        ExtendedAttributeResource.Cost5,
        "My cost");

    project.ExtendedAttributes.Add(resCostAttributeDefinition);

    var value = resCostAttributeDefinition.CreateExtendedAttribute();

    // Il tipo dell'attributo è "Cost", quindi dobbiamo usare la proprietà "NumericValue".
    value.NumericValue = 1500;

    assignment.ExtendedAttributes.Add(value);
}

{
    // Gli attributi personalizzati visibili nella visualizzazione "Task Usage" possono essere creati con il metodo ExtendedAttributeDefinition.CreateTaskDefinition.
    var taskCostAttributeDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(
        CustomFieldType.Cost,
        ExtendedAttributeTask.Cost5,
        "My cost for task");

    project.ExtendedAttributes.Add(taskCostAttributeDefinition);

    var value = taskCostAttributeDefinition.CreateExtendedAttribute();

    // Il tipo dell'attributo è "Cost", quindi dobbiamo usare la proprietà "NumericValue".
    value.NumericValue = 2300;

    assignment.ExtendedAttributes.Add(value);
}

project.Save(OutDir + "AddExtendedAttributesToResourceAssignment_out.mpp", SaveFileFormat.Mpp);
```

### Vedi anche

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateResourceDefinition(ExtendedAttributeResource, string) {#createresourcedefinition_1}

Metodo di fabbrica che crea una definizione di attributo esteso semplice, che Microsoft Project visualizza come "None". Ha [`CalculationType`](../calculationtype/) impostato su None e può essere utilizzato solo nelle Risorse. È necessario specificare *fieldId* e *alias* quando si chiama questo metodo. Il tipo di campo è dedotto dall'ID del campo.

```csharp
public static ExtendedAttributeDefinition CreateResourceDefinition(
    ExtendedAttributeResource fieldId, string alias)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldId | ExtendedAttributeResource | L'ID campo specificato per [`ExtendedAttributeResource`](../../extendedattributeresource/). |
| alias | Stringa | L'alias stringa specificato. |

### Valore di ritorno

Istanza creata della classe [`ExtendedAttributeDefinition`](../) con *fieldId* e *alias* specificati.

## Esempi

Utilizza questo esempio per creare una definizione di campo di testo personalizzato:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateResourceDefinition(ExtendedAttributeResource.Text27, "My custom field");
project.ExtendedAttributes.Add(resourceTextAttr);
```

Mostra come creare la definizione di attributo esteso e impostare il valore di un flag durante la sua costruzione.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var resource = project.Resources.Add("Resource 1");
resource.Set(Rsc.Type, ResourceType.Cost);

// creare una definizione per un campo personalizzato booleano
var definition = ExtendedAttributeDefinition.CreateResourceDefinition(ExtendedAttributeResource.Flag7, "My Custom Flag");

// creare un attributo e impostare il valore iniziale su 'true'
var attribute = definition.CreateExtendedAttribute(true);
resource.ExtendedAttributes.Add(attribute);
```

### Vedi anche

* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


