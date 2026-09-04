---
title: "ExtendedAttributeDefinition"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt eine erweiterte Attributdefinition dar, die mit einem Projekt verknüpft ist."
type: docs
weight: 83
url: /de/java/com.aspose.tasks/extendedattributedefinition/
---

**Inheritance:**
java.lang.Object
```
public class ExtendedAttributeDefinition
```

Stellt eine erweiterte Attributdefinition dar, die mit einem Projekt verknüpft ist.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [addLookupValue(Value value)](#addLookupValue-com.aspose.tasks.Value-) | Fügt einen Wert zur internen Lookup-Liste hinzu. |
| [compareTo(ExtendedAttributeDefinition o)](#compareTo-com.aspose.tasks.ExtendedAttributeDefinition-) | Vergleicht dieses Objekt mit einer anderen Instanz der @\{code ExtendedAttributeDefinition\} Klasse. |
| [createExtendedAttribute()](#createExtendedAttribute--) | Erstellt ein neues erweitertes Attribut mit der Feld-ID, die dem Feld-ID-Wert dieses Objekts entspricht. |
| [createExtendedAttribute(boolean flagValue)](#createExtendedAttribute-boolean-) | Erstellt ein neues erweitertes Attribut mit der Feld-ID, die dem Feld-ID-Wert dieses Objekts entspricht und dem angegebenen Flag-Wert. |
| [createExtendedAttribute(Duration durationValue)](#createExtendedAttribute-com.aspose.tasks.Duration-) | Erstellt ein neues erweitertes Attribut mit der Feld-ID, die dem Feld-ID-Wert dieses Objekts entspricht und dem angegebenen Dauerwert. |
| [createExtendedAttribute(Value lookupValue)](#createExtendedAttribute-com.aspose.tasks.Value-) | Erstellt ein neues erweitertes Attribut, das mit dem angegebenen [Value](../../com.aspose.tasks/value) Element verknüpft ist. |
| [createExtendedAttribute(String textValue)](#createExtendedAttribute-java.lang.String-) | Erstellt ein neues erweitertes Attribut mit der Feld-ID, die dem Feld-ID-Wert dieses Objekts entspricht und dem angegebenen Textwert. |
| [createExtendedAttribute(BigDecimal numericValue)](#createExtendedAttribute-java.math.BigDecimal-) | Erstellt ein neues erweitertes Attribut mit der Feld-ID, die dem Feld-ID-Wert dieses Objekts entspricht und dem angegebenen numerischen Wert. |
| [createExtendedAttribute(Date dateTimeValue)](#createExtendedAttribute-java.util.Date-) | Erstellt ein neues erweitertes Attribut mit der Feld-ID, die dem Feld-ID-Wert dieses Objekts entspricht und dem angegebenen Datumswert. |
| [createLookupResourceDefinition(int customFieldType, int fieldId, String alias)](#createLookupResourceDefinition-int-int-java.lang.String-) | Factory-Methode, die eine erweiterte Attributdefinition mit Lookup erstellt. |
| [createLookupResourceDefinition(int fieldId, String alias)](#createLookupResourceDefinition-int-java.lang.String-) | Factory-Methode, die eine erweiterte Attributdefinition mit Lookup erstellt. |
| [createLookupTaskDefinition(int customFieldType, int fieldId, String alias)](#createLookupTaskDefinition-int-int-java.lang.String-) | Factory-Methode, die eine erweiterte Attributdefinition mit Lookup erstellt. |
| [createLookupTaskDefinition(int fieldId, String alias)](#createLookupTaskDefinition-int-java.lang.String-) | Factory-Methode, die eine erweiterte Attributdefinition mit Lookup erstellt. |
| [createResourceDefinition(int customFieldType, int fieldId, String alias)](#createResourceDefinition-int-int-java.lang.String-) | Factory-Methode, die eine einfache erweiterte Attributdefinition erstellt, die Microsoft Project als "None" anzeigt. |
| [createResourceDefinition(int fieldId, String alias)](#createResourceDefinition-int-java.lang.String-) | Factory-Methode, die eine einfache erweiterte Attributdefinition erstellt, die Microsoft Project als "None" anzeigt. |
| [createTaskDefinition(int customFieldType, int fieldId, String alias)](#createTaskDefinition-int-int-java.lang.String-) | Factory-Methode, die eine einfache erweiterte Attributdefinition erstellt, die Microsoft Project als "None" anzeigt. |
| [createTaskDefinition(int fieldId, String alias)](#createTaskDefinition-int-java.lang.String-) | Factory-Methode, die eine einfache erweiterte Attributdefinition erstellt, die Microsoft Project als "None" anzeigt. |
| [equals(Object obj)](#equals-java.lang.Object-) | Gibt ein Flag zurück, das angibt, ob diese Instanz dem angegebenen Objekt gleich ist. |
| [getAlias()](#getAlias--) | Liefert den Alias eines benutzerdefinierten Feldes. |
| [getAppendNewValues()](#getAppendNewValues--) | Liefert einen Wert, der angibt, ob neue zu einem Projekt hinzugefügte Werte automatisch zur Liste hinzugefügt werden. |
| [getAutoRollDown()](#getAutoRollDown--) | Liefert einen Wert, der angibt, ob ein automatisches Herunterrollen zu Zuweisungen aktiviert ist. |
| [getCalculationType()](#getCalculationType--) | Liefert den Berechnungstyp des Werts des benutzerdefinierten Attributs. |
| [getCfType()](#getCfType--) | Liefert den Typ eines benutzerdefinierten Feldes. |
| [getDefault()](#getDefault--) | Liefert den Standardwert in der Liste. |
| [getDefaultGuid()](#getDefaultGuid--) | Liefert die GUID des Standard-Lookup-Tabelleneintrags. |
| [getElementType()](#getElementType--) | Ermittelt, ob das erweiterte Attribut mit einer Aufgabe, einer Ressource oder einer Zuweisung verknüpft ist. |
| [getFieldId()](#getFieldId--) | Liefert die Projekt-ID, die einem benutzerdefinierten Feld entspricht. |
| [getFieldName()](#getFieldName--) | Liefert den Namen eines benutzerdefinierten Feldes. |
| [getFormula()](#getFormula--) | Liefert die Formel, die Microsoft Project verwendet, um ein benutzerdefiniertes Aufgabefeld zu füllen. |
| [getGraphicalIndicator()](#getGraphicalIndicator--) | Liefert grafische Indikatorinformationen, die dem erweiterten Attribut zugeordnet sind. |
| [getGuid()](#getGuid--) | Liefert die GUID eines benutzerdefinierten Feldes. |
| [getLookupUid()](#getLookupUid--) | Liefert die GUID der Lookup-Tabelle, die einem benutzerdefinierten Feld zugeordnet ist. |
| [getMaxMultiValues()](#getMaxMultiValues--) | Liefert die maximale Anzahl von Werten, die Sie in einer Auswahlliste festlegen können. |
| [getParentProject()](#getParentProject--) | Liefert das übergeordnete Projekt für die Instanz von [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition). |
| [getPhoneticsAlias()](#getPhoneticsAlias--) | Liefert die phonetische Aussprache des Alias eines benutzerdefinierten Feldes. |
| [getRestrictValues()](#getRestrictValues--) | Liefert einen Wert, der angibt, ob die Werte des benutzerdefinierten Feldes auf Werte in der `ValueList`([getValueList()](../../com.aspose.tasks/extendedattributedefinition\#getValueList--)/ [setValueList(List)](../../com.aspose.tasks/extendedattributedefinition\#setValueList-List-Value--)) beschränkt sind. |
| [getRollupType()](#getRollupType--) | Liefert die Art und Weise, wie Rollups berechnet werden. |
| [getSecondaryGuid()](#getSecondaryGuid--) | Liefert die sekundäre GUID des erweiterten Attributs. |
| [getSecondaryPid()](#getSecondaryPid--) | Liefert die sekundäre PID eines benutzerdefinierten Feldes. |
| [getSummaryRowsCalculationType()](#getSummaryRowsCalculationType--) | Liefert den Berechnungstyp des Werts des benutzerdefinierten Attributs für Summenzeilen. |
| [getUserDef()](#getUserDef--) | Liefert einen Wert, der angibt, ob ein benutzerdefiniertes Feld vom Benutzer definiert ist. |
| [getValueList()](#getValueList--) | Liefert die List&lt;Value&gt; ValueList. |
| [getValuelistSortOrder()](#getValuelistSortOrder--) | Liefert die Art und Weise, wie Wertlisten sortiert werden. |
| [hashCode()](#hashCode--) | Gibt einen Hashcode für die Instanz der Klasse [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) zurück. |
| [removeLookupValue(Value value)](#removeLookupValue-com.aspose.tasks.Value-) | Entfernt einen Wert aus der internen Lookup-Liste. |
| [setAlias(String value)](#setAlias-java.lang.String-) | Setzt den Alias eines benutzerdefinierten Feldes. |
| [setAppendNewValues(boolean value)](#setAppendNewValues-boolean-) | Setzt einen Wert, der angibt, ob neue Werte, die zu einem Projekt hinzugefügt werden, automatisch zur Liste hinzugefügt werden. |
| [setAutoRollDown(boolean value)](#setAutoRollDown-boolean-) | Setzt einen Wert, der angibt, ob ein automatisches Herunterrollen zu Zuweisungen aktiviert ist. |
| [setCalculationType(int value)](#setCalculationType-int-) | Setzt den Berechnungstyp des Werts des benutzerdefinierten Attributs. |
| [setDefault(String value)](#setDefault-java.lang.String-) | Setzt den Standardwert in der Liste. |
| [setDefaultGuid(String value)](#setDefaultGuid-java.lang.String-) | Setzt die GUID des Standard‑Lookup‑Tabelleneintrags. |
| [setElementType(int value)](#setElementType-int-) | Legt fest, dass das erweiterte Attribut mit einer Aufgabe, einer Ressource oder einer Zuweisung verknüpft ist. |
| [setFieldId(String value)](#setFieldId-java.lang.String-) | Setzt die Projekt-ID eines benutzerdefinierten Feldes. |
| [setFormula(String value)](#setFormula-java.lang.String-) | Setzt die Formel, die Microsoft Project verwendet, um ein benutzerdefiniertes Aufgabefeld zu füllen. |
| [setGraphicalIndicator(GraphicalIndicatorsInfo value)](#setGraphicalIndicator-com.aspose.tasks.GraphicalIndicatorsInfo-) | Setzt eine grafische Indikator-Info, die mit dem erweiterten Attribut verknüpft ist. |
| [setGuid(String value)](#setGuid-java.lang.String-) | Setzt die GUID eines benutzerdefinierten Feldes. |
| [setMaxMultiValues(int value)](#setMaxMultiValues-int-) | Setzt die maximale Anzahl von Werten, die Sie in einer Auswahlliste festlegen können. |
| [setPhoneticsAlias(String value)](#setPhoneticsAlias-java.lang.String-) | Setzt die phonetische Aussprache des Alias eines benutzerdefinierten Feldes. |
| [setRestrictValues(boolean value)](#setRestrictValues-boolean-) | Setzt einen Wert, der angibt, ob die Werte des benutzerdefinierten Feldes auf Werte in der `ValueList`([getValueList()](../../com.aspose/tasks/extendedattributedefinition\#getValueList--)/ [setValueList(List)](../../com.aspose/tasks/extendedattributedefinition\#setValueList-List-Value--)) beschränkt sind. |
| [setRollupType(int value)](#setRollupType-int-) | Setzt die Art und Weise, wie Rollups berechnet werden. |
| [setSecondaryGuid(String value)](#setSecondaryGuid-java.lang.String-) | Setzt die sekundäre GUID des erweiterten Attributs. |
| [setSecondaryPid(String value)](#setSecondaryPid-java.lang.String-) | Setzt die sekundäre PID eines benutzerdefinierten Feldes. |
| [setSummaryRowsCalculationType(int value)](#setSummaryRowsCalculationType-int-) | Setzt den Berechnungstyp des Werts des benutzerdefinierten Attributs für Zusammenfassungszeilen. |
| [setUserDef(boolean value)](#setUserDef-boolean-) | Setzt einen Wert, der angibt, ob ein benutzerdefiniertes Feld vom Benutzer definiert ist. |
| [setValuelistSortOrder(int value)](#setValuelistSortOrder-int-) | Setzt die Art und Weise, wie Wertlisten sortiert werden. |
### addLookupValue(Value value) {#addLookupValue-com.aspose.tasks.Value-}
```
public final void addLookupValue(Value value)
```


Fügt einen Wert zur internen Lookup-Liste hinzu. Dies ist ein bevorzugter Weg für Manipulationen mit der `ValueList`([getValueList()](../../com.aspose/tasks/extendedattributedefinition\#getValueList--)/ [setValueList(List)](../../com.aspose/tasks/extendedattributedefinition\#setValueList-List-Value--)).

--------------------

&gt; ```
&gt; Verwenden Sie diesen Code, um einen neuen Wert zur Lookup-Liste hinzuzufügen:
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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | lookupValue | [Value](../../com.aspose.tasks/value) | Das angegebene [Value](../../com.aspose.tasks/value) Element. |

--------------------

`lookupValue` sollte zuvor zur [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) mittels der Methode [addLookupValue(Value)](../../com.aspose.tasks/extendedattributedefinition\#addLookupValue-Value-) hinzugefügt worden sein. |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class linked with specified [Value](../../com.aspose.tasks/value) item.
### createExtendedAttribute(String textValue) {#createExtendedAttribute-java.lang.String-}
```
public final ExtendedAttribute createExtendedAttribute(String textValue)
```


Erstellt ein neues erweitertes Attribut mit der Feld-ID, die dem Feld-ID-Wert dieses Objekts entspricht und dem angegebenen Textwert.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| textValue | java.lang.String | Der angegebene Textwert. |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class with the fieldID which equals to this object's fieldID value.
### createExtendedAttribute(BigDecimal numericValue) {#createExtendedAttribute-java.math.BigDecimal-}
```
public final ExtendedAttribute createExtendedAttribute(BigDecimal numericValue)
```


Erstellt ein neues erweitertes Attribut mit der Feld-ID, die dem Feld-ID-Wert dieses Objekts entspricht und dem angegebenen numerischen Wert.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| numericValue | java.math.BigDecimal | Der angegebene numerische Wert. |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class with the fieldID which equals to this object's fieldID value.
### createExtendedAttribute(Date dateTimeValue) {#createExtendedAttribute-java.util.Date-}
```
public final ExtendedAttribute createExtendedAttribute(Date dateTimeValue)
```


Erstellt ein neues erweitertes Attribut mit der Feld-ID, die dem Feld-ID-Wert dieses Objekts entspricht und dem angegebenen Datumswert.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| dateTimeValue | java.util.Date | Der angegebene Datum/Uhrzeit-Wert. |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class with the fieldID which equals to this object's fieldID value.
### createLookupResourceDefinition(int customFieldType, int fieldId, String alias) {#createLookupResourceDefinition-int-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createLookupResourceDefinition(int customFieldType, int fieldId, String alias)
```


Factory-Methode, die eine erweiterte Attributdefinition mit Lookup erstellt. Sie hat `CalculationType`([getCalculationType()](../../com.aspose/tasks/extendedattributedefinition\\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose/tasks/extendedattributedefinition\\#setCalculationType-int-)) gleich zu [CalculationType.Lookup](../../com.aspose.tasks/calculationtype\\#Lookup) und kann nur in Ressourcen verwendet werden. Sie müssen `customFieldType`, `fieldId` und `alias` angeben, wenn Sie diese Methode aufrufen.

--------------------

&gt; ```
&gt; Verwenden Sie dieses Beispiel, um eine benutzerdefinierte Felddefinition für eine Ressource mit Lookup zu erstellen und sie anschließend mit Textwerten zu füllen:
&gt; ``````

ExtendedAttributeDefinition resourceTextAttr = ExtendedAttributeDefinition.createLookupResourceDefinition(ExtendedAttributeResource.Text27, \"My custom field\");
resourceTextAttr.addLookupValue(new Value() {{
this.setId(1);
this.setVal("Text value 1");
this.setDescription("Text value description 1");
}});
resourceTextAttr.addLookupValue(new Value() {{
this.setId(2);
this.setVal(\"Text value 2\");
this.setDescription(\"Text value description 2\");
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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fieldId | int | Die angegebene [ExtendedAttributeResource](../../com.aspose.tasks/extendedattributeresource) Feld-ID. |
| alias | java.lang.String | Der angegebene String-Alias. |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `fieldId` and `alias`.
### createLookupTaskDefinition(int customFieldType, int fieldId, String alias) {#createLookupTaskDefinition-int-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createLookupTaskDefinition(int customFieldType, int fieldId, String alias)
```


Factory-Methode, die eine erweiterte Attributdefinition mit Lookup erstellt. Sie hat `CalculationType`([getCalculationType()](../../com.aspose/tasks/extendedattributedefinition\\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose/tasks/extendedattributedefinition\\#setCalculationType-int-)) gleich zu [CalculationType.Lookup](../../com.aspose.tasks/calculationtype\\#Lookup) und kann nur in Aufgaben verwendet werden. Sie müssen `customFieldType`, `fieldId` und `alias` angeben, wenn Sie diese Methode aufrufen.

--------------------

&gt; ```
&gt; Verwenden Sie dieses Beispiel, um eine benutzerdefinierte Felddefinition für eine Aufgabe mit Lookup zu erstellen und sie anschließend mit Textwerten zu füllen:
&gt; ``````

ExtendedAttributeDefinition taskTextAttr = ExtendedAttributeDefinition.createLookupTaskDefinition(CustomFieldType.Text, ExtendedAttributeResource.Text27, \"My custom field\");
taskTextAttr.addLookupValue(new Value() {{
this.setId(1);
this.setVal("Text value 1");
this.setDescription("Text value description 1");
}});
taskTextAttr.addLookupValue(new Value() {{
this.setId(2);
this.setVal(\"Text value 2\");
this.setDescription(\"Text value description 2\");
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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fieldId | int | Die angegebene [ExtendedAttributeTask](../../com.aspose.tasks/extendedattributetask) Feld-ID. |
| alias | java.lang.String | Der angegebene String-Alias. |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `fieldId` and `alias`.
### createResourceDefinition(int customFieldType, int fieldId, String alias) {#createResourceDefinition-int-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createResourceDefinition(int customFieldType, int fieldId, String alias)
```


Factory-Methode, die eine einfache erweiterte Attributdefinition erstellt, die Microsoft Project als \"None\" anzeigt. Sie hat `CalculationType`([getCalculationType()](../../com.aspose/tasks/extendedattributedefinition\\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose/tasks/extendedattributedefinition\\#setCalculationType-int-)) gleich zu [CalculationType.None](../../com.aspose.tasks/calculationtype\\#None) und kann nur in Ressourcen verwendet werden. Sie müssen `customFieldType`, `fieldId` und `alias` angeben, wenn Sie diese Methode aufrufen.

--------------------

&gt; ```
&gt; Verwenden Sie dieses Beispiel, um eine benutzerdefinierte Textfelddefinition zu erstellen:
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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fieldId | int | Die angegebene [ExtendedAttributeResource](../../com.aspose.tasks/extendedattributeresource) Feld-ID. |
| alias | java.lang.String | Der angegebene String-Alias. |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `fieldId` and `alias`.
### createTaskDefinition(int customFieldType, int fieldId, String alias) {#createTaskDefinition-int-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createTaskDefinition(int customFieldType, int fieldId, String alias)
```


Factory-Methode, die eine einfache erweiterte Attributdefinition erstellt, die Microsoft Project als "None" anzeigt. Sie hat `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) entspricht [CalculationType.None](../../com.aspose.tasks/calculationtype\#None) und kann nur in Aufgaben verwendet werden. Sie müssen `customFieldType`, `fieldId` und `alias` angeben, wenn Sie diese Methode aufrufen.

--------------------

&gt; ```
&gt; Verwenden Sie dieses Beispiel, um eine benutzerdefinierte Textfelddefinition zu erstellen:
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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fieldId | int | Die angegebene [ExtendedAttributeTask](../../com.aspose.tasks/extendedattributetask) Feld-ID. |
| alias | java.lang.String | Der angegebene String-Alias. |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `fieldId` and `alias`.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Gibt ein Flag zurück, das angibt, ob diese Instanz dem angegebenen Objekt gleich ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| obj | java.lang.Object | das angegebene Objekt, mit dem diese Instanz verglichen wird. |

**Returns:**
boolean - ein Flag, das angibt, ob diese Instanz dem angegebenen Objekt entspricht.
### getAlias() {#getAlias--}
```
public final String getAlias()
```


Liefert den Alias eines benutzerdefinierten Feldes.

**Returns:**
java.lang.String - der Alias eines benutzerdefinierten Feldes.
### getAppendNewValues() {#getAppendNewValues--}
```
public final boolean getAppendNewValues()
```


Liefert einen Wert, der angibt, ob neue zu einem Projekt hinzugefügte Werte automatisch zur Liste hinzugefügt werden.

--------------------

Derzeit unterstützt für MSP 2003/2007 Xml- und MSP 2003 mpp-Formate.

**Returns:**
boolean - ein Wert, der angibt, ob neue zu einem Projekt hinzugefügte Werte automatisch zur Liste hinzugefügt werden.
### getAutoRollDown() {#getAutoRollDown--}
```
public final boolean getAutoRollDown()
```


Liefert einen Wert, der angibt, ob ein automatisches Herunterrollen zu Zuweisungen aktiviert ist.

**Returns:**
boolean - ein Wert, der angibt, ob ein automatisches Roll-Down zu Zuweisungen aktiviert ist.
### getCalculationType() {#getCalculationType--}
```
public final int getCalculationType()
```


Liefert den Berechnungstyp des Werts des benutzerdefinierten Attributs.

**Returns:**
int - der Berechnungstyp des Werts des benutzerdefinierten Attributs.
### getCfType() {#getCfType--}
```
public final int getCfType()
```


Liefert den Typ eines benutzerdefinierten Feldes.

**Returns:**
int - der Typ eines benutzerdefinierten Feldes.
### getDefault() {#getDefault--}
```
public final String getDefault()
```


Liefert den Standardwert in der Liste.

--------------------

Derzeit unterstützt für MSP 2003/2007 Xml- und MSP 2003 mpp-Formate.

**Returns:**
java.lang.String - der Standardwert in der Liste.
### getDefaultGuid() {#getDefaultGuid--}
```
public final String getDefaultGuid()
```


Liefert die GUID des Standard-Lookup-Tabelleneintrags.

**Returns:**
java.lang.String - die GUID des Standard‑Lookup‑Tabelleneintrags.
### getElementType() {#getElementType--}
```
public final int getElementType()
```


Ermittelt, ob das erweiterte Attribut mit einer Aufgabe, einer Ressource oder einer Zuweisung verknüpft ist.

**Returns:**
int - das erweiterte Attribut ist einem Vorgang, einer Ressource oder einer Zuweisung zugeordnet.
### getFieldId() {#getFieldId--}
```
public final String getFieldId()
```


Gibt die Projekt‑ID eines benutzerdefinierten Feldes zurück. Verwenden Sie die String‑Darstellung einer Konstanten aus der Klasse [ExtendedAttributeTask](../../com.aspose.tasks/extendedattributetask), um die Eigenschaft `FieldId`([getFieldId()](../../com.aspose.tasks/extendedattributedefinition\#getFieldId--)/ [setFieldId(String)](../../com.aspose.tasks/extendedattributedefinition\#setFieldId-String-)) festzulegen.

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

Die bevorzugte Methode, die `FieldId`([getFieldId()](../../com.aspose/tasks/extendedattributedefinition\#getFieldId--)/ [setFieldId(String)](../../com.aspose/tasks/extendedattributedefinition\#setFieldId-String-))‑Eigenschaft zu setzen, besteht darin, [ExtendedAttributeDefinition](../../com.aspose/tasks/extendedattributedefinition) mit einer der dedizierten Fabrikmethoden wie [createTaskDefinition(int, String)](../../com.aspose/tasks/extendedattributedefinition\#createTaskDefinition-int--String-) oder [createLookupTaskDefinition(int, int, String)](../../com.aspose/tasks/extendedattributedefinition\#createLookupTaskDefinition-int--int--String-) zu erstellen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | entspricht der Projekt‑ID eines benutzerdefinierten Feldes. |

### setFormula(String value) {#setFormula-java.lang.String-}
```
public final void setFormula(String value)
```


Setzt die Formel, die Microsoft Project verwendet, um ein benutzerdefiniertes Aufgabefeld zu füllen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | die Formel, die Microsoft Project verwendet, um ein benutzerdefiniertes Aufgabefeld zu füllen. |

### setGraphicalIndicator(GraphicalIndicatorsInfo value) {#setGraphicalIndicator-com.aspose.tasks.GraphicalIndicatorsInfo-}
```
public final void setGraphicalIndicator(GraphicalIndicatorsInfo value)
```


Setzt eine grafische Indikator‑Info, die dem erweiterten Attribut zugeordnet ist. Gilt für das MPP‑Format.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [GraphicalIndicatorsInfo](../../com.aspose.tasks/graphicalindicatorsinfo) | eine grafische Hinweisinformation, die mit dem erweiterten Attribut verknüpft ist. |

### setGuid(String value) {#setGuid-java.lang.String-}
```
public final void setGuid(String value)
```


Setzt die GUID eines benutzerdefinierten Feldes.

--------------------

Derzeit nur für das Xml-Format unterstützt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | die GUID eines benutzerdefinierten Feldes. |

### setMaxMultiValues(int value) {#setMaxMultiValues-int-}
```
public final void setMaxMultiValues(int value)
```


Setzt die maximale Anzahl von Werten, die Sie in einer Auswahlliste festlegen können.

--------------------

Derzeit nur für das Xml-Format unterstützt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | die maximale Anzahl von Werten, die Sie in einer Auswahlliste festlegen können. |

### setPhoneticsAlias(String value) {#setPhoneticsAlias-java.lang.String-}
```
public final void setPhoneticsAlias(String value)
```


Setzt die phonetische Aussprache des Alias eines benutzerdefinierten Feldes.

--------------------

Derzeit nur für das Xml-Format unterstützt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | die phonetische Aussprache des Alias eines benutzerdefinierten Feldes. |

### setRestrictValues(boolean value) {#setRestrictValues-boolean-}
```
public final void setRestrictValues(boolean value)
```


Setzt einen Wert, der angibt, ob die Werte des benutzerdefinierten Feldes auf Werte in der `ValueList`([getValueList()](../../com.aspose/tasks/extendedattributedefinition\#getValueList--)/ [setValueList(List)](../../com.aspose/tasks/extendedattributedefinition\#setValueList-List-Value--)) beschränkt sind.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob die Werte des benutzerdefinierten Feldes auf Werte im |

### setRollupType(int value) {#setRollupType-int-}
```
public final void setRollupType(int value)
```


Setzt die Art und Weise, wie Rollups berechnet werden.

--------------------

Schreiben derzeit nur für das Xml-Format unterstützt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | die Art und Weise, wie Rollups berechnet werden. |

### setSecondaryGuid(String value) {#setSecondaryGuid-java.lang.String-}
```
public final void setSecondaryGuid(String value)
```


Setzt die sekundäre GUID des erweiterten Attributs.

--------------------

Dies ist eine neue Eigenschaft für MS Project 2010.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | die sekundäre GUID des erweiterten Attributs. |

### setSecondaryPid(String value) {#setSecondaryPid-java.lang.String-}
```
public final void setSecondaryPid(String value)
```


Setzt die sekundäre PID eines benutzerdefinierten Feldes.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | die sekundäre PID eines benutzerdefinierten Feldes. |

### setSummaryRowsCalculationType(int value) {#setSummaryRowsCalculationType-int-}
```
public final void setSummaryRowsCalculationType(int value)
```


Setzt den Berechnungstyp des Werts des benutzerdefinierten Attributs für Zusammenfassungszeilen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | der Berechnungstyp des Werts des benutzerdefinierten Attributs für Zusammenfassungszeilen. |

### setUserDef(boolean value) {#setUserDef-boolean-}
```
public final void setUserDef(boolean value)
```


Setzt einen Wert, der angibt, ob ein benutzerdefiniertes Feld vom Benutzer definiert ist.

--------------------

Derzeit nur für das Xml-Format unterstützt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob ein benutzerdefiniertes Feld vom Benutzer definiert ist. |

### setValuelistSortOrder(int value) {#setValuelistSortOrder-int-}
```
public final void setValuelistSortOrder(int value)
```


Legt fest, wie Wertlisten sortiert werden. Werte sind: 0=Absteigend, 1=Aufsteigend.

--------------------

Derzeit unterstützt für MSP 2003/2007 Xml- und MSP 2003 mpp-Formate.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | die Art und Weise, wie Wertlisten sortiert werden. |

