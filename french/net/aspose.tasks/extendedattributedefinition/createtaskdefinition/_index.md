---
title: "ExtendedAttributeDefinition.CreateTaskDefinition"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode ExtendedAttributeDefinition. Méthode d'usine qui crée une définition d'attribut étendu simple que Microsoft Project affiche comme None. Elle a CalculationType égal à None et ne peut être utilisée que dans Tasks. Vous devez spécifier customFieldType, fieldId et alias lors de l'appel de cette méthode."
type: docs
weight: 40
url: /fr/net/aspose.tasks/extendedattributedefinition/createtaskdefinition/
---
## CreateTaskDefinition(CustomFieldType, ExtendedAttributeTask, string) {#createtaskdefinition}

Méthode d'usine qui crée une définition d'attribut étendu simple, que Microsoft Project affiche comme "None". Elle a [`CalculationType`](../calculationtype/) égal à None et ne peut être utilisée que dans Tasks. Vous devez spécifier *customFieldType*, *fieldId* et *alias* lors de l'appel de cette méthode.

```csharp
public static ExtendedAttributeDefinition CreateTaskDefinition(CustomFieldType customFieldType, 
    ExtendedAttributeTask fieldId, string alias)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| customFieldType | CustomFieldType | Le type [`CustomFieldType`](../../customfieldtype/) spécifié. |
| fieldId | ExtendedAttributeTask | L'ID de champ spécifié [`ExtendedAttributeTask`](../../extendedattributetask/). |
| alias | Chaîne | L'alias de type String spécifié. |

### Valeur de retour

Instance créée de la classe [`ExtendedAttributeDefinition`](../) avec les *customFieldType*, *fieldId* et *alias* spécifiés.

## Exemples

Utilisez cet exemple pour créer une définition de champ texte personnalisé :

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text27, "My custom field");
project.ExtendedAttributes.Add(taskTextAttr);
```

Montre comment créer les attributs étendus d'une tâche.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// Créez une définition d'attribut étendu de type Text1
var taskExtendedAttributeText1Definition =
    ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text1, "Task City Name");

// Ajoutez-le à la collection d'attributs étendus du projet
project.ExtendedAttributes.Add(taskExtendedAttributeText1Definition);

// Ajoutez une tâche au projet
var task = project.RootTask.Children.Add("Task 1");

// Créez un attribut étendu à partir de la définition d'attribut
var taskExtendedAttributeText1 = taskExtendedAttributeText1Definition.CreateExtendedAttribute();

// Attribuez une valeur à l'attribut étendu généré. Le type de l'attribut est "Text", la propriété "TextValue" doit être utilisée.
taskExtendedAttributeText1.TextValue = "London";

// Ajoutez l'attribut étendu à la tâche
task.ExtendedAttributes.Add(taskExtendedAttributeText1);

project.Save(OutDir + "PlainTextExtendedAttribute_out.mpp", SaveFileFormat.Mpp);

var project4 = new Project(DataDir + "Blank2010.mpp");

// Créez une définition d'attribut étendu de type Text2
var taskExtendedAttributeText2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Text,
    ExtendedAttributeTask.Text2,
    "Task Towns Name");

// Ajouter des valeurs de recherche pour la définition d'attribut étendu
taskExtendedAttributeText2Definition.AddLookupValue(new Value { Id = 1, StringValue = "Town1", Description = "This is Town1" });
taskExtendedAttributeText2Definition.AddLookupValue(new Value { Id = 2, StringValue = "Town2", Description = "This is Town2" });

// Ajoutez-le à la collection d'attributs étendus du projet
project4.ExtendedAttributes.Add(taskExtendedAttributeText2Definition);

// Ajoutez une tâche au projet
var task2 = project4.RootTask.Children.Add("Task 2");

// Créez un attribut étendu à partir de la définition de recherche Text2 pour l'Id 1
var taskExtendedAttributeText2 = taskExtendedAttributeText2Definition.CreateExtendedAttribute(taskExtendedAttributeText2Definition.ValueList[1]);

// Ajoutez l'attribut étendu à la tâche
task2.ExtendedAttributes.Add(taskExtendedAttributeText2);

project4.Save(OutDir + "TextExtendedAttributeWithLookup_out.mpp", SaveFileFormat.Mpp);

