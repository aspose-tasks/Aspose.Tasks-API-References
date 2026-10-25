---
title: "Task.ExtendedAttributes"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété Task. Obtient l'objet ExtendedAttributeCollection contenant les valeurs d'un attribut étendu"
type: docs
weight: 400
url: /fr/net/aspose.tasks/task/extendedattributes/
---
## Task.ExtendedAttributes property

Obtient l'objet ExtendedAttributeCollection contenant les valeurs d'un attribut étendu.

```csharp
public ExtendedAttributeCollection ExtendedAttributes { get; }
```

## Remarques

Deux éléments de données sont nécessaires - un pointeur vers la table d'attributs étendus qui est spécifié soit par l'ID unique, soit par l'ID de champ, et la valeur qui est spécifiée soit avec la valeur, soit par un pointeur vers la liste de valeurs.

## Exemples

Montre comment lire les attributs étendus de la tâche.

```csharp
var project = new Project(DataDir + "ReadTaskExtendedAttributes.mpp");

// Créer la définition d'attribut étendu
var definition = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Start, ExtendedAttributeTask.Start7, "Start 7");
project.ExtendedAttributes.Add(definition);

// Obtenir la tâche d'index zéro
var tsk = project.RootTask.Children.GetById(1);

// Ajouter un attribut étendu
var extendedAttribute = definition.CreateExtendedAttribute();
extendedAttribute.DateValue = DateTime.Now;

// Vous pouvez également utiliser la syntaxe courte suivante : ExtendedAttribute attribute = attributeDefinition.CreateExtendedAttribute(DateTime.Now);
tsk.ExtendedAttributes.Add(extendedAttribute);

// Créez une définition d'attribut étendu de type Text1
var taskExtendedAttributeText1Definition =
    ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text1, "Task City Name");

// Ajoutez-le à la collection d'attributs étendus du projet
project.ExtendedAttributes.Add(taskExtendedAttributeText1Definition);

var newTask = project.RootTask.Children.Add("Task 1");

// Créez un attribut étendu à partir de la définition d'attribut
var taskExtendedAttributeText1 = taskExtendedAttributeText1Definition.CreateExtendedAttribute();

// Attribuez une valeur à l'attribut étendu généré. Le type de l'attribut est "Text", la propriété "TextValue" doit être utilisée.
taskExtendedAttributeText1.TextValue = "London";

// Ajoutez l'attribut étendu à la tâche
newTask.ExtendedAttributes.Add(taskExtendedAttributeText1);

// Créez une définition d'attribut étendu de type Text2
var taskExtendedAttributeText2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Text,
    ExtendedAttributeTask.Text2,
    "Task Towns Name");

// Ajouter des valeurs de recherche pour la définition d'attribut étendu
taskExtendedAttributeText2Definition.AddLookupValue(new Value { Id = 1, StringValue = "Town1", Description = "This is Town1" });
taskExtendedAttributeText2Definition.AddLookupValue(new Value { Id = 2, StringValue = "Town2", Description = "This is Town2" });

// Ajoutez-le à la collection d'attributs étendus du projet
project.ExtendedAttributes.Add(taskExtendedAttributeText2Definition);

var task2 = project.RootTask.Children.Add("Task 2");

// Créez un attribut étendu à partir de la définition de recherche Text2 pour l'Id 1
var taskExtendedAttributeText2 = taskExtendedAttributeText2Definition.CreateExtendedAttribute(taskExtendedAttributeText2Definition.ValueList[1]);

// Ajoutez l'attribut étendu à la tâche
task2.ExtendedAttributes.Add(taskExtendedAttributeText2);

// Créez une définition d'attribut étendu de type Duration2
var taskExtendedAttributeDuration2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Duration,
    ExtendedAttributeTask.Duration2,
    "Some duration");

// Ajoutez des valeurs de recherche pour la définition d'attribut étendu
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 3, Duration = project.GetDuration(4, TimeUnitType.Hour), Description = "4 hours" });
taskExtendedAttributeDuration2Definition.AddLookupValue(new Value { Id = 4, Duration = project.GetDuration(1, TimeUnitType.Day), Description = "1 day" });
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 5, Duration = project.GetDuration(1, TimeUnitType.Hour), Description = "1 hour" });
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 6, Duration = project.GetDuration(10, TimeUnitType.Day), Description = "10 days" });

// Ajoutez la définition à la collection d'attributs étendus du projet
project.ExtendedAttributes.Add(taskExtendedAttributeDuration2Definition);

var task3 = project.RootTask.Children.Add("Task 3");

// Créez un attribut étendu à partir de la définition de recherche Duration2 pour l'Id 3
var taskExtendedAttributeDuration2 =
    taskExtendedAttributeDuration2Definition.CreateExtendedAttribute(taskExtendedAttributeDuration2Definition.ValueList[3]);

// Ajoutez l'attribut étendu à la tâche
task3.ExtendedAttributes.Add(taskExtendedAttributeDuration2);

// Créez une définition d'attribut étendu de type Finish2
var taskExtendedAttributeFinish2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Finish,
    ExtendedAttributeTask.Finish2,
    "Some finish");

// Ajoutez des valeurs de recherche pour la définition d'attribut étendu
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 7, DateTimeValue = new DateTime(1984, 01, 01, 00, 00, 01), Description = "This is Value2" });
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 8, DateTimeValue = new DateTime(1994, 01, 01, 00, 01, 01), Description = "This is Value3" });
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 9, DateTimeValue = new DateTime(2009, 12, 31, 00, 00, 00), Description = "This is Value4" });
taskExtendedAttributeFinish2Definition.AddLookupValue(new Value { Id = 10, DateTimeValue = DateTime.Now, Description = "This is Value6" });

// Ajoutez la définition à la collection d'attributs étendus du projet
project.ExtendedAttributes.Add(taskExtendedAttributeFinish2Definition);

var task4 = project.RootTask.Children.Add("Task 4");

// Créez un attribut étendu à partir de la définition de recherche Finish2 pour l'Id 3
var taskExtendedAttributeFinish2 = taskExtendedAttributeFinish2Definition.CreateExtendedAttribute(taskExtendedAttributeFinish2Definition.ValueList[3]);

// Ajoutez l'attribut étendu à la tâche
task4.ExtendedAttributes.Add(taskExtendedAttributeFinish2);

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Lire les attributs étendus pour les tâches
foreach (var task in collector.Tasks)
{
    foreach (var attribute in task.ExtendedAttributes)
    {
        Console.WriteLine(attribute.FieldId);
        Console.WriteLine(attribute.ValueGuid);

        switch (attribute.AttributeDefinition.CfType)
        {
            case CustomFieldType.Date:
            case CustomFieldType.Start:
            case CustomFieldType.Finish:
                Console.WriteLine(attribute.DateValue);
                break;
            case CustomFieldType.Text:
                Console.WriteLine(attribute.TextValue);
                break;
            case CustomFieldType.Duration:
                Console.WriteLine(attribute.DurationValue.ToString());
                break;
            case CustomFieldType.Cost:
            case CustomFieldType.Number:
                Console.WriteLine(attribute.NumericValue);
                break;
            case CustomFieldType.Flag:
                Console.WriteLine(attribute.FlagValue);
                break;
            case CustomFieldType.Null:
            case CustomFieldType.RBS:
            case CustomFieldType.OutlineCode:
                return;
            default:
                return;
        }
    }
}

project.Save(OutDir + "ReadWriteTaskExtendedAttributes_out.mpp", SaveFileFormat.Mpp);
```

### Voir aussi

* class [ExtendedAttributeCollection](../../extendedattributecollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


