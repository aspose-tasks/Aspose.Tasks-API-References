---
title: "ExtendedAttributeDefinition.CreateExtendedAttribute"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ExtendedAttributeDefinition methode. Maakt een nieuw uitgebreid attribuut aan met de veld-ID die gelijk is aan de veld-ID-waarde van dit object."
type: docs
weight: 310
url: /nl/net/aspose.tasks/extendedattributedefinition/createextendedattribute/
---
## CreateExtendedAttribute() {#createextendedattribute}

Maakt een nieuw uitgebreid attribuut met de veld-ID die gelijk is aan de veld-ID-waarde van dit object.

```csharp
public ExtendedAttribute CreateExtendedAttribute()
```

### Retourwaarde

Retourneert een gemaakte instantie van de [`ExtendedAttribute`](../../extendedattribute/) klasse met de fieldID die gelijk is aan de fieldID-waarde van dit object.

## Voorbeelden

Toont hoe je uitgebreide attributen maakt.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var definition = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Text1);

// Als het aangepaste veld niet bestaat in Project, maak het dan aan.
if (definition == null)
{
    definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, "My text field");
    project.ExtendedAttributes.Add(definition);
}

// Genereer uitgebreid attribuut vanuit definitie
var attribute = definition.CreateExtendedAttribute();
attribute.TextValue = "Text attribute value";

// Voeg uitgebreid attribuut toe aan taak
var task = project.RootTask.Children.Add("Task 1");
task.ExtendedAttributes.Add(attribute);

project.Save(OutDir + "CreateExtendedAttributes_out.mpp", SaveFileFormat.Mpp);
```

### Zie ook

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(string) {#createextendedattribute_6}

Maakt een nieuw uitgebreid attribuut met de veld-ID die gelijk is aan de veld-ID-waarde van dit object en de opgegeven tekstwaarde.

```csharp
public ExtendedAttribute CreateExtendedAttribute(string textValue)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| textValue | String | De opgegeven tekstwaarde. |

### Retourwaarde

Retourneert een gemaakte instantie van de [`ExtendedAttribute`](../../extendedattribute/) klasse met de fieldID die gelijk is aan de fieldID-waarde van dit object.

### Uitzonderingen

| exceptie | conditie |
| --- | --- |
| InvalidOperationException | Als de huidige [`CfType`](../cftype/) niet 'Text' is |

## Voorbeelden

Toont hoe je een definitie van een uitgebreid attribuut maakt en een tekenreekswaarde voor het attribuut instelt tijdens de constructie.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, "My Text");
project.ExtendedAttributes.Add(definition);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 22, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// maak een uitgebreid attribuut met een waarde gelijk aan 'Common Info'
var extendedAttribute = definition.CreateExtendedAttribute("Common Info");

// voeg een uitgebreid attribuut toe geïnitialiseerd met de waarde 'Common Info'
task.ExtendedAttributes.Add(extendedAttribute);
```

### Zie ook

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(decimal) {#createextendedattribute_5}

Maakt een nieuw uitgebreid attribuut met de veld-ID die gelijk is aan de veld-ID-waarde van dit object en de opgegeven numerieke waarde.

```csharp
public ExtendedAttribute CreateExtendedAttribute(decimal numericValue)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| numericValue | Decimal | De opgegeven numerieke waarde. |

### Retourwaarde

Retourneert een gemaakte instantie van de [`ExtendedAttribute`](../../extendedattribute/) klasse met de fieldID die gelijk is aan de fieldID-waarde van dit object.

### Uitzonderingen

| exceptie | conditie |
| --- | --- |
| InvalidOperationException | Als de huidige [`CfType`](../cftype/) niet 'Number' of 'Cost' is |

## Voorbeelden

Toont hoe je een definitie van een uitgebreid attribuut maakt en een decimale waarde voor het attribuut instelt tijdens de constructie.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Cost1, "My Cost");
project.ExtendedAttributes.Add(definition);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 22, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// maak een uitgebreid attribuut met een waarde gelijk aan 999m
var extendedAttribute = definition.CreateExtendedAttribute(999m);

// voeg een uitgebreid attribuut toe geïnitialiseerd met de waarde 999m
task.ExtendedAttributes.Add(extendedAttribute);
```

### Zie ook

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(DateTime) {#createextendedattribute_4}

Maakt een nieuw uitgebreid attribuut met de veld-ID die gelijk is aan de veld-ID-waarde van dit object en de opgegeven datumwaarde.

```csharp
public ExtendedAttribute CreateExtendedAttribute(DateTime dateTimeValue)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| dateTimeValue | DateTime | De opgegeven datum‑tijdwaarde. |

### Retourwaarde

Retourneert een gemaakte instantie van de [`ExtendedAttribute`](../../extendedattribute/) klasse met de fieldID die gelijk is aan de fieldID-waarde van dit object.

### Uitzonderingen

| exceptie | conditie |
| --- | --- |
| InvalidOperationException | Als de huidige [`CfType`](../cftype/) niet 'Date', 'Start' of 'Finish' is |