var project2 = new Project(DataDir + "Blank2010.mpp");

// Créez une définition d'attribut étendu de type Duration2
var taskExtendedAttributeDuration2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Duration,
    ExtendedAttributeTask.Duration2,
    "Some duration");

// Ajoutez des valeurs de recherche pour la définition d'attribut étendu
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 2, Duration = project2.GetDuration(4, TimeUnitType.Hour), Description = "4 hours" });
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 3, Duration = project2.GetDuration(1, TimeUnitType.Day), Description = "1 day" });
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 4, Duration = project2.GetDuration(1, TimeUnitType.Hour), Description = "1 hour" });
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 7, Duration = project2.GetDuration(10, TimeUnitType.Day), Description = "10 days" });

// Ajoutez la définition à la collection d'attributs étendus du projet
project2.ExtendedAttributes.Add(taskExtendedAttributeDuration2Definition);

// Ajoutez une tâche au projet
var task3 = project2.RootTask.Children.Add("Task 3");

// Créez un attribut étendu à partir de la définition de recherche Duration2 pour l'Id 3
var taskExtendedAttributeDuration2 =
    taskExtendedAttributeDuration2Definition.CreateExtendedAttribute(taskExtendedAttributeDuration2Definition.ValueList[3]);

// Ajoutez l'attribut étendu à la tâche
task3.ExtendedAttributes.Add(taskExtendedAttributeDuration2);

project2.Save(OutDir + "DurationExtendedAttributeWithLookup_out.mpp", SaveFileFormat.Mpp);

var project3 = new Project(DataDir + "Blank2010.mpp");

// Créez une définition d'attribut étendu de type Finish2
var taskExtendedAttributeFinish2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Finish,
    ExtendedAttributeTask.Finish2,
    "Some finish");

// Ajoutez des valeurs de recherche pour la définition d'attribut étendu
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 2, DateTimeValue = new DateTime(1984, 01, 01, 00, 00, 01), Description = "This is Value2" });
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 3, DateTimeValue = new DateTime(1994, 01, 01, 00, 01, 01), Description = "This is Value3" });
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 4, DateTimeValue = new DateTime(2009, 12, 31, 00, 00, 00), Description = "This is Value4" });
taskExtendedAttributeFinish2Definition.AddLookupValue(new Value { Id = 7, DateTimeValue = DateTime.Now, Description = "This is Value6" });

// Ajoutez la définition à la collection d'attributs étendus du projet
project3.ExtendedAttributes.Add(taskExtendedAttributeFinish2Definition);

// Ajoutez une tâche au projet
var task4 = project3.RootTask.Children.Add("Task 4");

// Créez un attribut étendu à partir de la définition de recherche Finish2 pour l'Id 3
var taskExtendedAttributeFinish2 = taskExtendedAttributeFinish2Definition.CreateExtendedAttribute(taskExtendedAttributeFinish2Definition.ValueList[3]);

// Ajoutez l'attribut étendu à la tâche
task4.ExtendedAttributes.Add(taskExtendedAttributeFinish2);

project3.Save(OutDir + "FinishExtendedAttributeWithLookup_out.mpp", SaveFileFormat.Mpp);
```

### Voir aussi

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateTaskDefinition(ExtendedAttributeTask, string) {#createtaskdefinition_1}

Méthode d'usine qui crée une définition d'attribut étendu simple, affichée par Microsoft Project comme "None". Elle possède [`CalculationType`](../calculationtype/) égal à None et ne peut être utilisée que dans les tâches. Vous devez spécifier *fieldId* et *alias* lors de l'appel de cette méthode. Le type de champ est déduit de l'ID de champ.

```csharp
public static ExtendedAttributeDefinition CreateTaskDefinition(ExtendedAttributeTask fieldId, 
    string alias)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fieldId | ExtendedAttributeTask | L'ID de champ spécifié [`ExtendedAttributeTask`](../../extendedattributetask/). |
| alias | Chaîne | L'alias de type String spécifié. |

### Valeur de retour

Instance créée de la classe [`ExtendedAttributeDefinition`](../) avec le *fieldId* et l'*alias* spécifiés.

## Exemples

Utilisez cet exemple pour créer une définition de champ texte personnalisé :

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text27, "My custom field");
project.ExtendedAttributes.Add(taskTextAttr);
```

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

* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


