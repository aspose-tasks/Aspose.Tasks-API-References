---
title: "ExtendedAttributeDefinition.CreateResourceDefinition"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode ExtendedAttributeDefinition. Méthode d'usine qui crée une définition d'attribut étendu simple que Microsoft Project affiche comme None. Elle a CalculationType égal à None et ne peut être utilisée que dans les Ressources. Vous devez spécifier customFieldType, fieldId et alias lors de l'appel de cette méthode."
type: docs
weight: 30
url: /fr/net/aspose.tasks/extendedattributedefinition/createresourcedefinition/
---
## CreateResourceDefinition(CustomFieldType, ExtendedAttributeResource, string) {#createresourcedefinition}

Méthode d'usine qui crée une définition d'attribut étendu simple, que Microsoft Project affiche comme "None". Elle a [`CalculationType`](../calculationtype/) égal à None et ne peut être utilisée que dans les Ressources. Vous devez spécifier *customFieldType*, *fieldId* et *alias* lors de l'appel de cette méthode.

```csharp
public static ExtendedAttributeDefinition CreateResourceDefinition(CustomFieldType customFieldType, 
    ExtendedAttributeResource fieldId, string alias)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| customFieldType | CustomFieldType | Le type [`CustomFieldType`](../../customfieldtype/) spécifié. |
| fieldId | ExtendedAttributeResource | L'ID de champ spécifié pour [`ExtendedAttributeResource`](../../extendedattributeresource/). |
| alias | Chaîne | L'alias de type String spécifié. |

### Valeur de retour

Instance créée de la classe [`ExtendedAttributeDefinition`](../) avec les *customFieldType*, *fieldId* et *alias* spécifiés.

## Exemples

Utilisez cet exemple pour créer une définition de champ texte personnalisé :

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateResourceDefinition(CustomFieldType.Text, ExtendedAttributeResource.Text27, "My custom field");
project.ExtendedAttributes.Add(resourceTextAttr);
```

Montre comment ajouter un attribut étendu à une affectation de ressource.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// Ajouter une nouvelle tâche et une ressource
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Rsc");
var assignment = project.ResourceAssignments.Add(task, resource);
{
    // Les attributs personnalisés visibles dans la vue "Utilisation des ressources" peuvent être créés avec la méthode ExtendedAttributeDefinition.CreateResourceDefinition.
    var resCostAttributeDefinition = ExtendedAttributeDefinition.CreateResourceDefinition(
        CustomFieldType.Cost,
        ExtendedAttributeResource.Cost5,
        "My cost");

    project.ExtendedAttributes.Add(resCostAttributeDefinition);

    var value = resCostAttributeDefinition.CreateExtendedAttribute();

    // Le type de l'attribut est "Coût", nous devons donc utiliser la propriété "NumericValue".
    value.NumericValue = 1500;

    assignment.ExtendedAttributes.Add(value);
}

{
    // Les attributs personnalisés visibles dans la vue "Utilisation des tâches" peuvent être créés avec la méthode ExtendedAttributeDefinition.CreateTaskDefinition.
    var taskCostAttributeDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(
        CustomFieldType.Cost,
        ExtendedAttributeTask.Cost5,
        "My cost for task");

    project.ExtendedAttributes.Add(taskCostAttributeDefinition);

    var value = taskCostAttributeDefinition.CreateExtendedAttribute();

    // Le type de l'attribut est "Coût", nous devons donc utiliser la propriété "NumericValue".
    value.NumericValue = 2300;

    assignment.ExtendedAttributes.Add(value);
}

project.Save(OutDir + "AddExtendedAttributesToResourceAssignment_out.mpp", SaveFileFormat.Mpp);
```

### Voir aussi

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateResourceDefinition(ExtendedAttributeResource, string) {#createresourcedefinition_1}

Méthode d'usine qui crée une définition d'attribut étendu simple, que Microsoft Project affiche comme "None". Elle a [`CalculationType`](../calculationtype/) égal à None et ne peut être utilisée que dans les Ressources. Vous devez spécifier *fieldId* et *alias* lors de l'appel de cette méthode. Le type de champ est déduit de l'ID du champ.

```csharp
public static ExtendedAttributeDefinition CreateResourceDefinition(
    ExtendedAttributeResource fieldId, string alias)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fieldId | ExtendedAttributeResource | L'ID de champ spécifié pour [`ExtendedAttributeResource`](../../extendedattributeresource/). |
| alias | Chaîne | L'alias de type String spécifié. |

### Valeur de retour

Instance créée de la classe [`ExtendedAttributeDefinition`](../) avec le *fieldId* et l'*alias* spécifiés.

## Exemples

Utilisez cet exemple pour créer une définition de champ texte personnalisé :

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateResourceDefinition(ExtendedAttributeResource.Text27, "My custom field");
project.ExtendedAttributes.Add(resourceTextAttr);
```

Montre comment créer une définition d'attribut étendu et définir la valeur d'un drapeau lors de sa construction.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var resource = project.Resources.Add("Resource 1");
resource.Set(Rsc.Type, ResourceType.Cost);

// créer une définition pour un champ personnalisé booléen
var definition = ExtendedAttributeDefinition.CreateResourceDefinition(ExtendedAttributeResource.Flag7, "My Custom Flag");

// créer un attribut et définir la valeur initiale à 'true'
var attribute = definition.CreateExtendedAttribute(true);
resource.ExtendedAttributes.Add(attribute);
```

### Voir aussi

* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