## Voorbeelden

Toont hoe een definitie van een uitgebreid attribuut te maken en een datum‑tijdwaarde van het attribuut in te stellen tijdens de constructie.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var definitionWithDate = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Date1, "My Date");
project.ExtendedAttributes.Add(definitionWithDate);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 22, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// maak een uitgebreid attribuut met een waarde gelijk aan DateTime.Now
var extendedAttribute = definitionWithDate.CreateExtendedAttribute(DateTime.Now);

// voeg een uitgebreid attribuut toe
task.ExtendedAttributes.Add(extendedAttribute);
```

### Zie ook

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(Duration) {#createextendedattribute_1}

Maakt een nieuw uitgebreid attribuut met de veld-ID die gelijk is aan de veld-ID-waarde van dit object en de opgegeven duurwaarde.

```csharp
public ExtendedAttribute CreateExtendedAttribute(Duration durationValue)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| durationValue | Duur | De opgegeven duurwaarde. |

### Retourwaarde

Retourneert een gemaakte instantie van de [`ExtendedAttribute`](../../extendedattribute/) klasse met de fieldID die gelijk is aan de fieldID-waarde van dit object.

### Uitzonderingen

| exceptie | conditie |
| --- | --- |
| InvalidOperationException | Als de huidige [`CfType`](../cftype/) niet 'Duration' is |

## Voorbeelden

Toont hoe een definitie van een uitgebreid attribuut te maken en een duur in te stellen tijdens de constructie.

```csharp
var project = new Project(DataDir + "Project2.mpp");
var task = project.RootTask.Children.Add("Test");
task.Set(Tsk.Start, new DateTime(2020, 4, 22, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Duration1, "Custom Duration");
project.ExtendedAttributes.Add(definition);

// uitgebreid attribuut Duration1 = 2 dagen
var extendedAttribute = definition.CreateExtendedAttribute(project.GetDuration(2, TimeUnitType.Day));

// voeg een uitgebreid attribuut toe aan de taak
task.ExtendedAttributes.Add(extendedAttribute);
```

### Zie ook

* class [ExtendedAttribute](../../extendedattribute/)
* struct [Duration](../../duration/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(bool) {#createextendedattribute_3}

Maakt een nieuw uitgebreid attribuut met de veld-ID die gelijk is aan de veld-ID-waarde van dit object en de opgegeven vlagwaarde.

```csharp
public ExtendedAttribute CreateExtendedAttribute(bool flagValue)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| flagValue | Boolean | De opgegeven vlagwaarde. |

### Retourwaarde

Retourneert een gemaakte instantie van de [`ExtendedAttribute`](../../extendedattribute/) klasse met de fieldID die gelijk is aan de fieldID-waarde van dit object.

### Uitzonderingen

| exceptie | conditie |
| --- | --- |
| InvalidOperationException | Als de huidige [`CfType`](../cftype/) niet 'Flag' is |

## Voorbeelden

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

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(Value) {#createextendedattribute_2}

Maakt een nieuw uitgebreid attribuut aan dat gekoppeld is aan het opgegeven [`Value`](../../value/) item.

```csharp
public ExtendedAttribute CreateExtendedAttribute(Value lookupValue)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| lookupValue | Value | Het opgegeven [`Value`](../../value/) item. |

### Retourwaarde

Retourneert de gemaakte instantie van de [`ExtendedAttribute`](../../extendedattribute/) klasse die gekoppeld is aan het opgegeven [`Value`](../../value/) item.

## Opmerkingen

*lookupValue* should be previously added to the [`ExtendedAttributeDefinition`](../) using [`AddLookupValue`](../addlookupvalue/) method.

## Voorbeelden

Gebruik deze code om een nieuwe [`ExtendedAttribute`](../../extendedattribute/) te maken met een specifieke waarde:

```csharp
taskTextAttr.AddLookupValue(value1);
taskTextAttr.AddLookupValue(value2);
var extendedAttribute = taskTextAttr.CreateExtendedAttribute(value2);
```

Toont hoe een definitie van een uitgebreid attribuut te maken en een waarde in te stellen tijdens de constructie.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// Maak een definitie van een aangepast veld op basis van de opzoektafel die hierboven is gedeclareerd.
var customFieldDefinition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(CustomFieldType.Number, ExtendedAttributeTask.Number10, "Status");

var value1 = new Value { Id = 1, Val = "25", Description = "Active" };
var value2 = new Value { Id = 2, Val = "12", Description = "Inactive" };
customFieldDefinition.AddLookupValue(value1);
customFieldDefinition.AddLookupValue(value2);
project.ExtendedAttributes.Add(customFieldDefinition);

var task = project.RootTask.Children.Add("Task");

// maak een uitgebreid attribuut voor een waarde
var extendedAttribute = customFieldDefinition.CreateExtendedAttribute(value2);

// voeg een uitgebreid attribuut toe aan de taak
task.ExtendedAttributes.Add(extendedAttribute);
```

### Zie ook

* class [ExtendedAttribute](../../extendedattribute/)
* class [Value](../../value/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


