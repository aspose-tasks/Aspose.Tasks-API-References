---
title: "ExtendedAttributeDefinition"
second_title: "Aspose.Tasks for Java API Reference"
description: "Rappresenta una definizione di attributo esteso associata a un progetto."
type: docs
weight: 83
url: /it/java/com.aspose.tasks/extendedattributedefinition/
---

**Inheritance:**
java.lang.Object
```
public class ExtendedAttributeDefinition
```

Rappresenta una definizione di attributo esteso associata a un progetto.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [addLookupValue(Value value)](#addLookupValue-com.aspose.tasks.Value-) | Aggiunge un valore all'elenco interno di ricerca. |
| [compareTo(ExtendedAttributeDefinition o)](#compareTo-com.aspose.tasks.ExtendedAttributeDefinition-) | Confronta questo oggetto con un'altra istanza della classe @\{code ExtendedAttributeDefinition\}. |
| [createExtendedAttribute()](#createExtendedAttribute--) | Crea un nuovo attributo esteso con l'ID campo che è uguale al valore dell'ID campo di questo oggetto. |
| [createExtendedAttribute(boolean flagValue)](#createExtendedAttribute-boolean-) | Crea un nuovo attributo esteso con l'ID campo che è uguale al valore dell'ID campo di questo oggetto e al valore di flag specificato. |
| [createExtendedAttribute(Duration durationValue)](#createExtendedAttribute-com.aspose.tasks.Duration-) | Crea un nuovo attributo esteso con l'ID campo che è uguale al valore dell'ID campo di questo oggetto e al valore di durata specificato. |
| [createExtendedAttribute(Value lookupValue)](#createExtendedAttribute-com.aspose.tasks.Value-) | Crea un nuovo attributo esteso collegato all'elemento [Value](../../com.aspose.tasks/value) specificato. |
| [createExtendedAttribute(String textValue)](#createExtendedAttribute-java.lang.String-) | Crea un nuovo attributo esteso con l'ID campo che è uguale al valore dell'ID campo di questo oggetto e al valore di testo specificato. |
| [createExtendedAttribute(BigDecimal numericValue)](#createExtendedAttribute-java.math.BigDecimal-) | Crea un nuovo attributo esteso con l'ID campo che è uguale al valore dell'ID campo di questo oggetto e al valore numerico specificato. |
| [createExtendedAttribute(Date dateTimeValue)](#createExtendedAttribute-java.util.Date-) | Crea un nuovo attributo esteso con l'ID campo che è uguale al valore dell'ID campo di questo oggetto e al valore di data specificato. |
| [createLookupResourceDefinition(int customFieldType, int fieldId, String alias)](#createLookupResourceDefinition-int-int-java.lang.String-) | Metodo factory che crea una definizione di attributo esteso con ricerca. |
| [createLookupResourceDefinition(int fieldId, String alias)](#createLookupResourceDefinition-int-java.lang.String-) | Metodo factory che crea una definizione di attributo esteso con ricerca. |
| [createLookupTaskDefinition(int customFieldType, int fieldId, String alias)](#createLookupTaskDefinition-int-int-java.lang.String-) | Metodo factory che crea una definizione di attributo esteso con ricerca. |
| [createLookupTaskDefinition(int fieldId, String alias)](#createLookupTaskDefinition-int-java.lang.String-) | Metodo factory che crea una definizione di attributo esteso con ricerca. |
| [createResourceDefinition(int customFieldType, int fieldId, String alias)](#createResourceDefinition-int-int-java.lang.String-) | Metodo factory che crea una definizione di attributo esteso semplice, che Microsoft Project mostra come "None". |
| [createResourceDefinition(int fieldId, String alias)](#createResourceDefinition-int-java.lang.String-) | Metodo factory che crea una definizione di attributo esteso semplice, che Microsoft Project mostra come "None". |
| [createTaskDefinition(int customFieldType, int fieldId, String alias)](#createTaskDefinition-int-int-java.lang.String-) | Metodo factory che crea una definizione di attributo esteso semplice, che Microsoft Project mostra come "None". |
| [createTaskDefinition(int fieldId, String alias)](#createTaskDefinition-int-java.lang.String-) | Metodo factory che crea una definizione di attributo esteso semplice, che Microsoft Project mostra come "None". |
| [equals(Object obj)](#equals-java.lang.Object-) | Restituisce un flag che indica se questa istanza è uguale all'oggetto specificato. |
| [getAlias()](#getAlias--) | Ottiene l'alias di un campo personalizzato. |
| [getAppendNewValues()](#getAppendNewValues--) | Ottiene un valore che indica se i nuovi valori aggiunti a un progetto vengono aggiunti automaticamente all'elenco. |
| [getAutoRollDown()](#getAutoRollDown--) | Ottiene un valore che indica se è abilitato un roll down automatico alle assegnazioni. |
| [getCalculationType()](#getCalculationType--) | Ottiene il tipo di calcolo del valore dell'attributo personalizzato. |
| [getCfType()](#getCfType--) | Ottiene il tipo di un campo personalizzato. |
| [getDefault()](#getDefault--) | Ottiene il valore predefinito nell'elenco. |
| [getDefaultGuid()](#getDefaultGuid--) | Ottiene il Guid della voce della tabella di ricerca predefinita. |
| [getElementType()](#getElementType--) | Ottiene se l'attributo esteso è associato a un'attività, a una risorsa o a un'assegnazione. |
| [getFieldId()](#getFieldId--) | Ottiene corrisponde all'ID progetto di un campo personalizzato. |
| [getFieldName()](#getFieldName--) | Ottiene il nome di un campo personalizzato. |
| [getFormula()](#getFormula--) | Ottiene la formula che Microsoft Project utilizza per popolare un campo attività personalizzato. |
| [getGraphicalIndicator()](#getGraphicalIndicator--) | Ottiene le informazioni degli indicatori grafici associate all'attributo esteso. |
| [getGuid()](#getGuid--) | Ottiene il Guid di un campo personalizzato. |
| [getLookupUid()](#getLookupUid--) | Ottiene un Guid della tabella di ricerca associata a un campo personalizzato. |
| [getMaxMultiValues()](#getMaxMultiValues--) | Ottiene il numero massimo di valori che è possibile impostare in un elenco a discesa. |
| [getParentProject()](#getParentProject--) | Ottiene il progetto padre per l'istanza di [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition). |
| [getPhoneticsAlias()](#getPhoneticsAlias--) | Ottiene la pronuncia fonetica dell'alias di un campo personalizzato. |
| [getRestrictValues()](#getRestrictValues--) | Ottiene un valore che indica se i valori del campo personalizzato sono limitati ai valori nella `ValueList`([getValueList()](../../com.aspose.tasks/extendedattributedefinition\#getValueList--)/ [setValueList(List)](../../com.aspose.tasks/extendedattributedefinition\#setValueList-List-Value--)). |
| [getRollupType()](#getRollupType--) | Ottiene il modo in cui i rollup vengono calcolati. |
| [getSecondaryGuid()](#getSecondaryGuid--) | Ottiene il guid secondario dell'attributo esteso. |
| [getSecondaryPid()](#getSecondaryPid--) | Ottiene il PID secondario di un campo personalizzato. |
| [getSummaryRowsCalculationType()](#getSummaryRowsCalculationType--) | Ottiene il tipo di calcolo del valore dell'attributo personalizzato per le righe di riepilogo. |
| [getUserDef()](#getUserDef--) | Ottiene un valore che indica se un campo personalizzato è definito dall'utente. |
| [getValueList()](#getValueList--) | Ottiene la List&lt;Value&gt; ValueList. |
| [getValuelistSortOrder()](#getValuelistSortOrder--) | Ottiene il modo in cui le liste di valori sono ordinate. |
| [hashCode()](#hashCode--) | Restituisce un codice hash per l'istanza della classe [ExtendedAttributeDefinition](../../com.aspose/tasks/extendedattributedefinition). |
| [removeLookupValue(Value value)](#removeLookupValue-com.aspose.tasks.Value-) | Rimuove un valore dall'elenco di ricerca interno. |
| [setAlias(String value)](#setAlias-java.lang.String-) | Imposta l'alias di un campo personalizzato. |
| [setAppendNewValues(boolean value)](#setAppendNewValues-boolean-) | Imposta un valore che indica se i nuovi valori aggiunti a un progetto vengono aggiunti automaticamente all'elenco. |
| [setAutoRollDown(boolean value)](#setAutoRollDown-boolean-) | Imposta un valore che indica se è abilitata una propagazione automatica alle assegnazioni. |
| [setCalculationType(int value)](#setCalculationType-int-) | Imposta il tipo di calcolo del valore dell'attributo personalizzato. |
| [setDefault(String value)](#setDefault-java.lang.String-) | Imposta il valore predefinito nell'elenco. |
| [setDefaultGuid(String value)](#setDefaultGuid-java.lang.String-) | Imposta il GUID della voce predefinita della tabella di ricerca. |
| [setElementType(int value)](#setElementType-int-) | Imposta se l'attributo esteso è associato a un'attività, a una risorsa o a un'assegnazione. |
| [setFieldId(String value)](#setFieldId-java.lang.String-) | Imposta la corrispondenza con l'ID progetto di un campo personalizzato. |
| [setFormula(String value)](#setFormula-java.lang.String-) | Imposta la formula che Microsoft Project utilizza per popolare un campo attività personalizzato. |
| [setGraphicalIndicator(GraphicalIndicatorsInfo value)](#setGraphicalIndicator-com.aspose.tasks.GraphicalIndicatorsInfo-) | Imposta le informazioni degli indicatori grafici associate all'attributo esteso. |
| [setGuid(String value)](#setGuid-java.lang.String-) | Imposta il GUID di un campo personalizzato. |
| [setMaxMultiValues(int value)](#setMaxMultiValues-int-) | Imposta il numero massimo di valori che è possibile impostare in un elenco a discesa. |
| [setPhoneticsAlias(String value)](#setPhoneticsAlias-java.lang.String-) | Imposta la pronuncia fonetica dell'alias di un campo personalizzato. |
| [setRestrictValues(boolean value)](#setRestrictValues-boolean-) | Imposta un valore che indica se i valori del campo personalizzato sono limitati ai valori nella `ValueList`([getValueList()](../../com.aspose.tasks/extendedattributedefinition\#getValueList--)/ [setValueList(List)](../../com.aspose.tasks/extendedattributedefinition\#setValueList-List-Value--)). |
| [setRollupType(int value)](#setRollupType-int-) | Imposta il modo in cui vengono calcolati i rollup. |
| [setSecondaryGuid(String value)](#setSecondaryGuid-java.lang.String-) | Imposta il GUID secondario dell'attributo esteso. |
| [setSecondaryPid(String value)](#setSecondaryPid-java.lang.String-) | Imposta il PID secondario di un campo personalizzato. |
| [setSummaryRowsCalculationType(int value)](#setSummaryRowsCalculationType-int-) | Imposta il tipo di calcolo del valore dell'attributo personalizzato per le righe di riepilogo. |
| [setUserDef(boolean value)](#setUserDef-boolean-) | Imposta un valore che indica se un campo personalizzato è definito dall'utente. |
| [setValuelistSortOrder(int value)](#setValuelistSortOrder-int-) | Imposta il modo in cui gli elenchi di valori sono ordinati. |
### addLookupValue(Value value) {#addLookupValue-com.aspose.tasks.Value-}
```
public final void addLookupValue(Value value)
```


Aggiunge un valore all'elenco di ricerca interno. Questo è il modo consigliato per le manipolazioni con la `ValueList`([getValueList()](../../com.aspose.tasks/extendedattributedefinition\#getValueList--)/ [setValueList(List)](../../com.aspose.tasks/extendedattributedefinition\#setValueList-List-Value--)).

--------------------

&gt; ```
&gt; Usa questo codice per aggiungere un nuovo valore all'elenco di ricerca:
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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | lookupValue | [Value](../../com.aspose.tasks/value) | L'elemento [Value](../../com.aspose.tasks/value) specificato. |

--------------------

`lookupValue` dovrebbe essere aggiunto in precedenza al [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) usando il metodo [addLookupValue(Value)](../../com.aspose.tasks/extendedattributedefinition\#addLookupValue-Value-) . |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class linked with specified [Value](../../com.aspose.tasks/value) item.
### createExtendedAttribute(String textValue) {#createExtendedAttribute-java.lang.String-}
```
public final ExtendedAttribute createExtendedAttribute(String textValue)
```


Crea un nuovo attributo esteso con l'ID campo che è uguale al valore dell'ID campo di questo oggetto e al valore di testo specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| textValue | java.lang.String | Il valore di testo specificato. |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class with the fieldID which equals to this object's fieldID value.
### createExtendedAttribute(BigDecimal numericValue) {#createExtendedAttribute-java.math.BigDecimal-}
```
public final ExtendedAttribute createExtendedAttribute(BigDecimal numericValue)
```


Crea un nuovo attributo esteso con l'ID campo che è uguale al valore dell'ID campo di questo oggetto e al valore numerico specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| numericValue | java.math.BigDecimal | Il valore numerico specificato. |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class with the fieldID which equals to this object's fieldID value.
### createExtendedAttribute(Date dateTimeValue) {#createExtendedAttribute-java.util.Date-}
```
public final ExtendedAttribute createExtendedAttribute(Date dateTimeValue)
```


Crea un nuovo attributo esteso con l'ID campo che è uguale al valore dell'ID campo di questo oggetto e al valore di data specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| dateTimeValue | java.util.Date | Il valore datetime specificato. |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class with the fieldID which equals to this object's fieldID value.
### createLookupResourceDefinition(int customFieldType, int fieldId, String alias) {#createLookupResourceDefinition-int-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createLookupResourceDefinition(int customFieldType, int fieldId, String alias)
```


Metodo di fabbrica che crea una definizione di attributo esteso con lookup. Ha `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) uguale a [CalculationType.Lookup](../../com.aspose.tasks/calculationtype\#Lookup) e può essere usato solo nelle Risorse. È necessario specificare `customFieldType`, `fieldId` e `alias` quando si chiama questo metodo.

--------------------

&gt; ```
&gt; Usa questo esempio per creare una definizione di campo personalizzato per una risorsa con lookup e poi riempirla con valori di testo:
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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldId | int | L'ID del campo specificato [ExtendedAttributeResource](../../com.aspose.tasks/extendedattributeresource). |
| alias | java.lang.String | L'alias String specificato. |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `fieldId` and `alias`.
### createLookupTaskDefinition(int customFieldType, int fieldId, String alias) {#createLookupTaskDefinition-int-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createLookupTaskDefinition(int customFieldType, int fieldId, String alias)
```


Metodo di fabbrica che crea una definizione di attributo esteso con lookup. Ha `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) uguale a [CalculationType.Lookup](../../com.aspose.tasks/calculationtype\#Lookup) e può essere usato solo nei Task. È necessario specificare `customFieldType`, `fieldId` e `alias` quando si chiama questo metodo.

--------------------

&gt; ```
&gt; Utilizza questo esempio per creare una definizione di campo personalizzato per un'attività con lookup e poi riempirla con valori di testo:
&gt; ``````

ExtendedAttributeDefinition taskTextAttr = ExtendedAttributeDefinition.createLookupTaskDefinition(CustomFieldType.Text, ExtendedAttributeResource.Text27, \"My custom field\");
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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldId | int | L'ID del campo specificato [ExtendedAttributeTask](../../com.aspose.tasks/extendedattributetask). |
| alias | java.lang.String | L'alias String specificato. |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `fieldId` and `alias`.
### createResourceDefinition(int customFieldType, int fieldId, String alias) {#createResourceDefinition-int-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createResourceDefinition(int customFieldType, int fieldId, String alias)
```


Metodo di fabbrica che crea una semplice definizione di attributo esteso, che Microsoft Project mostra come \"None\". Ha `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) uguale a [CalculationType.None](../../com.aspose.tasks/calculationtype\#None) e può essere usato solo nelle Risorse. È necessario specificare `customFieldType`, `fieldId` e `alias` quando si chiama questo metodo.

--------------------

&gt; ```
&gt; Utilizza questo esempio per creare una definizione di campo di testo personalizzato:
&gt; ``````

ExtendedAttributeDefinition resourceTextAttr = ExtendedAttributeDefinition.createResourceDefinition(CustomFieldType.Text, ExtendedAttributeResource.Text27, \"My custom field\");
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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldId | int | L'ID del campo specificato [ExtendedAttributeResource](../../com.aspose.tasks/extendedattributeresource). |
| alias | java.lang.String | L'alias String specificato. |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `fieldId` and `alias`.
### createTaskDefinition(int customFieldType, int fieldId, String alias) {#createTaskDefinition-int-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createTaskDefinition(int customFieldType, int fieldId, String alias)
```


Metodo di fabbrica che crea una semplice definizione di attributo esteso, che Microsoft Project mostra come \"None\". Ha `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) uguale a [CalculationType.None](../../com.aspose.tasks/calculationtype\#None) e può essere usato solo nei Task. È necessario specificare `customFieldType`, `fieldId` e `alias` quando si chiama questo metodo.

--------------------

&gt; ```
&gt; Utilizza questo esempio per creare una definizione di campo di testo personalizzato:
&gt; ``````

ExtendedAttributeDefinition taskTextAttr = ExtendedAttributeDefinition.createTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text27, \"My custom field\");
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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldId | int | L'ID del campo specificato [ExtendedAttributeTask](../../com.aspose.tasks/extendedattributetask). |
| alias | java.lang.String | L'alias String specificato. |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `fieldId` and `alias`.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Restituisce un flag che indica se questa istanza è uguale all'oggetto specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| obj | java.lang.Object | l'oggetto specificato da confrontare con questa istanza. |

**Returns:**
boolean - un flag che indica se questa istanza è uguale all'oggetto specificato.
### getAlias() {#getAlias--}
```
public final String getAlias()
```


Ottiene l'alias di un campo personalizzato.

**Returns:**
java.lang.String - l'alias di un campo personalizzato.
### getAppendNewValues() {#getAppendNewValues--}
```
public final boolean getAppendNewValues()
```


Ottiene un valore che indica se i nuovi valori aggiunti a un progetto vengono aggiunti automaticamente all'elenco.

--------------------

Attualmente supportato per i formati MSP 2003/2007 Xml e MSP 2003 mpp.

**Returns:**
boolean - un valore che indica se i nuovi valori aggiunti a un progetto sono automaticamente aggiunti all'elenco.
### getAutoRollDown() {#getAutoRollDown--}
```
public final boolean getAutoRollDown()
```


Ottiene un valore che indica se è abilitato un roll down automatico alle assegnazioni.

**Returns:**
boolean - un valore che indica se è abilitato un roll down automatico alle assegnazioni.
### getCalculationType() {#getCalculationType--}
```
public final int getCalculationType()
```


Ottiene il tipo di calcolo del valore dell'attributo personalizzato.

**Returns:**
int - il tipo di calcolo del valore dell'attributo personalizzato.
### getCfType() {#getCfType--}
```
public final int getCfType()
```


Ottiene il tipo di un campo personalizzato.

**Returns:**
int - il tipo di un campo personalizzato.
### getDefault() {#getDefault--}
```
public final String getDefault()
```


Ottiene il valore predefinito nell'elenco.

--------------------

Attualmente supportato per i formati MSP 2003/2007 Xml e MSP 2003 mpp.

**Returns:**
java.lang.String - il valore predefinito nell'elenco.
### getDefaultGuid() {#getDefaultGuid--}
```
public final String getDefaultGuid()
```


Ottiene il Guid della voce della tabella di ricerca predefinita.

**Returns:**
java.lang.String - il Guid della voce predefinita della tabella di ricerca.
### getElementType() {#getElementType--}
```
public final int getElementType()
```


Ottiene se l'attributo esteso è associato a un'attività, a una risorsa o a un'assegnazione.

**Returns:**
int - l'attributo esteso è associato a un'attività, a una risorsa o a un'assegnazione.
### getFieldId() {#getFieldId--}
```
public final String getFieldId()
```


Gets corrisponde all'ID progetto di un campo personalizzato. Usa la rappresentazione stringa di una costante della classe [ExtendedAttributeTask](../../com.aspose.tasks/extendedattributetask) per specificare la proprietà `FieldId`([getFieldId()](../../com.aspose.tasks/extendedattributedefinition\#getFieldId--)/ [setFieldId(String)](../../com.aspose.tasks/extendedattributedefinition\#setFieldId-String-)).

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

Il modo consigliato per impostare la proprietà `FieldId`([getFieldId()](../../com.aspose/tasks/extendedattributedefinition\#getFieldId--)/ [setFieldId(String)](../../com.aspose/tasks/extendedattributedefinition\#setFieldId-String-)) è creare [ExtendedAttributeDefinition](../../com.aspose/tasks/extendedattributedefinition) utilizzando uno dei metodi di fabbrica dedicati come [createTaskDefinition(int, String)](../../com.aspose/tasks/extendedattributedefinition\#createTaskDefinition-int--String-) o [createLookupTaskDefinition(int, int, String)](../../com.aspose/tasks/extendedattributedefinition\#createLookupTaskDefinition-int--int--String-).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | corrisponde all'ID progetto di un campo personalizzato. |

### setFormula(String value) {#setFormula-java.lang.String-}
```
public final void setFormula(String value)
```


Imposta la formula che Microsoft Project utilizza per popolare un campo attività personalizzato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | la formula che Microsoft Project utilizza per popolare un campo attività personalizzato. |

### setGraphicalIndicator(GraphicalIndicatorsInfo value) {#setGraphicalIndicator-com.aspose.tasks.GraphicalIndicatorsInfo-}
```
public final void setGraphicalIndicator(GraphicalIndicatorsInfo value)
```


Imposta le informazioni degli indicatori grafici associate all'attributo esteso. Applicabile al formato MPP.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [GraphicalIndicatorsInfo](../../com.aspose.tasks/graphicalindicatorsinfo) | informazioni degli indicatori grafici associate all'attributo esteso. |

### setGuid(String value) {#setGuid-java.lang.String-}
```
public final void setGuid(String value)
```


Imposta il GUID di un campo personalizzato.

--------------------

Attualmente supportato solo per il formato Xml.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | il GUID di un campo personalizzato. |

### setMaxMultiValues(int value) {#setMaxMultiValues-int-}
```
public final void setMaxMultiValues(int value)
```


Imposta il numero massimo di valori che è possibile impostare in un elenco a discesa.

--------------------

Attualmente supportato solo per il formato Xml.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | il numero massimo di valori che è possibile impostare in un elenco a discesa. |

### setPhoneticsAlias(String value) {#setPhoneticsAlias-java.lang.String-}
```
public final void setPhoneticsAlias(String value)
```


Imposta la pronuncia fonetica dell'alias di un campo personalizzato.

--------------------

Attualmente supportato solo per il formato Xml.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | la pronuncia fonetica dell'alias di un campo personalizzato. |

### setRestrictValues(boolean value) {#setRestrictValues-boolean-}
```
public final void setRestrictValues(boolean value)
```


Imposta un valore che indica se i valori del campo personalizzato sono limitati ai valori nella `ValueList`([getValueList()](../../com.aspose.tasks/extendedattributedefinition\#getValueList--)/ [setValueList(List)](../../com.aspose.tasks/extendedattributedefinition\#setValueList-List-Value--)).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se i valori del campo personalizzato sono limitati ai valori in |

### setRollupType(int value) {#setRollupType-int-}
```
public final void setRollupType(int value)
```


Imposta il modo in cui vengono calcolati i rollup.

--------------------

Scrittura attualmente supportata solo per il formato Xml.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | il modo in cui vengono calcolati i rollup. |

### setSecondaryGuid(String value) {#setSecondaryGuid-java.lang.String-}
```
public final void setSecondaryGuid(String value)
```


Imposta il GUID secondario dell'attributo esteso.

--------------------

Questa è una nuova proprietà per MS Project 2010.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | il GUID secondario dell'attributo esteso. |

### setSecondaryPid(String value) {#setSecondaryPid-java.lang.String-}
```
public final void setSecondaryPid(String value)
```


Imposta il PID secondario di un campo personalizzato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | il PID secondario di un campo personalizzato. |

### setSummaryRowsCalculationType(int value) {#setSummaryRowsCalculationType-int-}
```
public final void setSummaryRowsCalculationType(int value)
```


Imposta il tipo di calcolo del valore dell'attributo personalizzato per le righe di riepilogo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | il tipo di calcolo del valore dell'attributo personalizzato per le righe di riepilogo. |

### setUserDef(boolean value) {#setUserDef-boolean-}
```
public final void setUserDef(boolean value)
```


Imposta un valore che indica se un campo personalizzato è definito dall'utente.

--------------------

Attualmente supportato solo per il formato Xml.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se un campo personalizzato è definito dall'utente. |

### setValuelistSortOrder(int value) {#setValuelistSortOrder-int-}
```
public final void setValuelistSortOrder(int value)
```


Imposta il modo in cui le liste di valori sono ordinate. I valori sono: 0=Decrescente, 1=Crescente.

--------------------

Attualmente supportato per i formati MSP 2003/2007 Xml e MSP 2003 mpp.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | il modo in cui le liste di valori sono ordinate. |

