---
title: "ExtendedAttributeDefinition.CreateExtendedAttribute"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode ExtendedAttributeDefinition. Crée un nouvel attribut étendu avec l'ID de champ qui est égal à la valeur de l'ID de champ de cet objet"
type: docs
weight: 310
url: /fr/net/aspose.tasks/extendedattributedefinition/createextendedattribute/
---
## CreateExtendedAttribute() {#createextendedattribute}

Crée un nouvel attribut étendu avec l'ID de champ qui est égal à la valeur de l'ID de champ de cet objet.

```csharp
public ExtendedAttribute CreateExtendedAttribute()
```

### Valeur de retour

renvoie l'instance créée de la classe [`ExtendedAttribute`](../../extendedattribute/) avec le fieldID qui est égal à la valeur du fieldID de cet objet.

## Exemples

Montre comment créer des attributs étendus.

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

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(string) {#createextendedattribute_6}

Crée un nouvel attribut étendu avec l'ID de champ qui est égal à la valeur de l'ID de champ de cet objet et la valeur de texte spécifiée.

```csharp
public ExtendedAttribute CreateExtendedAttribute(string textValue)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| textValue | Chaîne | La valeur texte spécifiée. |

### Valeur de retour

renvoie l'instance créée de la classe [`ExtendedAttribute`](../../extendedattribute/) avec le fieldID qui est égal à la valeur du fieldID de cet objet.

### Exceptions

| exception | condition |
| --- | --- |
| InvalidOperationException | Si le [`CfType`](../cftype/) actuel n'est pas « Text » |

## Exemples

Montre comment créer une définition d'attribut étendu et définir une valeur chaîne de l'attribut lors de sa construction.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, "My Text");
project.ExtendedAttributes.Add(definition);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 22, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// créer un attribut étendu avec une valeur égale à « Common Info »
var extendedAttribute = definition.CreateExtendedAttribute("Common Info");

// ajouter un attribut étendu initialisé avec la valeur « Common Info »
task.ExtendedAttributes.Add(extendedAttribute);
```

### Voir aussi

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(decimal) {#createextendedattribute_5}

Crée un nouvel attribut étendu avec l'ID de champ qui est égal à la valeur de l'ID de champ de cet objet et la valeur numérique spécifiée.

```csharp
public ExtendedAttribute CreateExtendedAttribute(decimal numericValue)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| numericValue | Decimal | La valeur numérique spécifiée. |

### Valeur de retour

renvoie l'instance créée de la classe [`ExtendedAttribute`](../../extendedattribute/) avec le fieldID qui est égal à la valeur du fieldID de cet objet.

### Exceptions

| exception | condition |
| --- | --- |
| InvalidOperationException | Si le [`CfType`](../cftype/) actuel n'est pas « Number » ou « Cost » |

## Exemples

Montre comment créer une définition d'attribut étendu et définir une valeur décimale de l'attribut lors de sa construction.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Cost1, "My Cost");
project.ExtendedAttributes.Add(definition);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 22, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// créer un attribut étendu avec une valeur égale à 999m 
var extendedAttribute = definition.CreateExtendedAttribute(999m);

// ajouter un attribut étendu initialisé avec la valeur 999m
task.ExtendedAttributes.Add(extendedAttribute);
```

### Voir aussi

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(DateTime) {#createextendedattribute_4}

Crée un nouvel attribut étendu avec l'ID de champ qui est égal à la valeur de l'ID de champ de cet objet et la valeur de date spécifiée.

```csharp
public ExtendedAttribute CreateExtendedAttribute(DateTime dateTimeValue)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| dateTimeValue | DateTime | La valeur de date et d'heure spécifiée. |

### Valeur de retour

renvoie l'instance créée de la classe [`ExtendedAttribute`](../../extendedattribute/) avec le fieldID qui est égal à la valeur du fieldID de cet objet.

### Exceptions

| exception | condition |
| --- | --- |
| InvalidOperationException | Si le [`CfType`](../cftype/) actuel n'est pas « Date », « Start » ou « Finish » |

## Exemples

Montre comment créer une définition d'attribut étendu et définir une valeur de date et heure de l'attribut lors de sa construction.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var definitionWithDate = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Date1, "My Date");
project.ExtendedAttributes.Add(definitionWithDate);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 22, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// crée un attribut étendu avec une valeur égale à DateTime.Now 
var extendedAttribute = definitionWithDate.CreateExtendedAttribute(DateTime.Now);

// ajouter un attribut étendu
task.ExtendedAttributes.Add(extendedAttribute);
```

### Voir aussi

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(Duration) {#createextendedattribute_1}

Crée un nouvel attribut étendu avec l'ID de champ qui est égal à la valeur de l'ID de champ de cet objet et la valeur de durée spécifiée.

```csharp
public ExtendedAttribute CreateExtendedAttribute(Duration durationValue)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| durationValue | Duration | La valeur de durée spécifiée. |

### Valeur de retour

renvoie l'instance créée de la classe [`ExtendedAttribute`](../../extendedattribute/) avec le fieldID qui est égal à la valeur du fieldID de cet objet.

### Exceptions

| exception | condition |
| --- | --- |
| InvalidOperationException | Si le [`CfType`](../cftype/) actuel n'est pas « Duration » |

## Exemples

Montre comment créer une définition d'attribut étendu et définir une durée lors de sa construction.

```csharp
var project = new Project(DataDir + "Project2.mpp");
var task = project.RootTask.Children.Add("Test");
task.Set(Tsk.Start, new DateTime(2020, 4, 22, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Duration1, "Custom Duration");
project.ExtendedAttributes.Add(definition);

// attribut étendu Duration1 = 2 jours
var extendedAttribute = definition.CreateExtendedAttribute(project.GetDuration(2, TimeUnitType.Day));

// ajouter un attribut étendu à la tâche
task.ExtendedAttributes.Add(extendedAttribute);
```

### Voir aussi

* class [ExtendedAttribute](../../extendedattribute/)
* struct [Duration](../../duration/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(bool) {#createextendedattribute_3}

Crée un nouvel attribut étendu avec l'ID de champ qui est égal à la valeur de l'ID de champ de cet objet et la valeur de drapeau spécifiée.

```csharp
public ExtendedAttribute CreateExtendedAttribute(bool flagValue)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| flagValue | Boolean | La valeur de drapeau spécifiée. |

### Valeur de retour

renvoie l'instance créée de la classe [`ExtendedAttribute`](../../extendedattribute/) avec le fieldID qui est égal à la valeur du fieldID de cet objet.

### Exceptions

| exception | condition |
| --- | --- |
| InvalidOperationException | Si le [`CfType`](../cftype/) actuel n'est pas « Flag » |

## Exemples

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

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(Value) {#createextendedattribute_2}

Crée un nouvel attribut étendu lié à l'élément [`Value`](../../value/) spécifié.

```csharp
public ExtendedAttribute CreateExtendedAttribute(Value lookupValue)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| lookupValue | Value | L'élément [`Value`](../../value/) spécifié. |

### Valeur de retour

renvoie l'instance créée de la classe [`ExtendedAttribute`](../../extendedattribute/) liée à l'élément [`Value`](../../value/) spécifié.

## Remarques

*lookupValue* should be previously added to the [`ExtendedAttributeDefinition`](../) using [`AddLookupValue`](../addlookupvalue/) method.

## Exemples

Utilisez ce code pour créer un nouveau [`ExtendedAttribute`](../../extendedattribute/) en utilisant une valeur spécifique :

```csharp
taskTextAttr.AddLookupValue(value1);
taskTextAttr.AddLookupValue(value2);
var extendedAttribute = taskTextAttr.CreateExtendedAttribute(value2);
```

Montre comment créer une définition d'attribut étendu et définir une valeur lors de sa construction.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// Créez une définition de champ personnalisé basée sur la table de correspondance, qui a été déclarée ci‑dessus.
var customFieldDefinition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(CustomFieldType.Number, ExtendedAttributeTask.Number10, "Status");

var value1 = new Value { Id = 1, Val = "25", Description = "Active" };
var value2 = new Value { Id = 2, Val = "12", Description = "Inactive" };
customFieldDefinition.AddLookupValue(value1);
customFieldDefinition.AddLookupValue(value2);
project.ExtendedAttributes.Add(customFieldDefinition);

var task = project.RootTask.Children.Add("Task");

// crée un attribut étendu pour une valeur 
var extendedAttribute = customFieldDefinition.CreateExtendedAttribute(value2);

// ajouter un attribut étendu à la tâche
task.ExtendedAttributes.Add(extendedAttribute);
```

### Voir aussi

* class [ExtendedAttribute](../../extendedattribute/)
* class [Value](../../value/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


