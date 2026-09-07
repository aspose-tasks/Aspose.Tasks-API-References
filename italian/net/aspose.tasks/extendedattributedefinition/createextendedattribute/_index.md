---
title: "ExtendedAttributeDefinition.CreateExtendedAttribute"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "ExtendedAttributeDefinition metodo. Crea un nuovo attributo esteso con l'ID campo che è uguale al valore dell'ID campo di questo oggetto"
type: docs
weight: 310
url: /it/net/aspose.tasks/extendedattributedefinition/createextendedattribute/
---
## CreateExtendedAttribute() {#createextendedattribute}

Crea un nuovo attributo esteso con l'ID campo che è uguale al valore dell'ID campo di questo oggetto.

```csharp
public ExtendedAttribute CreateExtendedAttribute()
```

### Valore di ritorno

restituisce l'istanza creata della classe [`ExtendedAttribute`](../../extendedattribute/) con il fieldID che è uguale al valore del fieldID di questo oggetto.

## Esempi

Mostra come creare attributi estesi.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var definition = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Text1);

// Se il campo Custom non esiste in Project, crealo
if (definition == null)
{
    definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, "My text field");
    project.ExtendedAttributes.Add(definition);
}

// Genera attributo esteso dalla definizione
var attribute = definition.CreateExtendedAttribute();
attribute.TextValue = "Text attribute value";

// Aggiungi attributo esteso al task
var task = project.RootTask.Children.Add("Task 1");
task.ExtendedAttributes.Add(attribute);

project.Save(OutDir + "CreateExtendedAttributes_out.mpp", SaveFileFormat.Mpp);
```

### Vedi anche

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(string) {#createextendedattribute_6}

Crea un nuovo attributo esteso con l'ID campo che è uguale al valore dell'ID campo di questo oggetto e al valore del testo specificato.

```csharp
public ExtendedAttribute CreateExtendedAttribute(string textValue)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| textValue | Stringa | Il valore di testo specificato. |

### Valore di ritorno

restituisce l'istanza creata della classe [`ExtendedAttribute`](../../extendedattribute/) con il fieldID che è uguale al valore del fieldID di questo oggetto.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| InvalidOperationException | Se l'attuale [`CfType`](../cftype/) non è 'Text' |

