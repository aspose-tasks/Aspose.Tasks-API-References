---
title: "ExtendedAttributeDefinition.CreateResourceDefinition"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ExtendedAttributeDefinition methode. Fabriekmethode die een eenvoudige definitie van een uitgebreid attribuut maakt die Microsoft Project weergeeft als None. Het heeft CalculationType gelijk aan None en kan alleen in Resource worden gebruikt. U moet customFieldType, fieldId en alias opgeven wanneer u deze methode aanroept."
type: docs
weight: 30
url: /nl/net/aspose.tasks/extendedattributedefinition/createresourcedefinition/
---
## CreateResourceDefinition(CustomFieldType, ExtendedAttributeResource, string) {#createresourcedefinition}

Fabriekmethode die een eenvoudige definitie van een uitgebreid attribuut maakt, die Microsoft Project weergeeft als "None". Het heeft [`CalculationType`](../calculationtype/) gelijk aan None en kan alleen in Resource worden gebruikt. U moet *customFieldType*, *fieldId* en *alias* opgeven wanneer u deze methode aanroept.

```csharp
public static ExtendedAttributeDefinition CreateResourceDefinition(CustomFieldType customFieldType, 
    ExtendedAttributeResource fieldId, string alias)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| customFieldType | CustomFieldType | Het opgegeven [`CustomFieldType`](../../customfieldtype/) type. |
| fieldId | ExtendedAttributeResource | Het opgegeven [`ExtendedAttributeResource`](../../extendedattributeresource/) veld-ID. |
| alias | String | De opgegeven String-alias. |

### Retourwaarde

Aangemaakt exemplaar van de [`ExtendedAttributeDefinition`](../) klasse met opgegeven *customFieldType*, *fieldId* en *alias*.

## Voorbeelden

Gebruik dit voorbeeld om een aangepaste tekstvelddefinitie te maken:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateResourceDefinition(CustomFieldType.Text, ExtendedAttributeResource.Text27, "My custom field");
project.ExtendedAttributes.Add(resourceTextAttr);
```

Toont hoe een uitgebreid attribuut toe te voegen aan een toewijzing van een resource.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// Nieuwe taak en resource toevoegen
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Rsc");
var assignment = project.ResourceAssignments.Add(task, resource);
{
    // Aangepaste attributen die zichtbaar zijn in de weergave "Resource Usage" kunnen worden gemaakt met de ExtendedAttributeDefinition.CreateResourceDefinition‑methode.
    var resCostAttributeDefinition = ExtendedAttributeDefinition.CreateResourceDefinition(
        CustomFieldType.Cost,
        ExtendedAttributeResource.Cost5,
        "My cost");

    project.ExtendedAttributes.Add(resCostAttributeDefinition);

    var value = resCostAttributeDefinition.CreateExtendedAttribute();

    // Het type van het attribuut is "Cost", dus we moeten de "NumericValue"‑eigenschap gebruiken.
    value.NumericValue = 1500;

    assignment.ExtendedAttributes.Add(value);
}

{
    // Aangepaste attributen die zichtbaar zijn in de weergave "Task Usage" kunnen worden gemaakt met de ExtendedAttributeDefinition.CreateTaskDefinition‑methode.
    var taskCostAttributeDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(
        CustomFieldType.Cost,
        ExtendedAttributeTask.Cost5,
        "My cost for task");

    project.ExtendedAttributes.Add(taskCostAttributeDefinition);

    var value = taskCostAttributeDefinition.CreateExtendedAttribute();

    // Het type van het attribuut is "Cost", dus we moeten de "NumericValue"‑eigenschap gebruiken.
    value.NumericValue = 2300;

    assignment.ExtendedAttributes.Add(value);
}

project.Save(OutDir + "AddExtendedAttributesToResourceAssignment_out.mpp", SaveFileFormat.Mpp);
```

### Zie ook

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateResourceDefinition(ExtendedAttributeResource, string) {#createresourcedefinition_1}

Fabriekmethode die een eenvoudige definitie van een uitgebreid attribuut maakt, die Microsoft Project weergeeft als "None". Het heeft [`CalculationType`](../calculationtype/) gelijk aan None en kan alleen in Resource worden gebruikt. U moet *fieldId* en *alias* opgeven wanneer u deze methode aanroept. Het veldtype wordt afgeleid van het veld‑id.

```csharp
public static ExtendedAttributeDefinition CreateResourceDefinition(
    ExtendedAttributeResource fieldId, string alias)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fieldId | ExtendedAttributeResource | Het opgegeven [`ExtendedAttributeResource`](../../extendedattributeresource/) veld-ID. |
| alias | String | De opgegeven String-alias. |

### Retourwaarde

Aangemaakt exemplaar van de [`ExtendedAttributeDefinition`](../) klasse met opgegeven *fieldId* en *alias*.

## Voorbeelden

Gebruik dit voorbeeld om een aangepaste tekstvelddefinitie te maken:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateResourceDefinition(ExtendedAttributeResource.Text27, "My custom field");
project.ExtendedAttributes.Add(resourceTextAttr);
```

Toont hoe een uitgebreide attribuutdefinitie te maken en een vlagwaarde in te stellen tijdens de constructie.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var resource = project.Resources.Add("Resource 1");
resource.Set(Rsc.Type, ResourceType.Cost);

// een definitie maken voor een booleaans aangepast veld
var definition = ExtendedAttributeDefinition.CreateResourceDefinition(ExtendedAttributeResource.Flag7, "My Custom Flag");

// een attribuut maken en de initiële waarde instellen op 'true'
var attribute = definition.CreateExtendedAttribute(true);
resource.ExtendedAttributes.Add(attribute);
```

### Zie ook

* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


