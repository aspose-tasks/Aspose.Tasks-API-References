---
title: "ExtendedAttributeDefinition"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Représente une définition d'attribut étendu associée à un projet."
type: docs
weight: 83
url: /fr/java/com.aspose.tasks/extendedattributedefinition/
---

**Inheritance:**
java.lang.Object
```
public class ExtendedAttributeDefinition
```

Représente une définition d'attribut étendu associée à un projet.
## Méthodes

| Méthode | Description |
| --- | --- |
| [addLookupValue(Value value)](#addLookupValue-com.aspose.tasks.Value-) | Ajoute une valeur à la liste de recherche interne. |
| [compareTo(ExtendedAttributeDefinition o)](#compareTo-com.aspose.tasks.ExtendedAttributeDefinition-) | Compare cet objet avec une autre instance de la classe @\{code ExtendedAttributeDefinition\}. |
| [createExtendedAttribute()](#createExtendedAttribute--) | Crée un nouvel attribut étendu avec l'ID de champ qui est égal à la valeur de l'ID de champ de cet objet. |
| [createExtendedAttribute(boolean flagValue)](#createExtendedAttribute-boolean-) | Crée un nouvel attribut étendu avec l'ID de champ qui est égal à la valeur de l'ID de champ de cet objet et la valeur du drapeau spécifiée. |
| [createExtendedAttribute(Duration durationValue)](#createExtendedAttribute-com.aspose.tasks.Duration-) | Crée un nouvel attribut étendu avec l'ID de champ qui est égal à la valeur de l'ID de champ de cet objet et la valeur de durée spécifiée. |
| [createExtendedAttribute(Value lookupValue)](#createExtendedAttribute-com.aspose.tasks.Value-) | Crée un nouvel attribut étendu lié à l'élément [Value](../../com.aspose.tasks/value) spécifié. |
| [createExtendedAttribute(String textValue)](#createExtendedAttribute-java.lang.String-) | Crée un nouvel attribut étendu avec l'ID de champ qui est égal à la valeur de l'ID de champ de cet objet et la valeur de texte spécifiée. |
| [createExtendedAttribute(BigDecimal numericValue)](#createExtendedAttribute-java.math.BigDecimal-) | Crée un nouvel attribut étendu avec l'ID de champ qui est égal à la valeur de l'ID de champ de cet objet et la valeur numérique spécifiée. |
| [createExtendedAttribute(Date dateTimeValue)](#createExtendedAttribute-java.util.Date-) | Crée un nouvel attribut étendu avec l'ID de champ qui est égal à la valeur de l'ID de champ de cet objet et la valeur de date spécifiée. |
| [createLookupResourceDefinition(int customFieldType, int fieldId, String alias)](#createLookupResourceDefinition-int-int-java.lang.String-) | Méthode d'usine qui crée une définition d'attribut étendu avec recherche. |
| [createLookupResourceDefinition(int fieldId, String alias)](#createLookupResourceDefinition-int-java.lang.String-) | Méthode d'usine qui crée une définition d'attribut étendu avec recherche. |
| [createLookupTaskDefinition(int customFieldType, int fieldId, String alias)](#createLookupTaskDefinition-int-int-java.lang.String-) | Méthode d'usine qui crée une définition d'attribut étendu avec recherche. |
| [createLookupTaskDefinition(int fieldId, String alias)](#createLookupTaskDefinition-int-java.lang.String-) | Méthode d'usine qui crée une définition d'attribut étendu avec recherche. |
| [createResourceDefinition(int customFieldType, int fieldId, String alias)](#createResourceDefinition-int-int-java.lang.String-) | Méthode d'usine qui crée une définition d'attribut étendu simple, que Microsoft Project affiche comme \"None\". |
| [createResourceDefinition(int fieldId, String alias)](#createResourceDefinition-int-java.lang.String-) | Méthode d'usine qui crée une définition d'attribut étendu simple, que Microsoft Project affiche comme \"None\". |
| [createTaskDefinition(int customFieldType, int fieldId, String alias)](#createTaskDefinition-int-int-java.lang.String-) | Méthode d'usine qui crée une définition d'attribut étendu simple, que Microsoft Project affiche comme \"None\". |
| [createTaskDefinition(int fieldId, String alias)](#createTaskDefinition-int-java.lang.String-) | Méthode d'usine qui crée une définition d'attribut étendu simple, que Microsoft Project affiche comme \"None\". |
| [equals(Object obj)](#equals-java.lang.Object-) | Renvoie un indicateur indiquant si cette instance est égale à l'objet spécifié. |
| [getAlias()](#getAlias--) | Obtient l'alias d'un champ personnalisé. |
| [getAppendNewValues()](#getAppendNewValues--) | Obtient une valeur indiquant si les nouvelles valeurs ajoutées à un projet sont automatiquement ajoutées à la liste. |
| [getAutoRollDown()](#getAutoRollDown--) | Obtient une valeur indiquant si un déploiement automatique vers les affectations est activé. |
| [getCalculationType()](#getCalculationType--) | Obtient le type de calcul de la valeur de l'attribut personnalisé. |
| [getCfType()](#getCfType--) | Obtient le type d'un champ personnalisé. |
| [getDefault()](#getDefault--) | Obtient la valeur par défaut dans la liste. |
| [getDefaultGuid()](#getDefaultGuid--) | Obtient le GUID de l'entrée de la table de recherche par défaut. |
| [getElementType()](#getElementType--) | Obtient l'attribut étendu associé à une tâche, une ressource ou une affectation. |
| [getFieldId()](#getFieldId--) | Obtient la correspondance avec l'ID du projet d'un champ personnalisé. |
| [getFieldName()](#getFieldName--) | Obtient le nom d'un champ personnalisé. |
| [getFormula()](#getFormula--) | Obtient la formule que Microsoft Project utilise pour remplir un champ de tâche personnalisé. |
| [getGraphicalIndicator()](#getGraphicalIndicator--) | Obtient les informations des indicateurs graphiques associées à l'attribut étendu. |
| [getGuid()](#getGuid--) | Obtient le GUID d'un champ personnalisé. |
| [getLookupUid()](#getLookupUid--) | Obtient le GUID de la table de recherche associée à un champ personnalisé. |
| [getMaxMultiValues()](#getMaxMultiValues--) | Obtient le nombre maximal de valeurs que vous pouvez définir dans une liste déroulante. |
| [getParentProject()](#getParentProject--) | Obtient le projet parent pour l'instance [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition). |
| [getPhoneticsAlias()](#getPhoneticsAlias--) | Obtient la prononciation phonétique de l'alias d'un champ personnalisé. |
| [getRestrictValues()](#getRestrictValues--) | Obtient une valeur indiquant si les valeurs du champ personnalisé sont limitées aux valeurs de la `ValueList`([getValueList()](../../com.aspose.tasks/extendedattributedefinition\#getValueList--)/ [setValueList(List)](../../com.aspose.tasks/extendedattributedefinition\#setValueList-List-Value--)). |
| [getRollupType()](#getRollupType--) | Obtient la façon dont les rollups sont calculés. |
| [getSecondaryGuid()](#getSecondaryGuid--) | Obtient le GUID secondaire de l'attribut étendu. |
| [getSecondaryPid()](#getSecondaryPid--) | Obtient le PID secondaire d'un champ personnalisé. |
| [getSummaryRowsCalculationType()](#getSummaryRowsCalculationType--) | Obtient le type de calcul de la valeur de l'attribut personnalisé pour les lignes de synthèse. |
| [getUserDef()](#getUserDef--) | Obtient une valeur indiquant si un champ personnalisé est défini par l'utilisateur. |
| [getValueList()](#getValueList--) | Obtient la List&lt;Value&gt; ValueList. |
| [getValuelistSortOrder()](#getValuelistSortOrder--) | Obtient la façon dont les listes de valeurs sont triées. |
| [hashCode()](#hashCode--) | Renvoie un code de hachage pour l'instance de la classe [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition). |
| [removeLookupValue(Value value)](#removeLookupValue-com.aspose.tasks.Value-) | Supprime une valeur de la liste de recherche interne. |
| [setAlias(String value)](#setAlias-java.lang.String-) | Définit l'alias d'un champ personnalisé. |
| [setAppendNewValues(boolean value)](#setAppendNewValues-boolean-) | Définit une valeur indiquant si les nouvelles valeurs ajoutées à un projet sont automatiquement ajoutées à la liste. |
| [setAutoRollDown(boolean value)](#setAutoRollDown-boolean-) | Définit une valeur indiquant si un déploiement automatique vers les affectations est activé. |
| [setCalculationType(int value)](#setCalculationType-int-) | Définit le type de calcul de la valeur de l'attribut personnalisé. |
| [setDefault(String value)](#setDefault-java.lang.String-) | Définit la valeur par défaut dans la liste. |
| [setDefaultGuid(String value)](#setDefaultGuid-java.lang.String-) | Définit le GUID de l'entrée de la table de recherche par défaut. |
| [setElementType(int value)](#setElementType-int-) | Définit que l'attribut étendu est associé à une tâche, une ressource ou une affectation. |
| [setFieldId(String value)](#setFieldId-java.lang.String-) | Définit correspond à l'identifiant du projet d'un champ personnalisé. |
| [setFormula(String value)](#setFormula-java.lang.String-) | Définit la formule que Microsoft Project utilise pour remplir un champ de tâche personnalisé. |
| [setGraphicalIndicator(GraphicalIndicatorsInfo value)](#setGraphicalIndicator-com.aspose.tasks.GraphicalIndicatorsInfo-) | Définit les informations d'indicateurs graphiques associées à l'attribut étendu. |
| [setGuid(String value)](#setGuid-java.lang.String-) | Définit le GUID d'un champ personnalisé. |
| [setMaxMultiValues(int value)](#setMaxMultiValues-int-) | Définit le nombre maximal de valeurs que vous pouvez définir dans une liste déroulante. |
| [setPhoneticsAlias(String value)](#setPhoneticsAlias-java.lang.String-) | Définit la prononciation phonétique de l'alias d'un champ personnalisé. |
| [setRestrictValues(boolean value)](#setRestrictValues-boolean-) | Définit une valeur indiquant si les valeurs du champ personnalisé sont limitées aux valeurs de la `ValueList`([getValueList()](../../com.aspose.tasks/extendedattributedefinition\#getValueList--)/ [setValueList(List)](../../com.aspose.tasks/extendedattributedefinition\#setValueList-List-Value--)). |
| [setRollupType(int value)](#setRollupType-int-) | Définit la manière dont les rollups sont calculés. |
| [setSecondaryGuid(String value)](#setSecondaryGuid-java.lang.String-) | Définit le GUID secondaire de l'attribut étendu. |
| [setSecondaryPid(String value)](#setSecondaryPid-java.lang.String-) | Définit le PID secondaire d'un champ personnalisé. |
| [setSummaryRowsCalculationType(int value)](#setSummaryRowsCalculationType-int-) | Définit le type de calcul de la valeur de l'attribut personnalisé pour les lignes de synthèse. |
| [setUserDef(boolean value)](#setUserDef-boolean-) | Définit une valeur indiquant si un champ personnalisé est défini par l'utilisateur. |
| [setValuelistSortOrder(int value)](#setValuelistSortOrder-int-) | Définit la façon dont les listes de valeurs sont triées. |
### addLookupValue(Value value) {#addLookupValue-com.aspose.tasks.Value-}
```
public final void addLookupValue(Value value)
```


Ajoute une valeur à la liste de recherche interne. C’est une méthode préférable pour les manipulations avec la `ValueList`([getValueList()](../../com.aspose.tasks/extendedattributedefinition\#getValueList--)/ [setValueList(List)](../../com.aspose.tasks/extendedattributedefinition\#setValueList-List-Value--)).

--------------------

&gt; ```
&gt; Utilisez ce code pour ajouter une nouvelle valeur à la liste de recherche :
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
| Paramètre | Type | Description |
| --- | --- | --- |
|  | lookupValue | [Value](../../com.aspose.tasks/value) | L'élément [Value](../../com.aspose.tasks/value) spécifié. |

--------------------

`lookupValue` doit être préalablement ajouté à la [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) en utilisant la méthode [addLookupValue(Value)](../../com.aspose.tasks/extendedattributedefinition\\#addLookupValue-Value-) . |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class linked with specified [Value](../../com.aspose.tasks/value) item.
### createExtendedAttribute(String textValue) {#createExtendedAttribute-java.lang.String-}
```
public final ExtendedAttribute createExtendedAttribute(String textValue)
```


Crée un nouvel attribut étendu avec l'ID de champ qui est égal à la valeur de l'ID de champ de cet objet et la valeur de texte spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| textValue | java.lang.String | La valeur texte spécifiée. |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class with the fieldID which equals to this object's fieldID value.
### createExtendedAttribute(BigDecimal numericValue) {#createExtendedAttribute-java.math.BigDecimal-}
```
public final ExtendedAttribute createExtendedAttribute(BigDecimal numericValue)
```


Crée un nouvel attribut étendu avec l'ID de champ qui est égal à la valeur de l'ID de champ de cet objet et la valeur numérique spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| numericValue | java.math.BigDecimal | La valeur numérique spécifiée. |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class with the fieldID which equals to this object's fieldID value.
### createExtendedAttribute(Date dateTimeValue) {#createExtendedAttribute-java.util.Date-}
```
public final ExtendedAttribute createExtendedAttribute(Date dateTimeValue)
```


Crée un nouvel attribut étendu avec l'ID de champ qui est égal à la valeur de l'ID de champ de cet objet et la valeur de date spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| dateTimeValue | java.util.Date | La valeur datetime spécifiée. |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class with the fieldID which equals to this object's fieldID value.
### createLookupResourceDefinition(int customFieldType, int fieldId, String alias) {#createLookupResourceDefinition-int-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createLookupResourceDefinition(int customFieldType, int fieldId, String alias)
```


Méthode d'usine qui crée une définition d'attribut étendu avec recherche. Elle possède `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\\#setCalculationType-int-)) égal à [CalculationType.Lookup](../../com.aspose.tasks/calculationtype\\#Lookup) et ne peut être utilisée que dans les Ressources. Vous devez spécifier `customFieldType`, `fieldId` et `alias` lors de l'appel de cette méthode.

--------------------

&gt; ```
&gt; Utilisez cet exemple pour créer une définition de champ personnalisé pour une ressource avec recherche, puis remplissez‑la avec des valeurs texte :
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
| Paramètre | Type | Description |
| --- | --- | --- |
| fieldId | int | L'ID de champ spécifié [ExtendedAttributeResource](../../com.aspose.tasks/extendedattributeresource). |
| alias | java.lang.String | L'alias String spécifié. |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `fieldId` and `alias`.
### createLookupTaskDefinition(int customFieldType, int fieldId, String alias) {#createLookupTaskDefinition-int-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createLookupTaskDefinition(int customFieldType, int fieldId, String alias)
```


Méthode d'usine qui crée une définition d'attribut étendu avec recherche. Elle possède `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) égale à [CalculationType.Lookup](../../com.aspose.tasks/calculationtype\#Lookup) et ne peut être utilisée que dans les Tasks. Vous devez spécifier `customFieldType`, `fieldId` et `alias` lors de l'appel de cette méthode.

--------------------

&gt; ```
&gt; Utilisez cet exemple pour créer une définition de champ personnalisé pour une tâche avec recherche, puis remplissez‑la avec des valeurs texte :
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
| Paramètre | Type | Description |
| --- | --- | --- |
| fieldId | int | L'ID de champ spécifié [ExtendedAttributeTask](../../com.aspose.tasks/extendedattributetask). |
| alias | java.lang.String | L'alias String spécifié. |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `fieldId` and `alias`.
### createResourceDefinition(int customFieldType, int fieldId, String alias) {#createResourceDefinition-int-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createResourceDefinition(int customFieldType, int fieldId, String alias)
```


Méthode d'usine qui crée une définition d'attribut étendu simple, que Microsoft Project affiche comme "None". Elle possède `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) égale à [CalculationType.None](../../com.aspose.tasks/calculationtype\#None) et ne peut être utilisée que dans les Resource. Vous devez spécifier `customFieldType`, `fieldId` et `alias` lors de l'appel de cette méthode.

--------------------

&gt; ```
&gt; Utilisez cet exemple pour créer une définition de champ texte personnalisé :
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
| Paramètre | Type | Description |
| --- | --- | --- |
| fieldId | int | L'ID de champ spécifié [ExtendedAttributeResource](../../com.aspose.tasks/extendedattributeresource). |
| alias | java.lang.String | L'alias String spécifié. |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `fieldId` and `alias`.
### createTaskDefinition(int customFieldType, int fieldId, String alias) {#createTaskDefinition-int-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createTaskDefinition(int customFieldType, int fieldId, String alias)
```


Méthode d'usine qui crée une définition d'attribut étendu simple, que Microsoft Project affiche comme "None". Elle possède `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) égale à [CalculationType.None](../../com.aspose.tasks/calculationtype\#None) et ne peut être utilisée que dans les Tasks. Vous devez spécifier `customFieldType`, `fieldId` et `alias` lors de l'appel de cette méthode.

--------------------

&gt; ```
&gt; Utilisez cet exemple pour créer une définition de champ texte personnalisé :
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
| Paramètre | Type | Description |
| --- | --- | --- |
| fieldId | int | L'ID de champ spécifié [ExtendedAttributeTask](../../com.aspose.tasks/extendedattributetask). |
| alias | java.lang.String | L'alias String spécifié. |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `fieldId` and `alias`.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Renvoie un indicateur indiquant si cette instance est égale à l'objet spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| obj | java.lang.Object | l'objet spécifié à comparer à cette instance. |

**Returns:**
boolean - un indicateur indiquant si cette instance est égale à l'objet spécifié.
### getAlias() {#getAlias--}
```
public final String getAlias()
```


Obtient l'alias d'un champ personnalisé.

**Returns:**
java.lang.String - l'alias d'un champ personnalisé.
### getAppendNewValues() {#getAppendNewValues--}
```
public final boolean getAppendNewValues()
```


Obtient une valeur indiquant si les nouvelles valeurs ajoutées à un projet sont automatiquement ajoutées à la liste.

--------------------

Actuellement pris en charge pour les formats MSP 2003/2007 Xml et MSP 2003 mpp.

**Returns:**
boolean - une valeur indiquant si les nouvelles valeurs ajoutées à un projet sont automatiquement ajoutées à la liste.
### getAutoRollDown() {#getAutoRollDown--}
```
public final boolean getAutoRollDown()
```


Obtient une valeur indiquant si un déploiement automatique vers les affectations est activé.

**Returns:**
boolean - une valeur indiquant si un déploiement automatique vers les affectations est activé.
### getCalculationType() {#getCalculationType--}
```
public final int getCalculationType()
```


Obtient le type de calcul de la valeur de l'attribut personnalisé.

**Returns:**
int - le type de calcul de la valeur de l'attribut personnalisé.
### getCfType() {#getCfType--}
```
public final int getCfType()
```


Obtient le type d'un champ personnalisé.

**Returns:**
int - le type d'un champ personnalisé.
### getDefault() {#getDefault--}
```
public final String getDefault()
```


Obtient la valeur par défaut dans la liste.

--------------------

Actuellement pris en charge pour les formats MSP 2003/2007 Xml et MSP 2003 mpp.

**Returns:**
java.lang.String - la valeur par défaut dans la liste.
### getDefaultGuid() {#getDefaultGuid--}
```
public final String getDefaultGuid()
```


Obtient le GUID de l'entrée de la table de recherche par défaut.

**Returns:**
java.lang.String - le GUID de l'entrée de table de recherche par défaut.
### getElementType() {#getElementType--}
```
public final int getElementType()
```


Obtient l'attribut étendu associé à une tâche, une ressource ou une affectation.

**Returns:**
int - l'attribut étendu est associé à une tâche, une ressource ou une affectation.
### getFieldId() {#getFieldId--}
```
public final String getFieldId()
```


Gets correspond à l'ID du projet d'un champ personnalisé. Utilisez la représentation sous forme de chaîne d'une constante de la classe [ExtendedAttributeTask](../../com.aspose.tasks/extendedattributetask) pour spécifier `FieldId`([getFieldId()](../../com.aspose.tasks/extendedattributedefinition\#getFieldId--)/ [setFieldId(String)](../../com.aspose.tasks/extendedattributedefinition\#setFieldId-String-)) propriété.

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

La façon préférable de définir la propriété `FieldId`([getFieldId()](../../com.aspose/tasks/extendedattributedefinition\#getFieldId--)/ [setFieldId(String)](../../com.aspose/tasks/extendedattributedefinition\#setFieldId-String-)) est de créer [ExtendedAttributeDefinition](../../com.aspose/tasks/extendedattributedefinition) en utilisant l'une des méthodes d'usine dédiées comme [createTaskDefinition(int, String)](../../com.aspose/tasks/extendedattributedefinition\#createTaskDefinition-int--String-) ou [createLookupTaskDefinition(int, int, String)](../../com.aspose/tasks/extendedattributedefinition\#createLookupTaskDefinition-int--int--String-).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | correspond à l'identifiant du projet d'un champ personnalisé. |

### setFormula(String value) {#setFormula-java.lang.String-}
```
public final void setFormula(String value)
```


Définit la formule que Microsoft Project utilise pour remplir un champ de tâche personnalisé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | la formule que Microsoft Project utilise pour remplir un champ de tâche personnalisé. |

### setGraphicalIndicator(GraphicalIndicatorsInfo value) {#setGraphicalIndicator-com.aspose.tasks.GraphicalIndicatorsInfo-}
```
public final void setGraphicalIndicator(GraphicalIndicatorsInfo value)
```


Définit des informations d'indicateurs graphiques associées à l'attribut étendu. Applicable au format MPP.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [GraphicalIndicatorsInfo](../../com.aspose.tasks/graphicalindicatorsinfo) | des informations d'indicateurs graphiques associées à l'attribut étendu. |

### setGuid(String value) {#setGuid-java.lang.String-}
```
public final void setGuid(String value)
```


Définit le GUID d'un champ personnalisé.

--------------------

Actuellement pris en charge uniquement pour le format Xml.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | le GUID d'un champ personnalisé. |

### setMaxMultiValues(int value) {#setMaxMultiValues-int-}
```
public final void setMaxMultiValues(int value)
```


Définit le nombre maximal de valeurs que vous pouvez définir dans une liste déroulante.

--------------------

Actuellement pris en charge uniquement pour le format Xml.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | le nombre maximal de valeurs que vous pouvez définir dans une liste déroulante. |

### setPhoneticsAlias(String value) {#setPhoneticsAlias-java.lang.String-}
```
public final void setPhoneticsAlias(String value)
```


Définit la prononciation phonétique de l'alias d'un champ personnalisé.

--------------------

Actuellement pris en charge uniquement pour le format Xml.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | la prononciation phonétique de l'alias d'un champ personnalisé. |

### setRestrictValues(boolean value) {#setRestrictValues-boolean-}
```
public final void setRestrictValues(boolean value)
```


Définit une valeur indiquant si les valeurs du champ personnalisé sont limitées aux valeurs de la `ValueList`([getValueList()](../../com.aspose.tasks/extendedattributedefinition\#getValueList--)/ [setValueList(List)](../../com.aspose.tasks/extendedattributedefinition\#setValueList-List-Value--)).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant si les valeurs du champ personnalisé sont limitées aux valeurs dans le |

### setRollupType(int value) {#setRollupType-int-}
```
public final void setRollupType(int value)
```


Définit la manière dont les rollups sont calculés.

--------------------

L'écriture est actuellement prise en charge uniquement pour le format Xml.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | la façon dont les rollups sont calculés. |

### setSecondaryGuid(String value) {#setSecondaryGuid-java.lang.String-}
```
public final void setSecondaryGuid(String value)
```


Définit le GUID secondaire de l'attribut étendu.

--------------------

Ceci est une nouvelle propriété pour MS Project 2010.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | le GUID secondaire de l'attribut étendu. |

### setSecondaryPid(String value) {#setSecondaryPid-java.lang.String-}
```
public final void setSecondaryPid(String value)
```


Définit le PID secondaire d'un champ personnalisé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | le PID secondaire d'un champ personnalisé. |

### setSummaryRowsCalculationType(int value) {#setSummaryRowsCalculationType-int-}
```
public final void setSummaryRowsCalculationType(int value)
```


Définit le type de calcul de la valeur de l'attribut personnalisé pour les lignes de synthèse.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | le type de calcul de la valeur de l'attribut personnalisé pour les lignes de synthèse. |

### setUserDef(boolean value) {#setUserDef-boolean-}
```
public final void setUserDef(boolean value)
```


Définit une valeur indiquant si un champ personnalisé est défini par l'utilisateur.

--------------------

Actuellement pris en charge uniquement pour le format Xml.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant si un champ personnalisé est défini par l'utilisateur. |

### setValuelistSortOrder(int value) {#setValuelistSortOrder-int-}
```
public final void setValuelistSortOrder(int value)
```


Définit la façon dont les listes de valeurs sont triées. Les valeurs sont : 0=Descendant, 1=Ascendant.

--------------------

Actuellement pris en charge pour les formats MSP 2003/2007 Xml et MSP 2003 mpp.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | la façon dont les listes de valeurs sont triées. |