## Esempi

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

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(decimal) {#createextendedattribute_5}

Crea un nuovo attributo esteso con l'ID campo che è uguale al valore dell'ID campo di questo oggetto e al valore numerico specificato.

```csharp
public ExtendedAttribute CreateExtendedAttribute(decimal numericValue)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| numericValue | Decimal | Il valore numerico specificato. |

### Valore di ritorno

restituisce l'istanza creata della classe [`ExtendedAttribute`](../../extendedattribute/) con il fieldID che è uguale al valore del fieldID di questo oggetto.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| InvalidOperationException | Se l'attuale [`CfType`](../cftype/) non è 'Number' o 'Cost' |

## Esempi

Mostra come creare la definizione di attributo esteso e impostare un valore decimale dell'attributo durante la sua costruzione.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Cost1, "My Cost");
project.ExtendedAttributes.Add(definition);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 22, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// crea attributo esteso con un valore uguale a 999m 
var extendedAttribute = definition.CreateExtendedAttribute(999m);

// aggiungi attributo esteso inizializzato con valore 999m
task.ExtendedAttributes.Add(extendedAttribute);
```

### Vedi anche

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(DateTime) {#createextendedattribute_4}

Crea un nuovo attributo esteso con l'ID campo che è uguale al valore dell'ID campo di questo oggetto e al valore della data specificato.

```csharp
public ExtendedAttribute CreateExtendedAttribute(DateTime dateTimeValue)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| dateTimeValue | DateTime | Il valore data e ora specificato. |

### Valore di ritorno

restituisce l'istanza creata della classe [`ExtendedAttribute`](../../extendedattribute/) con il fieldID che è uguale al valore del fieldID di questo oggetto.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| InvalidOperationException | Se il corrente [`CfType`](../cftype/) non è 'Date', 'Start' o 'Finish' |

## Esempi

Mostra come creare la definizione di attributo esteso e impostare un valore data e ora dell'attributo durante la sua costruzione.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var definitionWithDate = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Date1, "My Date");
project.ExtendedAttributes.Add(definitionWithDate);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 22, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// crea attributo esteso con un valore uguale a DateTime.Now 
var extendedAttribute = definitionWithDate.CreateExtendedAttribute(DateTime.Now);

// aggiungi attributo esteso
task.ExtendedAttributes.Add(extendedAttribute);
```

### Vedi anche

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(Duration) {#createextendedattribute_1}

Crea un nuovo attributo esteso con l'ID campo che è uguale al valore dell'ID campo di questo oggetto e al valore della durata specificato.

```csharp
public ExtendedAttribute CreateExtendedAttribute(Duration durationValue)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| durationValue | Durata | Il valore di durata specificato. |

### Valore di ritorno

restituisce l'istanza creata della classe [`ExtendedAttribute`](../../extendedattribute/) con il fieldID che è uguale al valore del fieldID di questo oggetto.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| InvalidOperationException | Se il corrente [`CfType`](../cftype/) non è 'Duration' |

## Esempi

Mostra come creare la definizione di attributo esteso e impostare una durata durante la sua costruzione.

```csharp
var project = new Project(DataDir + "Project2.mpp");
var task = project.RootTask.Children.Add("Test");
task.Set(Tsk.Start, new DateTime(2020, 4, 22, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Duration1, "Custom Duration");
project.ExtendedAttributes.Add(definition);

// attributo esteso Duration1 = 2 giorni
var extendedAttribute = definition.CreateExtendedAttribute(project.GetDuration(2, TimeUnitType.Day));

// aggiungi attributo esteso al compito
task.ExtendedAttributes.Add(extendedAttribute);
```

### Vedi anche

* class [ExtendedAttribute](../../extendedattribute/)
* struct [Duration](../../duration/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(bool) {#createextendedattribute_3}

Crea un nuovo attributo esteso con l'ID campo che è uguale al valore dell'ID campo di questo oggetto e al valore della flag specificato.

```csharp
public ExtendedAttribute CreateExtendedAttribute(bool flagValue)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| flagValue | Boolean | Il valore flag specificato. |

### Valore di ritorno

restituisce l'istanza creata della classe [`ExtendedAttribute`](../../extendedattribute/) con il fieldID che è uguale al valore del fieldID di questo oggetto.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| InvalidOperationException | Se il corrente [`CfType`](../cftype/) non è 'Flag' |

## Esempi

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

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(Value) {#createextendedattribute_2}

Crea un nuovo attributo esteso collegato all'elemento [`Value`](../../value/) specificato.

```csharp
public ExtendedAttribute CreateExtendedAttribute(Value lookupValue)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| lookupValue | Value | L'elemento [`Value`](../../value/) specificato. |

### Valore di ritorno

restituisce l'istanza creata della classe [`ExtendedAttribute`](../../extendedattribute/) collegata all'elemento [`Value`](../../value/) specificato.

## Osservazioni

*lookupValue* should be previously added to the [`ExtendedAttributeDefinition`](../) using [`AddLookupValue`](../addlookupvalue/) method.

## Esempi

Usa questo codice per creare un nuovo [`ExtendedAttribute`](../../extendedattribute/) usando un valore specifico:

```csharp
taskTextAttr.AddLookupValue(value1);
taskTextAttr.AddLookupValue(value2);
var extendedAttribute = taskTextAttr.CreateExtendedAttribute(value2);
```

Mostra come creare la definizione di attributo esteso e impostare un valore durante la sua costruzione.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// Crea una definizione di campo personalizzato basata sulla tabella di ricerca, dichiarata sopra.
var customFieldDefinition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(CustomFieldType.Number, ExtendedAttributeTask.Number10, "Status");

var value1 = new Value { Id = 1, Val = "25", Description = "Active" };
var value2 = new Value { Id = 2, Val = "12", Description = "Inactive" };
customFieldDefinition.AddLookupValue(value1);
customFieldDefinition.AddLookupValue(value2);
project.ExtendedAttributes.Add(customFieldDefinition);

var task = project.RootTask.Children.Add("Task");

// crea attributo esteso per un valore 
var extendedAttribute = customFieldDefinition.CreateExtendedAttribute(value2);

// aggiungi attributo esteso al compito
task.ExtendedAttributes.Add(extendedAttribute);
```

### Vedi anche

* class [ExtendedAttribute](../../extendedattribute/)
* class [Value](../../value/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


