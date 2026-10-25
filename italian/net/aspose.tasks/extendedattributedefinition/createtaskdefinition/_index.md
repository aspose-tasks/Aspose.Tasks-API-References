---
title: "ExtendedAttributeDefinition.CreateTaskDefinition"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "ExtendedAttributeDefinition metodo. Metodo di fabbrica che crea una semplice definizione di attributo esteso che Microsoft Project mostra come None. Ha CalculationType impostato su None e può essere usato solo nei Compiti. È necessario specificare customFieldType, fieldId e alias quando si chiama questo metodo"
type: docs
weight: 40
url: /it/net/aspose.tasks/extendedattributedefinition/createtaskdefinition/
---
## CreateTaskDefinition(CustomFieldType, ExtendedAttributeTask, string) {#createtaskdefinition}

Metodo di fabbrica che crea una semplice definizione di attributo esteso, che Microsoft Project mostra come "None". Ha [`CalculationType`](../calculationtype/) impostato su None e può essere usato solo nei Compiti. È necessario specificare *customFieldType*, *fieldId* e *alias* quando si chiama questo metodo.

```csharp
public static ExtendedAttributeDefinition CreateTaskDefinition(CustomFieldType customFieldType, 
    ExtendedAttributeTask fieldId, string alias)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| customFieldType | CustomFieldType | Il tipo [`CustomFieldType`](../../customfieldtype/) specificato. |
| fieldId | ExtendedAttributeTask | L'ID campo specificato per [`ExtendedAttributeTask`](../../extendedattributetask/). |
| alias | Stringa | L'alias stringa specificato. |

### Valore di ritorno

Istanza creata della classe [`ExtendedAttributeDefinition`](../) con *customFieldType*, *fieldId* e *alias* specificati.

## Esempi

Utilizza questo esempio per creare una definizione di campo di testo personalizzato:

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text27, "My custom field");
project.ExtendedAttributes.Add(taskTextAttr);
```

Mostra come creare gli attributi estesi dell'attività.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// Crea una definizione di attributo esteso di tipo Text1
var taskExtendedAttributeText1Definition =
    ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text1, "Task City Name");

// Aggiungila alla raccolta di Extended Attributes del progetto
project.ExtendedAttributes.Add(taskExtendedAttributeText1Definition);

// Aggiungi un'attività al progetto
var task = project.RootTask.Children.Add("Task 1");

// Crea un Extended Attribute dalla Attribute Definition
var taskExtendedAttributeText1 = taskExtendedAttributeText1Definition.CreateExtendedAttribute();

// Assegna un valore al Extended Attribute generato. Il tipo dell'attributo è "Text", dovrebbe essere utilizzata la proprietà "TextValue".
taskExtendedAttributeText1.TextValue = "London";

// Aggiungi il Extended Attribute all'attività
task.ExtendedAttributes.Add(taskExtendedAttributeText1);

project.Save(OutDir + "PlainTextExtendedAttribute_out.mpp", SaveFileFormat.Mpp);

var project4 = new Project(DataDir + "Blank2010.mpp");

// Crea una Extended Attribute Definition di tipo Text2
var taskExtendedAttributeText2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Text,
    ExtendedAttributeTask.Text2,
    "Task Towns Name");

// Aggiungi valori di ricerca per la definizione di attributo esteso
taskExtendedAttributeText2Definition.AddLookupValue(new Value { Id = 1, StringValue = "Town1", Description = "This is Town1" });
taskExtendedAttributeText2Definition.AddLookupValue(new Value { Id = 2, StringValue = "Town2", Description = "This is Town2" });

// Aggiungila alla raccolta di Extended Attributes del progetto
project4.ExtendedAttributes.Add(taskExtendedAttributeText2Definition);

// Aggiungi un'attività al progetto
var task2 = project4.RootTask.Children.Add("Task 2");

// Crea un Extended Attribute dalla Text2 Lookup Definition per Id 1
var taskExtendedAttributeText2 = taskExtendedAttributeText2Definition.CreateExtendedAttribute(taskExtendedAttributeText2Definition.ValueList[1]);

// Aggiungi il Extended Attribute all'attività
task2.ExtendedAttributes.Add(taskExtendedAttributeText2);

project4.Save(OutDir + "TextExtendedAttributeWithLookup_out.mpp", SaveFileFormat.Mpp);

var project2 = new Project(DataDir + "Blank2010.mpp");

// Crea una Extended Attribute Definition di tipo Duration2
var taskExtendedAttributeDuration2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Duration,
    ExtendedAttributeTask.Duration2,
    "Some duration");

