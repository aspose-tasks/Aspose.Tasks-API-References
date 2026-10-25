---
title: "ExtendedAttributeDefinition"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Stelt een definitie van een uitgebreid attribuut voor dat aan een project is gekoppeld."
type: docs
weight: 83
url: /nl/java/com.aspose.tasks/extendedattributedefinition/
---

**Inheritance:**
java.lang.Object
```
public class ExtendedAttributeDefinition
```

Stelt een definitie van een uitgebreid attribuut voor dat aan een project is gekoppeld.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [addLookupValue(Value value)](#addLookupValue-com.aspose.tasks.Value-) | Voegt een waarde toe aan de interne opzoeklijst. |
| [compareTo(ExtendedAttributeDefinition o)](#compareTo-com.aspose.tasks.ExtendedAttributeDefinition-) | Vergelijkt dit object met een andere instantie van de @\{code ExtendedAttributeDefinition\} klasse. |
| [createExtendedAttribute()](#createExtendedAttribute--) | Maakt een nieuw uitgebreid attribuut met de veld-ID die gelijk is aan de veld-ID-waarde van dit object. |
| [createExtendedAttribute(boolean flagValue)](#createExtendedAttribute-boolean-) | Maakt een nieuw uitgebreid attribuut met de veld-ID die gelijk is aan de veld-ID-waarde van dit object en de opgegeven vlagwaarde. |
| [createExtendedAttribute(Duration durationValue)](#createExtendedAttribute-com.aspose.tasks.Duration-) | Maakt een nieuw uitgebreid attribuut met de veld-ID die gelijk is aan de veld-ID-waarde van dit object en de opgegeven duurwaarde. |
| [createExtendedAttribute(Value lookupValue)](#createExtendedAttribute-com.aspose.tasks.Value-) | Maakt een nieuw uitgebreid attribuut gekoppeld aan het opgegeven [Value](../../com.aspose.tasks/value) item. |
| [createExtendedAttribute(String textValue)](#createExtendedAttribute-java.lang.String-) | Maakt een nieuw uitgebreid attribuut met de veld-ID die gelijk is aan de veld-ID-waarde van dit object en de opgegeven tekstwaarde. |
| [createExtendedAttribute(BigDecimal numericValue)](#createExtendedAttribute-java.math.BigDecimal-) | Maakt een nieuw uitgebreid attribuut met de veld-ID die gelijk is aan de veld-ID-waarde van dit object en de opgegeven numerieke waarde. |
| [createExtendedAttribute(Date dateTimeValue)](#createExtendedAttribute-java.util.Date-) | Maakt een nieuw uitgebreid attribuut met de veld-ID die gelijk is aan de veld-ID-waarde van dit object en de opgegeven datumwaarde. |
| [createLookupResourceDefinition(int customFieldType, int fieldId, String alias)](#createLookupResourceDefinition-int-int-java.lang.String-) | Factory-methode die een definitie van een uitgebreid attribuut maakt met opzoekfunctie. |
| [createLookupResourceDefinition(int fieldId, String alias)](#createLookupResourceDefinition-int-java.lang.String-) | Factory-methode die een definitie van een uitgebreid attribuut maakt met opzoekfunctie. |
| [createLookupTaskDefinition(int customFieldType, int fieldId, String alias)](#createLookupTaskDefinition-int-int-java.lang.String-) | Factory-methode die een definitie van een uitgebreid attribuut maakt met opzoekfunctie. |
| [createLookupTaskDefinition(int fieldId, String alias)](#createLookupTaskDefinition-int-java.lang.String-) | Factory-methode die een definitie van een uitgebreid attribuut maakt met opzoekfunctie. |
| [createResourceDefinition(int customFieldType, int fieldId, String alias)](#createResourceDefinition-int-int-java.lang.String-) | Factory-methode die een eenvoudige definitie van een uitgebreid attribuut maakt, die Microsoft Project weergeeft als \"None\". |
| [createResourceDefinition(int fieldId, String alias)](#createResourceDefinition-int-java.lang.String-) | Factory-methode die een eenvoudige definitie van een uitgebreid attribuut maakt, die Microsoft Project weergeeft als \"None\". |
| [createTaskDefinition(int customFieldType, int fieldId, String alias)](#createTaskDefinition-int-int-java.lang.String-) | Factory-methode die een eenvoudige definitie van een uitgebreid attribuut maakt, die Microsoft Project weergeeft als \"None\". |
| [createTaskDefinition(int fieldId, String alias)](#createTaskDefinition-int-java.lang.String-) | Factory-methode die een eenvoudige definitie van een uitgebreid attribuut maakt, die Microsoft Project weergeeft als \"None\". |
| [equals(Object obj)](#equals-java.lang.Object-) | Retourneert een vlag die aangeeft of deze instantie gelijk is aan het opgegeven object. |
| [getAlias()](#getAlias--) | Haalt de alias van een aangepast veld op. |
| [getAppendNewValues()](#getAppendNewValues--) | Haalt een waarde op die aangeeft of nieuwe waarden die aan een project worden toegevoegd automatisch aan de lijst worden toegevoegd. |
| [getAutoRollDown()](#getAutoRollDown--) | Haalt een waarde op die aangeeft of een automatische doorrol naar toewijzingen is ingeschakeld. |
| [getCalculationType()](#getCalculationType--) | Haalt het type berekening van de waarde van het aangepaste attribuut op. |
| [getCfType()](#getCfType--) | Haalt het type van een aangepast veld op. |
| [getDefault()](#getDefault--) | Haalt de standaardwaarde in de lijst op. |
| [getDefaultGuid()](#getDefaultGuid--) | Haalt de Guid van het standaard lookup‑tabelitem op. |
| [getElementType()](#getElementType--) | Haalt op of het uitgebreide attribuut is gekoppeld aan een taak, een resource of een toewijzing. |
| [getFieldId()](#getFieldId--) | Haalt de project‑id op die overeenkomt met een aangepast veld. |
| [getFieldName()](#getFieldName--) | Haalt de naam van een aangepast veld op. |
| [getFormula()](#getFormula--) | Haalt de formule op die Microsoft Project gebruikt om een aangepast taakveld te vullen. |
| [getGraphicalIndicator()](#getGraphicalIndicator--) | Haalt de grafische indicatorinformatie op die aan het uitgebreide attribuut is gekoppeld. |
| [getGuid()](#getGuid--) | Haalt de Guid van een aangepast veld op. |
| [getLookupUid()](#getLookupUid--) | Haalt een Guid op van de lookup‑tabel die aan een aangepast veld is gekoppeld. |
| [getMaxMultiValues()](#getMaxMultiValues--) | Haalt het maximale aantal waarden op dat u kunt instellen in een keuzelijst. |
| [getParentProject()](#getParentProject--) | Haalt het bovenliggende project op voor de [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition)‑instantie. |
| [getPhoneticsAlias()](#getPhoneticsAlias--) | Haalt de fonetische uitspraak van de alias van een aangepast veld op. |
| [getRestrictValues()](#getRestrictValues--) | Haalt een waarde op die aangeeft of de waarden van het aangepaste veld beperkt zijn tot waarden in de `ValueList`([getValueList()](../../com.aspose.tasks/extendedattributedefinition\\#getValueList--)/ [setValueList(List)](../../com.aspose.tasks/extendedattributedefinition\\#setValueList-List-Value--)). |
| [getRollupType()](#getRollupType--) | Haalt de manier waarop roll‑ups worden berekend op. |
| [getSecondaryGuid()](#getSecondaryGuid--) | Haalt de secundaire guid van het uitgebreide attribuut op. |
| [getSecondaryPid()](#getSecondaryPid--) | Haalt de secundaire PID van een aangepast veld op. |
| [getSummaryRowsCalculationType()](#getSummaryRowsCalculationType--) | Haalt het type berekening van de waarde van het aangepaste attribuut voor samenvattingsrijen op. |
| [getUserDef()](#getUserDef--) | Haalt een waarde op die aangeeft of een aangepast veld door de gebruiker is gedefinieerd. |
| [getValueList()](#getValueList--) | Haalt de List&lt;Value&gt; ValueList op. |
| [getValuelistSortOrder()](#getValuelistSortOrder--) | Haalt de manier waarop waardelijsten worden gesorteerd op. |
| [hashCode()](#hashCode--) | Retourneert een hashcode voor de instantie van de [ExtendedAttributeDefinition](../../com.aspose/tasks/extendedattributedefinition) klasse. |
| [removeLookupValue(Value value)](#removeLookupValue-com.aspose.tasks.Value-) | Verwijdert een waarde uit de interne opzoeklijst. |
| [setAlias(String value)](#setAlias-java.lang.String-) | Stelt de alias van een aangepast veld in. |
| [setAppendNewValues(boolean value)](#setAppendNewValues-boolean-) | Stelt een waarde in die aangeeft of nieuwe waarden die aan een project worden toegevoegd automatisch aan de lijst worden toegevoegd. |
| [setAutoRollDown(boolean value)](#setAutoRollDown-boolean-) | Stelt een waarde in die aangeeft of een automatische doorrol naar toewijzingen is ingeschakeld. |
| [setCalculationType(int value)](#setCalculationType-int-) | Stelt het type berekening van de waarde van het aangepaste attribuut in. |
| [setDefault(String value)](#setDefault-java.lang.String-) | Stelt de standaardwaarde in de lijst in. |
| [setDefaultGuid(String value)](#setDefaultGuid-java.lang.String-) | Stelt de Guid van het standaard opzoektabelitem in. |
| [setElementType(int value)](#setElementType-int-) | Stelt in dat het uitgebreide attribuut is gekoppeld aan een taak, een resource of een toewijzing. |
| [setFieldId(String value)](#setFieldId-java.lang.String-) | Stelt overeen met de project-id van een aangepast veld. |
| [setFormula(String value)](#setFormula-java.lang.String-) | Stelt de formule in die Microsoft Project gebruikt om een aangepast taakveld te vullen. |
| [setGraphicalIndicator(GraphicalIndicatorsInfo value)](#setGraphicalIndicator-com.aspose.tasks.GraphicalIndicatorsInfo-) | Stelt grafische indicatorinformatie in die is gekoppeld aan het uitgebreide attribuut. |
| [setGuid(String value)](#setGuid-java.lang.String-) | Stelt de Guid van een aangepast veld in. |
| [setMaxMultiValues(int value)](#setMaxMultiValues-int-) | Stelt het maximale aantal waarden in dat u in een keuzelijst kunt instellen. |
| [setPhoneticsAlias(String value)](#setPhoneticsAlias-java.lang.String-) | Stelt de fonetische uitspraak van de alias van een aangepast veld in. |
| [setRestrictValues(boolean value)](#setRestrictValues-boolean-) | Stelt een waarde in die aangeeft of de waarden van het aangepaste veld beperkt zijn tot waarden in de `ValueList`([getValueList()](../../com.aspose/tasks/extendedattributedefinition\#getValueList--)/ [setValueList(List)](../../com.aspose/tasks/extendedattributedefinition\#setValueList-List-Value--)). |
| [setRollupType(int value)](#setRollupType-int-) | Stelt de manier in waarop roll-ups worden berekend. |
| [setSecondaryGuid(String value)](#setSecondaryGuid-java.lang.String-) | Stelt de secundaire guid van het uitgebreide attribuut in. |
| [setSecondaryPid(String value)](#setSecondaryPid-java.lang.String-) | Stelt de secundaire PID van een aangepast veld in. |
| [setSummaryRowsCalculationType(int value)](#setSummaryRowsCalculationType-int-) | Stelt het type berekening van de waarde van het aangepaste attribuut in voor samenvattingsrijen. |
| [setUserDef(boolean value)](#setUserDef-boolean-) | Stelt een waarde in die aangeeft of een aangepast veld door de gebruiker is gedefinieerd. |
| [setValuelistSortOrder(int value)](#setValuelistSortOrder-int-) | Stelt de manier in waarop waardelijsten worden gesorteerd. |
### addLookupValue(Value value) {#addLookupValue-com.aspose.tasks.Value-}
```
public final void addLookupValue(Value value)
```


Voegt een waarde toe aan de interne opzoeklijst. Dit is een voorkeursmethode voor manipulaties met de `ValueList`([getValueList()](../../com.aspose/tasks/extendedattributedefinition\#getValueList--)/ [setValueList(List)](../../com.aspose/tasks/extendedattributedefinition\#setValueList-List-Value--)).

--------------------

&gt; ```
&gt; Gebruik deze code om een nieuwe waarde toe te voegen aan de opzoeklijst:
&gt; ``````

taskTextAttr.addLookupValue(new Value() {{
this.setId(1);
this.setVal("Text value 1");
this.setDescription("Text value description 1");
}});
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Value](../../com.aspose.tasks/value) | Value to add into lookup.

--------------------

This method works only for [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) instances which have `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) equals to [CalculationType.Lookup](../../com.aspose.tasks/calculationtype\#Lookup). |

### compareTo(ExtendedAttributeDefinition o) {#compareTo-com.aspose.tasks.ExtendedAttributeDefinition-}
```
public int compareTo(ExtendedAttributeDefinition o)
```


Compares this object with another instance of the @\{code ExtendedAttributeDefinition\} class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| o | [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) | the object to be compared. |

**Returns:**
int - a negative integer, zero, or a positive integer as this object is less than, equal to, or greater than the specified object.
### createExtendedAttribute() {#createExtendedAttribute--}
```
public final ExtendedAttribute createExtendedAttribute()
```


Creates a new extended attribute with the field ID which equals to this object's field ID value.

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class with the fieldID which equals to this object's fieldID value.
### createExtendedAttribute(boolean flagValue) {#createExtendedAttribute-boolean-}
```
public final ExtendedAttribute createExtendedAttribute(boolean flagValue)
```


Creates a new extended attribute with the field ID which equals to this object's field ID value and the specified flag value.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| flagValue | boolean | The specified flag value. |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class with the fieldID which equals to this object's fieldID value.
### createExtendedAttribute(Duration durationValue) {#createExtendedAttribute-com.aspose.tasks.Duration-}
```
public final ExtendedAttribute createExtendedAttribute(Duration durationValue)
```


Creates a new extended attribute with the field ID which equals to this object's field ID value and the specified duration value.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| durationValue | [Duration](../../com.aspose.tasks/duration) | The specified duration value. |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class with the fieldID which equals to this object's fieldID value.
### createExtendedAttribute(Value lookupValue) {#createExtendedAttribute-com.aspose.tasks.Value-}
```
public final ExtendedAttribute createExtendedAttribute(Value lookupValue)
```


Creates new extended attribute linked with specified [Value](../../com.aspose.tasks/value) item.

--------------------

&gt; ```
&gt; Use this code to create new [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) using specific value:
&gt; ``````

 taskTextAttr.addLookupValue(value1);
 taskTextAttr.addLookupValue(value2);
 ExtendedAttribute extendedAttribute = taskTextAttr.createExtendedAttribute(value2);
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | lookupValue | [Value](../../com.aspose.tasks/value) | Het opgegeven [Value](../../com.aspose.tasks/value) item. |

--------------------

`lookupValue` moet eerder worden toegevoegd aan de [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) met behulp van de [addLookupValue(Value)](../../com.aspose.tasks/extendedattributedefinition\#addLookupValue-Value-) methode. |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class linked with specified [Value](../../com.aspose.tasks/value) item.
### createExtendedAttribute(String textValue) {#createExtendedAttribute-java.lang.String-}
```
public final ExtendedAttribute createExtendedAttribute(String textValue)
```


Maakt een nieuw uitgebreid attribuut met de veld-ID die gelijk is aan de veld-ID-waarde van dit object en de opgegeven tekstwaarde.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| textValue | java.lang.String | De opgegeven tekstwaarde. |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class with the fieldID which equals to this object's fieldID value.
### createExtendedAttribute(BigDecimal numericValue) {#createExtendedAttribute-java.math.BigDecimal-}
```
public final ExtendedAttribute createExtendedAttribute(BigDecimal numericValue)
```


Maakt een nieuw uitgebreid attribuut met de veld-ID die gelijk is aan de veld-ID-waarde van dit object en de opgegeven numerieke waarde.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| numericValue | java.math.BigDecimal | De opgegeven numerieke waarde. |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class with the fieldID which equals to this object's fieldID value.
### createExtendedAttribute(Date dateTimeValue) {#createExtendedAttribute-java.util.Date-}
```
public final ExtendedAttribute createExtendedAttribute(Date dateTimeValue)
```


Maakt een nieuw uitgebreid attribuut met de veld-ID die gelijk is aan de veld-ID-waarde van dit object en de opgegeven datumwaarde.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| dateTimeValue | java.util.Date | De opgegeven datum‑tijdwaarde. |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class with the fieldID which equals to this object's fieldID value.
### createLookupResourceDefinition(int customFieldType, int fieldId, String alias) {#createLookupResourceDefinition-int-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createLookupResourceDefinition(int customFieldType, int fieldId, String alias)
```


Factory‑methode die een uitgebreide attribuutdefinitie met lookup maakt. Het heeft `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) gelijk aan [CalculationType.Lookup](../../com.aspose.tasks/calculationtype\#Lookup) en kan alleen in Resources worden gebruikt. U moet `customFieldType`, `fieldId` en `alias` opgeven bij het aanroepen van deze methode.

--------------------

&gt; ```
&gt; Gebruik dit voorbeeld om een aangepaste velddefinitie voor een resource met lookup te maken en deze vervolgens te vullen met tekstwaarden:
&gt; ``````

ExtendedAttributeDefinition resourceTextAttr = ExtendedAttributeDefinition.createLookupResourceDefinition(ExtendedAttributeResource.Text27, "My custom field");
resourceTextAttr.addLookupValue(new Value() {{
this.setId(1);
this.setVal("Text value 1");
this.setDescription("Text value description 1");
}});
resourceTextAttr.addLookupValue(new Value() {{
this.setId(2);
this.setVal("Text value 2");
this.setDescription("Text value description 2");
}});
project.getExtendedAttributes().add(resourceTextAttr);
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| customFieldType | int | The specified [CustomFieldType](../../com.aspose.tasks/customfieldtype) type. |
| fieldId | int | The specified [ExtendedAttributeResource](../../com.aspose.tasks/extendedattributeresource) field ID. |
| alias | java.lang.String | The specified String alias. |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `customFieldType`, `fieldId` and `alias`.
### createLookupResourceDefinition(int fieldId, String alias) {#createLookupResourceDefinition-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createLookupResourceDefinition(int fieldId, String alias)
```


Factory method which creates an extended attribute definition with lookup. It has `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) equals to [CalculationType.Lookup](../../com.aspose.tasks/calculationtype\#Lookup) and can be used in Resources only. You are required to specify `fieldId` and `alias` when call this method. The field type is inferred from field id.

--------------------

&gt; ```
&gt; Use this example to create a custom field definition for a resource with lookup and then fill it with text values:
&gt; ``````

 ExtendedAttributeDefinition resourceTextAttr = ExtendedAttributeDefinition.createLookupResourceDefinition(ExtendedAttributeResource.Text27, "My custom field");
     resourceTextAttr.addLookupValue(new Value() {{
         this.setId(1);
         this.setVal("Text value 1");
         this.setDescription("Text value description 1");
     }});
     resourceTextAttr.addLookupValue(new Value() {{
         this.setId(2);
         this.setVal("Text value 2");
         this.setDescription("Text value description 2");
     }});
     project.getExtendedAttributes().add(resourceTextAttr);
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fieldId | int | Het opgegeven [ExtendedAttributeResource](../../com.aspose.tasks/extendedattributeresource) veld-ID. |
| alias | java.lang.String | De opgegeven String alias. |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `fieldId` and `alias`.
### createLookupTaskDefinition(int customFieldType, int fieldId, String alias) {#createLookupTaskDefinition-int-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createLookupTaskDefinition(int customFieldType, int fieldId, String alias)
```


Factory-methode die een uitgebreide attribuutdefinitie met opzoeking maakt. Het heeft `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) gelijk aan [CalculationType.Lookup](../../com.aspose.tasks/calculationtype\#Lookup) en kan alleen in Taken worden gebruikt. U moet `customFieldType`, `fieldId` en `alias` opgeven bij het aanroepen van deze methode.

--------------------

&gt; ```
&gt; Gebruik dit voorbeeld om een aangepaste velddefinitie voor een taak met opzoeking te maken en deze vervolgens te vullen met tekstwaarden:
&gt; ``````

ExtendedAttributeDefinition taskTextAttr = ExtendedAttributeDefinition.createLookupTaskDefinition(CustomFieldType.Text, ExtendedAttributeResource.Text27, "My custom field");
taskTextAttr.addLookupValue(new Value() {{
this.setId(1);
this.setVal("Text value 1");
this.setDescription("Text value description 1");
}});
taskTextAttr.addLookupValue(new Value() {{
this.setId(2);
this.setVal("Text value 2");
this.setDescription("Text value description 2");
}});
project.getExtendedAttributes().add(taskTextAttr);
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| customFieldType | int | The specified [CustomFieldType](../../com.aspose.tasks/customfieldtype) type. |
| fieldId | int | The specified [ExtendedAttributeTask](../../com.aspose.tasks/extendedattributetask) field ID. |
| alias | java.lang.String | The specified String alias. |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `customFieldType`, `fieldId` and `alias`.
### createLookupTaskDefinition(int fieldId, String alias) {#createLookupTaskDefinition-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createLookupTaskDefinition(int fieldId, String alias)
```


Factory method which creates an extended attribute definition with lookup. It has `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) equals to [CalculationType.Lookup](../../com.aspose.tasks/calculationtype\#Lookup) and can be used in Tasks only. You are required to specify `fieldId` and `alias` when call this method. The field type is inferred from field id.

--------------------

&gt; ```
&gt; Use this example to create a custom field definition for a task with lookup and then fill it with text values:
&gt; ``````

 ExtendedAttributeDefinition taskTextAttr = ExtendedAttributeDefinition.createLookupTaskDefinition(CustomFieldType.Text, ExtendedAttributeResource.Text27, "My custom field");
 taskTextAttr.addLookupValue(new Value() {{
     this.setId(1);
     this.setVal("Text value 1");
     this.setDescription("Text value description 1");
 }});
 taskTextAttr.addLookupValue(new Value() {{
     this.setId(2);
     this.setVal("Text value 2");
     this.setDescription("Text value description 2");
 }});
 project.getExtendedAttributes().add(taskTextAttr);
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fieldId | int | Het opgegeven [ExtendedAttributeTask](../../com.aspose.tasks/extendedattributetask) veld-ID. |
| alias | java.lang.String | De opgegeven String alias. |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `fieldId` and `alias`.
### createResourceDefinition(int customFieldType, int fieldId, String alias) {#createResourceDefinition-int-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createResourceDefinition(int customFieldType, int fieldId, String alias)
```


Factory-methode die een eenvoudige uitgebreide attribuutdefinitie maakt, die Microsoft Project weergeeft als "None". Het heeft `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) gelijk aan [CalculationType.None](../../com.aspose.tasks/calculationtype\#None) en kan alleen in Resource worden gebruikt. U moet `customFieldType`, `fieldId` en `alias` opgeven bij het aanroepen van deze methode.

--------------------

&gt; ```
&gt; Gebruik dit voorbeeld om een aangepaste tekstvelddefinitie te maken:
&gt; ``````

ExtendedAttributeDefinition resourceTextAttr = ExtendedAttributeDefinition.createResourceDefinition(CustomFieldType.Text, ExtendedAttributeResource.Text27, "My custom field");
project.getExtendedAttributes().add(resourceTextAttr);
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| customFieldType | int | The specified [CustomFieldType](../../com.aspose.tasks/customfieldtype) type. |
| fieldId | int | The specified [ExtendedAttributeResource](../../com.aspose.tasks/extendedattributeresource) field ID. |
| alias | java.lang.String | The specified String alias. |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `customFieldType`, `fieldId` and `alias`.
### createResourceDefinition(int fieldId, String alias) {#createResourceDefinition-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createResourceDefinition(int fieldId, String alias)
```


Factory method which creates a simple extended attribute definition, which Microsoft Project shows as "None". It has `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) equals to [CalculationType.None](../../com.aspose.tasks/calculationtype\#None) and can be used in Resource only. You are required to specify `fieldId` and `alias` when call this method. The field type is inferred from field id.

--------------------

&gt; ```
&gt; Use this example to create a custom text field definition:
&gt; ``````

 ExtendedAttributeDefinition resourceTextAttr = ExtendedAttributeDefinition.createResourceDefinition(ExtendedAttributeResource.Text27, "My custom field");
 project.getExtendedAttributes().add(resourceTextAttr);
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fieldId | int | Het opgegeven [ExtendedAttributeResource](../../com.aspose.tasks/extendedattributeresource) veld-ID. |
| alias | java.lang.String | De opgegeven String alias. |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `fieldId` and `alias`.
### createTaskDefinition(int customFieldType, int fieldId, String alias) {#createTaskDefinition-int-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createTaskDefinition(int customFieldType, int fieldId, String alias)
```


Factory-methode die een eenvoudige uitgebreide attribuutdefinitie maakt, die Microsoft Project weergeeft als "None". Het heeft `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) gelijk aan [CalculationType.None](../../com.aspose.tasks/calculationtype\#None) en kan alleen in Taken worden gebruikt. U moet `customFieldType`, `fieldId` en `alias` opgeven bij het aanroepen van deze methode.

--------------------

&gt; ```
&gt; Gebruik dit voorbeeld om een aangepaste tekstvelddefinitie te maken:
&gt; ``````

ExtendedAttributeDefinition taskTextAttr = ExtendedAttributeDefinition.createTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text27, "My custom field");
project.getExtendedAttributes().add(taskTextAttr);
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| customFieldType | int | The specified [CustomFieldType](../../com.aspose.tasks/customfieldtype) type. |
| fieldId | int | The specified [ExtendedAttributeTask](../../com.aspose.tasks/extendedattributetask) field ID. |
| alias | java.lang.String | The specified String alias. |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `customFieldType`, `fieldId` and `alias`.
### createTaskDefinition(int fieldId, String alias) {#createTaskDefinition-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createTaskDefinition(int fieldId, String alias)
```


Factory method which creates a simple extended attribute definition, which Microsoft Project shows as "None". It has `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) equals to [CalculationType.None](../../com.aspose.tasks/calculationtype\#None) and can be used in Tasks only. You are required to specify `fieldId` and `alias` when calling this method. The field type is inferred from field id.

--------------------

&gt; ```
&gt; Use this example to create a custom text field definition:
&gt; ``````

 ExtendedAttributeDefinition taskTextAttr = ExtendedAttributeDefinition.createTaskDefinition(ExtendedAttributeTask.Text27, "My custom field");
 project.getExtendedAttributes().add(taskTextAttr);
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fieldId | int | Het opgegeven [ExtendedAttributeTask](../../com.aspose.tasks/extendedattributetask) veld-ID. |
| alias | java.lang.String | De opgegeven String alias. |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `fieldId` and `alias`.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Retourneert een vlag die aangeeft of deze instantie gelijk is aan het opgegeven object.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| obj | java.lang.Object | het opgegeven object om te vergelijken met deze instantie. |

**Returns:**
boolean - een vlag die aangeeft of deze instantie gelijk is aan het opgegeven object.
### getAlias() {#getAlias--}
```
public final String getAlias()
```


Haalt de alias van een aangepast veld op.

**Returns:**
java.lang.String - de alias van een aangepast veld.
### getAppendNewValues() {#getAppendNewValues--}
```
public final boolean getAppendNewValues()
```


Haalt een waarde op die aangeeft of nieuwe waarden die aan een project worden toegevoegd automatisch aan de lijst worden toegevoegd.

--------------------

Momenteel ondersteund voor MSP 2003/2007 Xml- en MSP 2003 mpp-formaten.

**Returns:**
boolean - een waarde die aangeeft of nieuwe waarden die aan een project worden toegevoegd automatisch aan de lijst worden toegevoegd.
### getAutoRollDown() {#getAutoRollDown--}
```
public final boolean getAutoRollDown()
```


Haalt een waarde op die aangeeft of een automatische doorrol naar toewijzingen is ingeschakeld.

**Returns:**
boolean - een waarde die aangeeft of een automatische doorrol naar toewijzingen is ingeschakeld.
### getCalculationType() {#getCalculationType--}
```
public final int getCalculationType()
```


Haalt het type berekening van de waarde van het aangepaste attribuut op.

**Returns:**
int - het type berekening van de waarde van het aangepaste attribuut.
### getCfType() {#getCfType--}
```
public final int getCfType()
```


Haalt het type van een aangepast veld op.

**Returns:**
int - het type van een aangepast veld.
### getDefault() {#getDefault--}
```
public final String getDefault()
```


Haalt de standaardwaarde in de lijst op.

--------------------

Momenteel ondersteund voor MSP 2003/2007 Xml- en MSP 2003 mpp-formaten.

**Returns:**
java.lang.String - de standaardwaarde in de lijst.
### getDefaultGuid() {#getDefaultGuid--}
```
public final String getDefaultGuid()
```


Haalt de Guid van het standaard lookup‑tabelitem op.

**Returns:**
java.lang.String - de Guid van het standaard opzoektabelitem.
### getElementType() {#getElementType--}
```
public final int getElementType()
```


Haalt op of het uitgebreide attribuut is gekoppeld aan een taak, een resource of een toewijzing.

**Returns:**
int - het uitgebreide attribuut is gekoppeld aan een taak, een resource of een toewijzing.
### getFieldId() {#getFieldId--}
```
public final String getFieldId()
```


Gets komt overeen met de project-id van een aangepast veld. Gebruik de tekenreeksrepresentatie van een constante uit de [ExtendedAttributeTask](../../com.aspose.tasks/extendedattributetask) klasse om de `FieldId`([getFieldId()](../../com.aspose.tasks/extendedattributedefinition\#getFieldId--)/ [setFieldId(String)](../../com.aspose.tasks/extendedattributedefinition\#setFieldId-String-)) eigenschap te specificeren.

--------------------

&gt; ```
&gt;
&gt; ``````

customFieldDefinition.setFieldId(Integer.toString(ExtendedAttributeTask.Number10));
 
```

--------------------

Preferable way to set `FieldId`([getFieldId()](../../com.aspose.tasks/extendedattributedefinition\#getFieldId--)/ [setFieldId(String)](../../com.aspose.tasks/extendedattributedefinition\#setFieldId-String-)) property is to create [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) using one of the dedicated factory methods like [createTaskDefinition(int, String)](../../com.aspose.tasks/extendedattributedefinition\#createTaskDefinition-int--String-) or [createLookupTaskDefinition(int, int, String)](../../com.aspose.tasks/extendedattributedefinition\#createLookupTaskDefinition-int--int--String-).

**Returns:**
java.lang.String - corresponds to the project id of a custom field.
### getFieldName() {#getFieldName--}
```
public final String getFieldName()
```


Gets the name of a custom field.

--------------------

Should not be set directly, instead create ExtendedAttributeDefinition using strongly typed static factory methods named like create\*Definition().

**Returns:**
java.lang.String - the name of a custom field.
### getFormula() {#getFormula--}
```
public final String getFormula()
```


Gets the formula that Microsoft Project uses to populate a custom task field.

**Returns:**
java.lang.String - the formula that Microsoft Project uses to populate a custom task field.
### getGraphicalIndicator() {#getGraphicalIndicator--}
```
public final GraphicalIndicatorsInfo getGraphicalIndicator()
```


Gets a graphical indicators info associated with the extended attribute. Applicable to MPP format.

**Returns:**
[GraphicalIndicatorsInfo](../../com.aspose.tasks/graphicalindicatorsinfo) - a graphical indicators info associated with the extended attribute.
### getGuid() {#getGuid--}
```
public final String getGuid()
```


Gets the Guid of a custom field.

--------------------

Currently supported for Xml format only.

**Returns:**
java.lang.String - the Guid of a custom field.
### getLookupUid() {#getLookupUid--}
```
public final String getLookupUid()
```


Gets a Guid of the lookup table associated with a custom field.

--------------------

In order to create a custom field with lookup, use one of the factory methods: [createLookupTaskDefinition(int, int, String)](../../com.aspose.tasks/extendedattributedefinition\#createLookupTaskDefinition-int--int--String-) or [createLookupResourceDefinition(int, int, String)](../../com.aspose.tasks/extendedattributedefinition\#createLookupResourceDefinition-int--int--String-).

**Returns:**
java.lang.String - a Guid of the lookup table associated with a custom field.
### getMaxMultiValues() {#getMaxMultiValues--}
```
public final int getMaxMultiValues()
```


Gets the maximum number of values you can set in a pick list.

--------------------

Currently supported for Xml format only.

**Returns:**
int - the maximum number of values you can set in a pick list.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Gets the parent project for the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) instance.

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent project for the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) instance.
### getPhoneticsAlias() {#getPhoneticsAlias--}
```
public final String getPhoneticsAlias()
```


Gets the phonetic pronunciation of the alias of a custom field.

--------------------

Currently supported for Xml format only.

**Returns:**
java.lang.String - the phonetic pronunciation of the alias of a custom field.
### getRestrictValues() {#getRestrictValues--}
```
public final boolean getRestrictValues()
```


Gets a value indicating whether the custom field values are restricted to values in the `ValueList`([getValueList()](../../com.aspose.tasks/extendedattributedefinition\#getValueList--)/ [setValueList(List)](../../com.aspose.tasks/extendedattributedefinition\#setValueList-List-Value--)).

**Returns:**
boolean - a value indicating whether the custom field values are restricted to values in the `ValueList`([getValueList()](../../com.aspose.tasks/extendedattributedefinition\#getValueList--)/ [setValueList(List)](../../com.aspose.tasks/extendedattributedefinition\#setValueList-List-Value--)).
### getRollupType() {#getRollupType--}
```
public final int getRollupType()
```


Gets the way rollups are calculated.

--------------------

Writing currently supported for Xml format only.

**Returns:**
int - the way rollups are calculated.
### getSecondaryGuid() {#getSecondaryGuid--}
```
public final String getSecondaryGuid()
```


Gets the secondary guid of extended attribute.

--------------------

This is new for MS Project 2010 property.

**Returns:**
java.lang.String - the secondary guid of extended attribute.
### getSecondaryPid() {#getSecondaryPid--}
```
public final String getSecondaryPid()
```


Gets the secondary PID of a custom field.

**Returns:**
java.lang.String - the secondary PID of a custom field.
### getSummaryRowsCalculationType() {#getSummaryRowsCalculationType--}
```
public final int getSummaryRowsCalculationType()
```


Gets the type of calculation of the custom attribute's value for summary rows.

**Returns:**
int - the type of calculation of the custom attribute's value for summary rows.
### getUserDef() {#getUserDef--}
```
public final boolean getUserDef()
```


Gets a value indicating whether a custom field is user defined.

--------------------

Currently supported for Xml format only.

**Returns:**
boolean - a value indicating whether a custom field is user defined.
### getValueList() {#getValueList--}
```
public final List<Value> getValueList()
```


Gets the List&lt;Value&gt; ValueList.

--------------------

When values of extended attributes are specified as properties of elements in the schema, they may either be specified by values or by references to the values contained in this list. Applications may assume ordering of the list by ordering specified here. Currently supported for MSP 2003/2007 Xml and MSP 2003 mpp formats. Do not change this list directly. Use ExtendedAttributeDefinition.addLookupValue/removeLookupValue methods instead.

**Returns:**
java.util.List&lt;com.aspose.tasks.Value&gt; - the List&lt;Value&gt; ValueList.
### getValuelistSortOrder() {#getValuelistSortOrder--}
```
public final int getValuelistSortOrder()
```


Gets the way value lists are sorted. Values are: 0=Descending, 1=Ascending.

--------------------

Currently supported for MSP 2003/2007 Xml and MSP 2003 mpp formats.

**Returns:**
int - the way value lists are sorted.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Returns a hash code for the instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class.

**Returns:**
int - a hash code for this object.
### removeLookupValue(Value value) {#removeLookupValue-com.aspose.tasks.Value-}
```
public final void removeLookupValue(Value value)
```


Removes a value from the internal lookup list. This is a preferable way for manipulations with the `ValueList`([getValueList()](../../com.aspose.tasks/extendedattributedefinition\#getValueList--)/ [setValueList(List)](../../com.aspose.tasks/extendedattributedefinition\#setValueList-List-Value--)).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Value](../../com.aspose.tasks/value) | Value to remove from lookup.

--------------------

This method works only for [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) instances which have `CalculationType`([getCalculationType](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) equals to [CalculationType.Lookup](../../com.aspose.tasks/calculationtype\#Lookup). |

### setAlias(String value) {#setAlias-java.lang.String-}
```
public final void setAlias(String value)
```


Sets the alias of a custom field.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the alias of a custom field. |

### setAppendNewValues(boolean value) {#setAppendNewValues-boolean-}
```
public final void setAppendNewValues(boolean value)
```


Sets a value indicating whether new values added to a project are automatically added to the list.

--------------------

Currently supported for MSP 2003/2007 Xml and MSP 2003 mpp formats.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether new values added to a project are automatically added to the list. |

### setAutoRollDown(boolean value) {#setAutoRollDown-boolean-}
```
public final void setAutoRollDown(boolean value)
```


Sets a value indicating whether an automatic roll down to assignments is enabled.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether an automatic roll down to assignments is enabled. |

### setCalculationType(int value) {#setCalculationType-int-}
```
public final void setCalculationType(int value)
```


Sets the type of calculation of the custom attribute's value.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the type of calculation of the custom attribute's value. |

### setDefault(String value) {#setDefault-java.lang.String-}
```
public final void setDefault(String value)
```


Sets the default value in the list.

Currently supported for MSP 2003/2007 Xml and MSP 2003 mpp formats.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the default value in the list. |

### setDefaultGuid(String value) {#setDefaultGuid-java.lang.String-}
```
public final void setDefaultGuid(String value)
```


Sets the Guid of the default lookup table entry.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the Guid of the default lookup table entry. |

### setElementType(int value) {#setElementType-int-}
```
public final void setElementType(int value)
```


Sets the extended attribute is associated with a task, a resource or an assignment.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the extended attribute is associated with a task, a resource or an assignment. |

### setFieldId(String value) {#setFieldId-java.lang.String-}
```
public final void setFieldId(String value)
```


Sets corresponds to the project id of a custom field. Use string representation of a constant from [ExtendedAttributeTask](../../com.aspose.tasks/extendedattributetask) class to specify `FieldId`([getFieldId()](../../com.aspose.tasks/extendedattributedefinition\#getFieldId--)/ [setFieldId(String)](../../com.aspose.tasks/extendedattributedefinition\#setFieldId-String-)) property.

--------------------

&gt; ```
&gt; 
&gt; ``````

 customFieldDefinition.setFieldId(Integer.toString(ExtendedAttributeTask.Number10));
 
```

--------------------

De voorkeur heeft om de `FieldId`([getFieldId()](../../com.aspose/tasks/extendedattributedefinition\\#getFieldId--)/ [setFieldId(String)](../../com.aspose/tasks/extendedattributedefinition\\#setFieldId-String-)) eigenschap in te stellen door een [ExtendedAttributeDefinition](../../com.aspose/tasks/extendedattributedefinition) te maken met een van de speciale fabrieksmethoden zoals [createTaskDefinition(int, String)](../../com.aspose/tasks/extendedattributedefinition\\#createTaskDefinition-int--String-) of [createLookupTaskDefinition(int, int, String)](../../com.aspose/tasks/extendedattributedefinition\\#createLookupTaskDefinition-int--int--String-).

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | komt overeen met de project-id van een aangepast veld. |

### setFormula(String value) {#setFormula-java.lang.String-}
```
public final void setFormula(String value)
```


Stelt de formule in die Microsoft Project gebruikt om een aangepast taakveld te vullen.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | de formule die Microsoft Project gebruikt om een aangepast taakveld te vullen. |

### setGraphicalIndicator(GraphicalIndicatorsInfo value) {#setGraphicalIndicator-com.aspose.tasks.GraphicalIndicatorsInfo-}
```
public final void setGraphicalIndicator(GraphicalIndicatorsInfo value)
```


Stelt grafische indicatorinformatie in die is gekoppeld aan het uitgebreide attribuut. Van toepassing op MPP-formaat.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [GraphicalIndicatorsInfo](../../com.aspose.tasks/graphicalindicatorsinfo) | grafische indicatorinformatie die is gekoppeld aan het uitgebreide attribuut. |

### setGuid(String value) {#setGuid-java.lang.String-}
```
public final void setGuid(String value)
```


Stelt de Guid van een aangepast veld in.

--------------------

Momenteel alleen ondersteund voor Xml-formaat.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | de Guid van een aangepast veld. |

### setMaxMultiValues(int value) {#setMaxMultiValues-int-}
```
public final void setMaxMultiValues(int value)
```


Stelt het maximale aantal waarden in dat u in een keuzelijst kunt instellen.

--------------------

Momenteel alleen ondersteund voor Xml-formaat.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | het maximale aantal waarden dat u kunt instellen in een keuzelijst. |

### setPhoneticsAlias(String value) {#setPhoneticsAlias-java.lang.String-}
```
public final void setPhoneticsAlias(String value)
```


Stelt de fonetische uitspraak van de alias van een aangepast veld in.

--------------------

Momenteel alleen ondersteund voor Xml-formaat.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | de fonetische uitspraak van de alias van een aangepast veld. |

### setRestrictValues(boolean value) {#setRestrictValues-boolean-}
```
public final void setRestrictValues(boolean value)
```


Stelt een waarde in die aangeeft of de waarden van het aangepaste veld beperkt zijn tot waarden in de `ValueList`([getValueList()](../../com.aspose/tasks/extendedattributedefinition\#getValueList--)/ [setValueList(List)](../../com.aspose/tasks/extendedattributedefinition\#setValueList-List-Value--)).

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of de waarden van het aangepaste veld beperkt zijn tot waarden in de |

### setRollupType(int value) {#setRollupType-int-}
```
public final void setRollupType(int value)
```


Stelt de manier in waarop roll-ups worden berekend.

--------------------

Schrijven momenteel alleen ondersteund voor Xml-formaat.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | de manier waarop roll-ups worden berekend. |

### setSecondaryGuid(String value) {#setSecondaryGuid-java.lang.String-}
```
public final void setSecondaryGuid(String value)
```


Stelt de secundaire guid van het uitgebreide attribuut in.

--------------------

Dit is een nieuwe eigenschap voor MS Project 2010.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | de secundaire guid van het uitgebreide attribuut. |

### setSecondaryPid(String value) {#setSecondaryPid-java.lang.String-}
```
public final void setSecondaryPid(String value)
```


Stelt de secundaire PID van een aangepast veld in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | de secundaire PID van een aangepast veld. |

### setSummaryRowsCalculationType(int value) {#setSummaryRowsCalculationType-int-}
```
public final void setSummaryRowsCalculationType(int value)
```


Stelt het type berekening van de waarde van het aangepaste attribuut in voor samenvattingsrijen.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | het type berekening van de waarde van het aangepaste attribuut voor samenvattingsrijen. |

### setUserDef(boolean value) {#setUserDef-boolean-}
```
public final void setUserDef(boolean value)
```


Stelt een waarde in die aangeeft of een aangepast veld door de gebruiker is gedefinieerd.

--------------------

Momenteel alleen ondersteund voor Xml-formaat.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of een aangepast veld door de gebruiker is gedefinieerd. |

### setValuelistSortOrder(int value) {#setValuelistSortOrder-int-}
```
public final void setValuelistSortOrder(int value)
```


Stelt de manier in waarop waardelijsten worden gesorteerd. Waarden zijn: 0=Aflopend, 1=Oplopend.

--------------------

Momenteel ondersteund voor MSP 2003/2007 Xml- en MSP 2003 mpp-formaten.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | de manier waarop waardelijsten worden gesorteerd. |

