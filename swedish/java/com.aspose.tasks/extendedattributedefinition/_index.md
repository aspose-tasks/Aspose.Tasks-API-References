---
title: "ExtendedAttributeDefinition"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar en definition av ett utökat attribut som är associerat med ett projekt."
type: docs
weight: 83
url: /sv/java/com.aspose.tasks/extendedattributedefinition/
---

**Inheritance:**
java.lang.Object
```
public class ExtendedAttributeDefinition
```

Representerar en definition av ett utökat attribut som är associerat med ett projekt.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [addLookupValue(Value value)](#addLookupValue-com.aspose.tasks.Value-) | Lägger till ett värde i den interna uppslagslistan. |
| [compareTo(ExtendedAttributeDefinition o)](#compareTo-com.aspose.tasks.ExtendedAttributeDefinition-) | Jämför detta objekt med en annan instans av @\{code ExtendedAttributeDefinition\} klassen. |
| [createExtendedAttribute()](#createExtendedAttribute--) | Skapar ett nytt utökat attribut med fält‑ID som är lika med detta objekts fält‑ID‑värde. |
| [createExtendedAttribute(boolean flagValue)](#createExtendedAttribute-boolean-) | Skapar ett nytt utökat attribut med fält-ID som är lika med detta objekts fält-ID-värde och det angivna flaggvärdet. |
| [createExtendedAttribute(Duration durationValue)](#createExtendedAttribute-com.aspose.tasks.Duration-) | Skapar ett nytt utökat attribut med fält-ID som är lika med detta objekts fält-ID-värde och det angivna varaktighetsvärdet. |
| [createExtendedAttribute(Value lookupValue)](#createExtendedAttribute-com.aspose.tasks.Value-) | Skapar ett nytt utökat attribut länkat till angivet [Value](../../com.aspose.tasks/value)-objekt. |
| [createExtendedAttribute(String textValue)](#createExtendedAttribute-java.lang.String-) | Skapar ett nytt utökat attribut med fält-ID som är lika med detta objekts fält-ID-värde och det angivna textvärdet. |
| [createExtendedAttribute(BigDecimal numericValue)](#createExtendedAttribute-java.math.BigDecimal-) | Skapar ett nytt utökat attribut med fält-ID som är lika med detta objekts fält-ID-värde och det angivna numeriska värdet. |
| [createExtendedAttribute(Date dateTimeValue)](#createExtendedAttribute-java.util.Date-) | Skapar ett nytt utökat attribut med fält-ID som är lika med detta objekts fält-ID-värde och det angivna datumvärdet. |
| [createLookupResourceDefinition(int customFieldType, int fieldId, String alias)](#createLookupResourceDefinition-int-int-java.lang.String-) | Fabrikmetod som skapar en definition av ett utökat attribut med uppslagning. |
| [createLookupResourceDefinition(int fieldId, String alias)](#createLookupResourceDefinition-int-java.lang.String-) | Fabrikmetod som skapar en definition av ett utökat attribut med uppslagning. |
| [createLookupTaskDefinition(int customFieldType, int fieldId, String alias)](#createLookupTaskDefinition-int-int-java.lang.String-) | Fabrikmetod som skapar en definition av ett utökat attribut med uppslagning. |
| [createLookupTaskDefinition(int fieldId, String alias)](#createLookupTaskDefinition-int-java.lang.String-) | Fabrikmetod som skapar en definition av ett utökat attribut med uppslagning. |
| [createResourceDefinition(int customFieldType, int fieldId, String alias)](#createResourceDefinition-int-int-java.lang.String-) | Fabrikmetod som skapar en enkel definition av ett utökat attribut, som Microsoft Project visar som "None". |
| [createResourceDefinition(int fieldId, String alias)](#createResourceDefinition-int-java.lang.String-) | Fabrikmetod som skapar en enkel definition av ett utökat attribut, som Microsoft Project visar som "None". |
| [createTaskDefinition(int customFieldType, int fieldId, String alias)](#createTaskDefinition-int-int-java.lang.String-) | Fabrikmetod som skapar en enkel definition av ett utökat attribut, som Microsoft Project visar som "None". |
| [createTaskDefinition(int fieldId, String alias)](#createTaskDefinition-int-java.lang.String-) | Fabrikmetod som skapar en enkel definition av ett utökat attribut, som Microsoft Project visar som "None". |
| [equals(Object obj)](#equals-java.lang.Object-) | Returnerar en flagga som indikerar om denna instans är lika med det angivna objektet. |
| [getAlias()](#getAlias--) | Hämtar aliaset för ett anpassat fält. |
| [getAppendNewValues()](#getAppendNewValues--) | Hämtar ett värde som indikerar om nya värden som läggs till i ett projekt automatiskt läggs till i listan. |
| [getAutoRollDown()](#getAutoRollDown--) | Hämtar ett värde som indikerar om en automatisk nedrullning till tilldelningar är aktiverad. |
| [getCalculationType()](#getCalculationType--) | Hämtar beräkningstypen för det anpassade attributets värde. |
| [getCfType()](#getCfType--) | Hämtar typen av ett anpassat fält. |
| [getDefault()](#getDefault--) | Hämtar standardvärdet i listan. |
| [getDefaultGuid()](#getDefaultGuid--) | Hämtar GUID för standarduppslagsposten. |
| [getElementType()](#getElementType--) | Hämtar om det utökade attributet är associerat med en uppgift, en resurs eller en tilldelning. |
| [getFieldId()](#getFieldId--) | Hämtar motsvarigheten till projekt-ID för ett anpassat fält. |
| [getFieldName()](#getFieldName--) | Hämtar namnet på ett anpassat fält. |
| [getFormula()](#getFormula--) | Hämtar formeln som Microsoft Project använder för att fylla i ett anpassat uppgiftsfält. |
| [getGraphicalIndicator()](#getGraphicalIndicator--) | Hämtar information om grafiska indikatorer som är associerade med det utökade attributet. |
| [getGuid()](#getGuid--) | Hämtar GUID för ett anpassat fält. |
| [getLookupUid()](#getLookupUid--) | Hämtar GUID för uppslagstabellen som är associerad med ett anpassat fält. |
| [getMaxMultiValues()](#getMaxMultiValues--) | Hämtar det maximala antalet värden du kan ange i en urvalslista. |
| [getParentProject()](#getParentProject--) | Hämtar överordnat projekt för [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition)-instansen. |
| [getPhoneticsAlias()](#getPhoneticsAlias--) | Hämtar den fonetiska uttalningen av aliaset för ett anpassat fält. |
| [getRestrictValues()](#getRestrictValues--) | Hämtar ett värde som indikerar om värdena för det anpassade fältet är begränsade till värden i `ValueList`([getValueList()](../../com.aspose.tasks/extendedattributedefinition\#getValueList--)/ [setValueList(List)](../../com.aspose.tasks/extendedattributedefinition\#setValueList-List-Value--)). |
| [getRollupType()](#getRollupType--) | Hämtar hur sammanställningar beräknas. |
| [getSecondaryGuid()](#getSecondaryGuid--) | Hämtar den sekundära GUID:n för det utökade attributet. |
| [getSecondaryPid()](#getSecondaryPid--) | Hämtar den sekundära PID:n för ett anpassat fält. |
| [getSummaryRowsCalculationType()](#getSummaryRowsCalculationType--) | Hämtar typen av beräkning av det anpassade attributets värde för summeringsrader. |
| [getUserDef()](#getUserDef--) | Hämtar ett värde som indikerar om ett anpassat fält är användardefinierat. |
| [getValueList()](#getValueList--) | Hämtar List&lt;Value&gt; ValueList. |
| [getValuelistSortOrder()](#getValuelistSortOrder--) | Hämtar hur värdelistor sorteras. |
| [hashCode()](#hashCode--) | Returnerar en hashkod för instansen av klassen [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition). |
| [removeLookupValue(Value value)](#removeLookupValue-com.aspose.tasks.Value-) | Tar bort ett värde från den interna uppslagslistan. |
| [setAlias(String value)](#setAlias-java.lang.String-) | Ställer in aliaset för ett anpassat fält. |
| [setAppendNewValues(boolean value)](#setAppendNewValues-boolean-) | Ställer in ett värde som indikerar om nya värden som läggs till i ett projekt automatiskt läggs till i listan. |
| [setAutoRollDown(boolean value)](#setAutoRollDown-boolean-) | Ställer in ett värde som indikerar om en automatisk nedrullning till tilldelningar är aktiverad. |
| [setCalculationType(int value)](#setCalculationType-int-) | Ställer in typen av beräkning av det anpassade attributets värde. |
| [setDefault(String value)](#setDefault-java.lang.String-) | Ställer in standardvärdet i listan. |
| [setDefaultGuid(String value)](#setDefaultGuid-java.lang.String-) | Ställer in GUID:n för standarduppslagsposten. |
| [setElementType(int value)](#setElementType-int-) | Ställer in att det utökade attributet är associerat med en uppgift, en resurs eller en tilldelning. |
| [setFieldId(String value)](#setFieldId-java.lang.String-) | Ställer in motsvarigheten till projekt‑id för ett anpassat fält. |
| [setFormula(String value)](#setFormula-java.lang.String-) | Ställer in formeln som Microsoft Project använder för att fylla i ett anpassat uppgiftsfält. |
| [setGraphicalIndicator(GraphicalIndicatorsInfo value)](#setGraphicalIndicator-com.aspose.tasks.GraphicalIndicatorsInfo-) | Ställer in grafisk indikatorinformation som är associerad med det utökade attributet. |
| [setGuid(String value)](#setGuid-java.lang.String-) | Ställer in GUID:n för ett anpassat fält. |
| [setMaxMultiValues(int value)](#setMaxMultiValues-int-) | Ställer in det maximala antalet värden du kan ange i en urvalslista. |
| [setPhoneticsAlias(String value)](#setPhoneticsAlias-java.lang.String-) | Ställer in den fonetiska uttalningen av aliaset för ett anpassat fält. |
| [setRestrictValues(boolean value)](#setRestrictValues-boolean-) | Ställer in ett värde som indikerar om värdena för det anpassade fältet är begränsade till värden i `ValueList`([getValueList()](../../com.aspose.tasks/extendedattributedefinition\#getValueList--)/ [setValueList(List)](../../com.aspose.tasks/extendedattributedefinition\#setValueList-List-Value--)). |
| [setRollupType(int value)](#setRollupType-int-) | Ställer in hur summeringar beräknas. |
| [setSecondaryGuid(String value)](#setSecondaryGuid-java.lang.String-) | Ställer in den sekundära GUID för utökad attribut. |
| [setSecondaryPid(String value)](#setSecondaryPid-java.lang.String-) | Ställer in den sekundära PID för ett anpassat fält. |
| [setSummaryRowsCalculationType(int value)](#setSummaryRowsCalculationType-int-) | Ställer in beräkningstypen för det anpassade attributets värde i sammanfattningsrader. |
| [setUserDef(boolean value)](#setUserDef-boolean-) | Ställer in ett värde som indikerar om ett anpassat fält är användardefinierat. |
| [setValuelistSortOrder(int value)](#setValuelistSortOrder-int-) | Ställer in hur värdelistor sorteras. |
### addLookupValue(Value value) {#addLookupValue-com.aspose.tasks.Value-}
```
public final void addLookupValue(Value value)
```


Lägger till ett värde i den interna uppslagslistan. Detta är ett föredraget sätt för manipulationer med `ValueList`([getValueList()](../../com.aspose/tasks/extendedattributedefinition\#getValueList--)/ [setValueList(List)](../../com.aspose.tasks/extendedattributedefinition\#setValueList-List-Value--)).

--------------------

&gt; ```
&gt; Använd den här koden för att lägga till ett nytt Value till uppslagslistan:
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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | lookupValue | [Value](../../com.aspose.tasks/value) | Det angivna [Value](../../com.aspose.tasks/value) objektet. |

--------------------

`lookupValue` bör tidigare ha lagts till i [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) med hjälp av [addLookupValue(Value)](../../com.aspose.tasks/extendedattributedefinition\#addLookupValue-Value-) metoden. |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class linked with specified [Value](../../com.aspose.tasks/value) item.
### createExtendedAttribute(String textValue) {#createExtendedAttribute-java.lang.String-}
```
public final ExtendedAttribute createExtendedAttribute(String textValue)
```


Skapar ett nytt utökat attribut med fält-ID som är lika med detta objekts fält-ID-värde och det angivna textvärdet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| textValue | java.lang.String | Det angivna textvärdet. |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class with the fieldID which equals to this object's fieldID value.
### createExtendedAttribute(BigDecimal numericValue) {#createExtendedAttribute-java.math.BigDecimal-}
```
public final ExtendedAttribute createExtendedAttribute(BigDecimal numericValue)
```


Skapar ett nytt utökat attribut med fält-ID som är lika med detta objekts fält-ID-värde och det angivna numeriska värdet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| numericValue | java.math.BigDecimal | Det angivna numeriska värdet. |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class with the fieldID which equals to this object's fieldID value.
### createExtendedAttribute(Date dateTimeValue) {#createExtendedAttribute-java.util.Date-}
```
public final ExtendedAttribute createExtendedAttribute(Date dateTimeValue)
```


Skapar ett nytt utökat attribut med fält-ID som är lika med detta objekts fält-ID-värde och det angivna datumvärdet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| dateTimeValue | java.util.Date | Det angivna datetime‑värdet. |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class with the fieldID which equals to this object's fieldID value.
### createLookupResourceDefinition(int customFieldType, int fieldId, String alias) {#createLookupResourceDefinition-int-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createLookupResourceDefinition(int customFieldType, int fieldId, String alias)
```


Fabriksmetod som skapar en definition av ett utökat attribut med uppslagning. Den har `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) lika med [CalculationType.Lookup](../../com.aspose.tasks/calculationtype\#Lookup) och kan endast användas i resurser. Du måste ange `customFieldType`, `fieldId` och `alias` när du anropar den här metoden.

--------------------

&gt; ```
&gt; Använd detta exempel för att skapa en anpassad fältdefinition för en resurs med uppslagning och sedan fylla den med textvärden:
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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldId | int | Det angivna [ExtendedAttributeResource](../../com.aspose.tasks/extendedattributeresource) fält-ID:t. |
| alias | java.lang.String | Det angivna String‑aliaset. |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `fieldId` and `alias`.
### createLookupTaskDefinition(int customFieldType, int fieldId, String alias) {#createLookupTaskDefinition-int-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createLookupTaskDefinition(int customFieldType, int fieldId, String alias)
```


Fabriksmetod som skapar en definition av ett utökat attribut med uppslagning. Den har `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) lika med [CalculationType.Lookup](../../com.aspose.tasks/calculationtype\#Lookup) och kan endast användas i uppgifter. Du måste ange `customFieldType`, `fieldId` och `alias` när du anropar den här metoden.

--------------------

&gt; ```
&gt; Använd detta exempel för att skapa en anpassad fältdefinition för en uppgift med uppslagning och sedan fylla den med textvärden:
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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldId | int | Det angivna [ExtendedAttributeTask](../../com.aspose.tasks/extendedattributetask) fält-ID:t. |
| alias | java.lang.String | Det angivna String‑aliaset. |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `fieldId` and `alias`.
### createResourceDefinition(int customFieldType, int fieldId, String alias) {#createResourceDefinition-int-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createResourceDefinition(int customFieldType, int fieldId, String alias)
```


Fabriksmetod som skapar en enkel definition av ett utökat attribut, som Microsoft Project visar som "None". Den har `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) lika med [CalculationType.None](../../com.aspose.tasks/calculationtype\#None) och kan endast användas i resurser. Du måste ange `customFieldType`, `fieldId` och `alias` när du anropar den här metoden.

--------------------

&gt; ```
&gt; Använd detta exempel för att skapa en anpassad textfältdefinition:
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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldId | int | Det angivna [ExtendedAttributeResource](../../com.aspose.tasks/extendedattributeresource) fält-ID:t. |
| alias | java.lang.String | Det angivna String‑aliaset. |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `fieldId` and `alias`.
### createTaskDefinition(int customFieldType, int fieldId, String alias) {#createTaskDefinition-int-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createTaskDefinition(int customFieldType, int fieldId, String alias)
```


Fabrikmetod som skapar en enkel definition av utökad attribut, som Microsoft Project visar som "None". Den har `CalculationType`([getCalculationType()](../../com.aspose/tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose/tasks/extendedattributedefinition\#setCalculationType-int-)) lika med [CalculationType.None](../../com.aspose/tasks/calculationtype\#None) och kan endast användas i Uppgifter. Du måste ange `customFieldType`, `fieldId` och `alias` när du anropar denna metod.

--------------------

&gt; ```
&gt; Använd detta exempel för att skapa en anpassad textfältdefinition:
&gt; ``````

ExtendedAttributeDefinition taskTextAttr = ExtendedAttributeDefinition.createTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text27, "Mitt anpassade fält");
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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldId | int | Det angivna [ExtendedAttributeTask](../../com.aspose.tasks/extendedattributetask) fält-ID:t. |
| alias | java.lang.String | Det angivna String‑aliaset. |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `fieldId` and `alias`.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Returnerar en flagga som indikerar om denna instans är lika med det angivna objektet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| obj | java.lang.Object | det specificerade objektet att jämföra med denna instans. |

**Returns:**
boolean - en flagga som indikerar om denna instans är lika med det specificerade objektet.
### getAlias() {#getAlias--}
```
public final String getAlias()
```


Hämtar aliaset för ett anpassat fält.

**Returns:**
java.lang.String - aliaset för ett anpassat fält.
### getAppendNewValues() {#getAppendNewValues--}
```
public final boolean getAppendNewValues()
```


Hämtar ett värde som indikerar om nya värden som läggs till i ett projekt automatiskt läggs till i listan.

--------------------

Stöds för närvarande för MSP 2003/2007 Xml och MSP 2003 mpp-format.

**Returns:**
boolean - ett värde som indikerar om nya värden som läggs till i ett projekt automatiskt läggs till i listan.
### getAutoRollDown() {#getAutoRollDown--}
```
public final boolean getAutoRollDown()
```


Hämtar ett värde som indikerar om en automatisk nedrullning till tilldelningar är aktiverad.

**Returns:**
boolean - ett värde som indikerar om en automatisk nedrullning till tilldelningar är aktiverad.
### getCalculationType() {#getCalculationType--}
```
public final int getCalculationType()
```


Hämtar beräkningstypen för det anpassade attributets värde.

**Returns:**
int - typen av beräkning av det anpassade attributets värde.
### getCfType() {#getCfType--}
```
public final int getCfType()
```


Hämtar typen av ett anpassat fält.

**Returns:**
int - typen av ett anpassat fält.
### getDefault() {#getDefault--}
```
public final String getDefault()
```


Hämtar standardvärdet i listan.

--------------------

Stöds för närvarande för MSP 2003/2007 Xml och MSP 2003 mpp-format.

**Returns:**
java.lang.String - standardvärdet i listan.
### getDefaultGuid() {#getDefaultGuid--}
```
public final String getDefaultGuid()
```


Hämtar GUID för standarduppslagsposten.

**Returns:**
java.lang.String - Guid för standarduppslagsposten.
### getElementType() {#getElementType--}
```
public final int getElementType()
```


Hämtar om det utökade attributet är associerat med en uppgift, en resurs eller en tilldelning.

**Returns:**
int - det utökade attributet är associerat med en uppgift, en resurs eller en tilldelning.
### getFieldId() {#getFieldId--}
```
public final String getFieldId()
```


Hämtar motsvarigheten till projekt-id för ett anpassat fält. Använd strängrepresentationen av en konstant från klassen [ExtendedAttributeTask](../../com.aspose/tasks/extendedattributetask) för att ange `FieldId`([getFieldId()](../../com.aspose/tasks/extendedattributedefinition\#getFieldId--)/ [setFieldId(String)](../../com.aspose/tasks/extendedattributedefinition\#setFieldId-String-)) egenskapen.

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

Det föredragna sättet att sätta `FieldId`([getFieldId()](../../com.aspose/tasks/extendedattributedefinition\#getFieldId--)/ [setFieldId(String)](../../com.aspose/tasks/extendedattributedefinition\#setFieldId-String-)) egenskapen är att skapa [ExtendedAttributeDefinition](../../com.aspose/tasks/extendedattributedefinition) med en av de dedikerade fabriksmetoderna såsom [createTaskDefinition(int, String)](../../com.aspose/tasks/extendedattributedefinition\#createTaskDefinition-int--String-) eller [createLookupTaskDefinition(int, int, String)](../../com.aspose/tasks/extendedattributedefinition\#createLookupTaskDefinition-int--int--String-).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | korresponderar med projekt‑id för ett anpassat fält. |

### setFormula(String value) {#setFormula-java.lang.String-}
```
public final void setFormula(String value)
```


Ställer in formeln som Microsoft Project använder för att fylla i ett anpassat uppgiftsfält.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | formeln som Microsoft Project använder för att fylla i ett anpassat uppgiftsfält. |

### setGraphicalIndicator(GraphicalIndicatorsInfo value) {#setGraphicalIndicator-com.aspose.tasks.GraphicalIndicatorsInfo-}
```
public final void setGraphicalIndicator(GraphicalIndicatorsInfo value)
```


Ställer in information om grafiska indikatorer som är associerad med det utökade attributet. Gäller för MPP-format.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [GraphicalIndicatorsInfo](../../com.aspose.tasks/graphicalindicatorsinfo) | information om grafiska indikatorer som är associerad med det utökade attributet. |

### setGuid(String value) {#setGuid-java.lang.String-}
```
public final void setGuid(String value)
```


Ställer in GUID:n för ett anpassat fält.

--------------------

Stöds för närvarande endast för Xml-format.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | Guid för ett anpassat fält. |

### setMaxMultiValues(int value) {#setMaxMultiValues-int-}
```
public final void setMaxMultiValues(int value)
```


Ställer in det maximala antalet värden du kan ange i en urvalslista.

--------------------

Stöds för närvarande endast för Xml-format.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | det maximala antalet värden du kan ange i en urvalslista. |

### setPhoneticsAlias(String value) {#setPhoneticsAlias-java.lang.String-}
```
public final void setPhoneticsAlias(String value)
```


Ställer in den fonetiska uttalningen av aliaset för ett anpassat fält.

--------------------

Stöds för närvarande endast för Xml-format.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | den fonetiska uttalningen av aliaset för ett anpassat fält. |

### setRestrictValues(boolean value) {#setRestrictValues-boolean-}
```
public final void setRestrictValues(boolean value)
```


Ställer in ett värde som indikerar om värdena för det anpassade fältet är begränsade till värden i `ValueList`([getValueList()](../../com.aspose.tasks/extendedattributedefinition\#getValueList--)/ [setValueList(List)](../../com.aspose.tasks/extendedattributedefinition\#setValueList-List-Value--)).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som indikerar om de anpassade fältvärdena är begränsade till värden i |

### setRollupType(int value) {#setRollupType-int-}
```
public final void setRollupType(int value)
```


Ställer in hur summeringar beräknas.

--------------------

Skrivning stöds för närvarande endast för Xml-format.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | sättet som summeringar beräknas på. |

### setSecondaryGuid(String value) {#setSecondaryGuid-java.lang.String-}
```
public final void setSecondaryGuid(String value)
```


Ställer in den sekundära GUID för utökad attribut.

--------------------

Detta är nytt för MS Project 2010‑egenskapen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | det sekundära guid för det utökade attributet. |

### setSecondaryPid(String value) {#setSecondaryPid-java.lang.String-}
```
public final void setSecondaryPid(String value)
```


Ställer in den sekundära PID för ett anpassat fält.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | det sekundära PID för ett anpassat fält. |

### setSummaryRowsCalculationType(int value) {#setSummaryRowsCalculationType-int-}
```
public final void setSummaryRowsCalculationType(int value)
```


Ställer in beräkningstypen för det anpassade attributets värde i sammanfattningsrader.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | typen av beräkning av det anpassade attributets värde för sammanfattningsrader. |

### setUserDef(boolean value) {#setUserDef-boolean-}
```
public final void setUserDef(boolean value)
```


Ställer in ett värde som indikerar om ett anpassat fält är användardefinierat.

--------------------

Stöds för närvarande endast för Xml-format.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som indikerar om ett anpassat fält är användardefinierat. |

### setValuelistSortOrder(int value) {#setValuelistSortOrder-int-}
```
public final void setValuelistSortOrder(int value)
```


Ställer in hur värdelistor sorteras. Värdena är: 0=Fallande, 1=Stigande.

--------------------

Stöds för närvarande för MSP 2003/2007 Xml och MSP 2003 mpp-format.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | sättet som värdelistor sorteras på. |