// Aggiungi valori di lookup per la Extended Attribute Definition
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 2, Duration = project2.GetDuration(4, TimeUnitType.Hour), Description = "4 hours" });
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 3, Duration = project2.GetDuration(1, TimeUnitType.Day), Description = "1 day" });
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 4, Duration = project2.GetDuration(1, TimeUnitType.Hour), Description = "1 hour" });
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 7, Duration = project2.GetDuration(10, TimeUnitType.Day), Description = "10 days" });

// Aggiungi la definizione alla raccolta di Extended Attributes del progetto
project2.ExtendedAttributes.Add(taskExtendedAttributeDuration2Definition);

// Aggiungi un'attività al progetto
var task3 = project2.RootTask.Children.Add("Task 3");

// Crea un Extended Attribute dalla Duration2 Lookup Definition per Id 3
var taskExtendedAttributeDuration2 =
    taskExtendedAttributeDuration2Definition.CreateExtendedAttribute(taskExtendedAttributeDuration2Definition.ValueList[3]);

// Aggiungi il Extended Attribute all'attività
task3.ExtendedAttributes.Add(taskExtendedAttributeDuration2);

project2.Save(OutDir + "DurationExtendedAttributeWithLookup_out.mpp", SaveFileFormat.Mpp);

var project3 = new Project(DataDir + "Blank2010.mpp");

// Crea una Extended Attribute Definition di tipo Finish2
var taskExtendedAttributeFinish2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Finish,
    ExtendedAttributeTask.Finish2,
    "Some finish");

// Aggiungi valori di lookup per la Extended Attribute Definition
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 2, DateTimeValue = new DateTime(1984, 01, 01, 00, 00, 01), Description = "This is Value2" });
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 3, DateTimeValue = new DateTime(1994, 01, 01, 00, 01, 01), Description = "This is Value3" });
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 4, DateTimeValue = new DateTime(2009, 12, 31, 00, 00, 00), Description = "This is Value4" });
taskExtendedAttributeFinish2Definition.AddLookupValue(new Value { Id = 7, DateTimeValue = DateTime.Now, Description = "This is Value6" });

// Aggiungi la definizione alla raccolta di Extended Attributes del progetto
project3.ExtendedAttributes.Add(taskExtendedAttributeFinish2Definition);

// Aggiungi un'attività al progetto
var task4 = project3.RootTask.Children.Add("Task 4");

// Crea un Extended Attribute dalla Finish2 Lookup Definition per Id 3
var taskExtendedAttributeFinish2 = taskExtendedAttributeFinish2Definition.CreateExtendedAttribute(taskExtendedAttributeFinish2Definition.ValueList[3]);

// Aggiungi il Extended Attribute all'attività
task4.ExtendedAttributes.Add(taskExtendedAttributeFinish2);

project3.Save(OutDir + "FinishExtendedAttributeWithLookup_out.mpp", SaveFileFormat.Mpp);
```

### Vedi anche

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateTaskDefinition(ExtendedAttributeTask, string) {#createtaskdefinition_1}

Metodo di fabbrica che crea una semplice definizione di attributo esteso, che Microsoft Project mostra come "None". Ha [`CalculationType`](../calculationtype/) impostato su None e può essere usato solo nei Task. È necessario specificare *fieldId* e *alias* quando si chiama questo metodo. Il tipo di campo è dedotto dall'ID campo.

```csharp
public static ExtendedAttributeDefinition CreateTaskDefinition(ExtendedAttributeTask fieldId, 
    string alias)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldId | ExtendedAttributeTask | L'ID campo specificato per [`ExtendedAttributeTask`](../../extendedattributetask/). |
| alias | Stringa | L'alias stringa specificato. |

### Valore di ritorno

Istanza creata della classe [`ExtendedAttributeDefinition`](../) con *fieldId* e *alias* specificati.

## Esempi

Utilizza questo esempio per creare una definizione di campo di testo personalizzato:

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text27, "My custom field");
project.ExtendedAttributes.Add(taskTextAttr);
```

Mostra come creare la definizione di attributo esteso e impostare un valore stringa dell'attributo durante la sua costruzione.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, "My Text");
project.ExtendedAttributes.Add(definition);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 22, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// crea attributo esteso con un valore uguale a 'Common Info'
var extendedAttribute = definition.CreateExtendedAttribute("Common Info");

// aggiungi attributo esteso inizializzato con valore 'Common Info'
task.ExtendedAttributes.Add(extendedAttribute);
```

### Vedi anche

* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


