---
title: "ExtendedAttributeDefinition"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa una definición de atributo extendido asociada a un proyecto."
type: docs
weight: 83
url: /es/java/com.aspose.tasks/extendedattributedefinition/
---

**Inheritance:**
java.lang.Object
```
public class ExtendedAttributeDefinition
```

Representa una definición de atributo extendido asociada a un proyecto.
## Métodos

| Método | Descripción |
| --- | --- |
| [addLookupValue(Value value)](#addLookupValue-com.aspose.tasks.Value-) | Agrega un valor a la lista de búsqueda interna. |
| [compareTo(ExtendedAttributeDefinition o)](#compareTo-com.aspose.tasks.ExtendedAttributeDefinition-) | Compara este objeto con otra instancia de la clase @\{code ExtendedAttributeDefinition\}. |
| [createExtendedAttribute()](#createExtendedAttribute--) | Crea un nuevo atributo extendido con el ID de campo que es igual al valor del ID de campo de este objeto. |
| [createExtendedAttribute(boolean flagValue)](#createExtendedAttribute-boolean-) | Crea un nuevo atributo extendido con el ID de campo que es igual al valor del ID de campo de este objeto y al valor de bandera especificado. |
| [createExtendedAttribute(Duration durationValue)](#createExtendedAttribute-com.aspose.tasks.Duration-) | Crea un nuevo atributo extendido con el ID de campo que es igual al valor del ID de campo de este objeto y al valor de duración especificado. |
| [createExtendedAttribute(Value lookupValue)](#createExtendedAttribute-com.aspose.tasks.Value-) | Crea un nuevo atributo extendido vinculado con el elemento [Value](../../com.aspose.tasks/value) especificado. |
| [createExtendedAttribute(String textValue)](#createExtendedAttribute-java.lang.String-) | Crea un nuevo atributo extendido con el ID de campo que es igual al valor del ID de campo de este objeto y al valor de texto especificado. |
| [createExtendedAttribute(BigDecimal numericValue)](#createExtendedAttribute-java.math.BigDecimal-) | Crea un nuevo atributo extendido con el ID de campo que es igual al valor del ID de campo de este objeto y al valor numérico especificado. |
| [createExtendedAttribute(Date dateTimeValue)](#createExtendedAttribute-java.util.Date-) | Crea un nuevo atributo extendido con el ID de campo que es igual al valor del ID de campo de este objeto y al valor de fecha especificado. |
| [createLookupResourceDefinition(int customFieldType, int fieldId, String alias)](#createLookupResourceDefinition-int-int-java.lang.String-) | Método de fábrica que crea una definición de atributo extendido con búsqueda. |
| [createLookupResourceDefinition(int fieldId, String alias)](#createLookupResourceDefinition-int-java.lang.String-) | Método de fábrica que crea una definición de atributo extendido con búsqueda. |
| [createLookupTaskDefinition(int customFieldType, int fieldId, String alias)](#createLookupTaskDefinition-int-int-java.lang.String-) | Método de fábrica que crea una definición de atributo extendido con búsqueda. |
| [createLookupTaskDefinition(int fieldId, String alias)](#createLookupTaskDefinition-int-java.lang.String-) | Método de fábrica que crea una definición de atributo extendido con búsqueda. |
| [createResourceDefinition(int customFieldType, int fieldId, String alias)](#createResourceDefinition-int-int-java.lang.String-) | Método de fábrica que crea una definición de atributo extendido simple, que Microsoft Project muestra como "None". |
| [createResourceDefinition(int fieldId, String alias)](#createResourceDefinition-int-java.lang.String-) | Método de fábrica que crea una definición de atributo extendido simple, que Microsoft Project muestra como "None". |
| [createTaskDefinition(int customFieldType, int fieldId, String alias)](#createTaskDefinition-int-int-java.lang.String-) | Método de fábrica que crea una definición de atributo extendido simple, que Microsoft Project muestra como "None". |
| [createTaskDefinition(int fieldId, String alias)](#createTaskDefinition-int-java.lang.String-) | Método de fábrica que crea una definición de atributo extendido simple, que Microsoft Project muestra como "None". |
| [equals(Object obj)](#equals-java.lang.Object-) | Devuelve una bandera que indica si esta instancia es igual al objeto especificado. |
| [getAlias()](#getAlias--) | Obtiene el alias de un campo personalizado. |
| [getAppendNewValues()](#getAppendNewValues--) | Obtiene un valor que indica si los nuevos valores añadidos a un proyecto se añaden automáticamente a la lista. |
| [getAutoRollDown()](#getAutoRollDown--) | Obtiene un valor que indica si se habilita una reducción automática a asignaciones. |
| [getCalculationType()](#getCalculationType--) | Obtiene el tipo de cálculo del valor del atributo personalizado. |
| [getCfType()](#getCfType--) | Obtiene el tipo de un campo personalizado. |
| [getDefault()](#getDefault--) | Obtiene el valor predeterminado en la lista. |
| [getDefaultGuid()](#getDefaultGuid--) | Obtiene el Guid de la entrada predeterminada de la tabla de búsqueda. |
| [getElementType()](#getElementType--) | Obtiene si el atributo extendido está asociado a una tarea, un recurso o una asignación. |
| [getFieldId()](#getFieldId--) | Obtiene lo que corresponde al id del proyecto de un campo personalizado. |
| [getFieldName()](#getFieldName--) | Obtiene el nombre de un campo personalizado. |
| [getFormula()](#getFormula--) | Obtiene la fórmula que Microsoft Project usa para rellenar un campo de tarea personalizado. |
| [getGraphicalIndicator()](#getGraphicalIndicator--) | Obtiene la información de indicadores gráficos asociada al atributo extendido. |
| [getGuid()](#getGuid--) | Obtiene el Guid de un campo personalizado. |
| [getLookupUid()](#getLookupUid--) | Obtiene un Guid de la tabla de búsqueda asociada a un campo personalizado. |
| [getMaxMultiValues()](#getMaxMultiValues--) | Obtiene el número máximo de valores que puede establecer en una lista de selección. |
| [getParentProject()](#getParentProject--) | Obtiene el proyecto principal para la instancia de [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition). |
| [getPhoneticsAlias()](#getPhoneticsAlias--) | Obtiene la pronunciación fonética del alias de un campo personalizado. |
| [getRestrictValues()](#getRestrictValues--) | Obtiene un valor que indica si los valores del campo personalizado están restringidos a los valores en la `ValueList`([getValueList()](../../com.aspose.tasks/extendedattributedefinition\#getValueList--)/ [setValueList(List)](../../com.aspose.tasks/extendedattributedefinition\#setValueList-List-Value--)). |
| [getRollupType()](#getRollupType--) | Obtiene la forma en que se calculan los acumulados. |
| [getSecondaryGuid()](#getSecondaryGuid--) | Obtiene el guid secundario del atributo extendido. |
| [getSecondaryPid()](#getSecondaryPid--) | Obtiene el PID secundario de un campo personalizado. |
| [getSummaryRowsCalculationType()](#getSummaryRowsCalculationType--) | Obtiene el tipo de cálculo del valor del atributo personalizado para filas de resumen. |
| [getUserDef()](#getUserDef--) | Obtiene un valor que indica si un campo personalizado es definido por el usuario. |
| [getValueList()](#getValueList--) | Obtiene la List&lt;Value&gt; ValueList. |
| [getValuelistSortOrder()](#getValuelistSortOrder--) | Obtiene la forma en que se ordenan las listas de valores. |
| [hashCode()](#hashCode--) | Devuelve un código hash para la instancia de la clase [ExtendedAttributeDefinition](../../com.aspose/tasks/extendedattributedefinition). |
| [removeLookupValue(Value value)](#removeLookupValue-com.aspose.tasks.Value-) | Elimina un valor de la lista de búsqueda interna. |
| [setAlias(String value)](#setAlias-java.lang.String-) | Establece el alias de un campo personalizado. |
| [setAppendNewValues(boolean value)](#setAppendNewValues-boolean-) | Establece un valor que indica si los nuevos valores añadidos a un proyecto se añaden automáticamente a la lista. |
| [setAutoRollDown(boolean value)](#setAutoRollDown-boolean-) | Establece un valor que indica si se habilita una propagación automática a las asignaciones. |
| [setCalculationType(int value)](#setCalculationType-int-) | Establece el tipo de cálculo del valor del atributo personalizado. |
| [setDefault(String value)](#setDefault-java.lang.String-) | Establece el valor predeterminado en la lista. |
| [setDefaultGuid(String value)](#setDefaultGuid-java.lang.String-) | Establece el Guid de la entrada de tabla de búsqueda predeterminada. |
| [setElementType(int value)](#setElementType-int-) | Establece que el atributo extendido está asociado a una tarea, un recurso o una asignación. |
| [setFieldId(String value)](#setFieldId-java.lang.String-) | Establece que corresponde al id del proyecto de un campo personalizado. |
| [setFormula(String value)](#setFormula-java.lang.String-) | Establece la fórmula que Microsoft Project usa para rellenar un campo de tarea personalizado. |
| [setGraphicalIndicator(GraphicalIndicatorsInfo value)](#setGraphicalIndicator-com.aspose.tasks.GraphicalIndicatorsInfo-) | Establece la información de indicadores gráficos asociada al atributo extendido. |
| [setGuid(String value)](#setGuid-java.lang.String-) | Establece el Guid de un campo personalizado. |
| [setMaxMultiValues(int value)](#setMaxMultiValues-int-) | Establece el número máximo de valores que puede establecer en una lista de selección. |
| [setPhoneticsAlias(String value)](#setPhoneticsAlias-java.lang.String-) | Establece la pronunciación fonética del alias de un campo personalizado. |
| [setRestrictValues(boolean value)](#setRestrictValues-boolean-) | Establece un valor que indica si los valores del campo personalizado están restringidos a los valores en la `ValueList`([getValueList()](../../com.aspose.tasks/extendedattributedefinition\#getValueList--)/ [setValueList(List)](../../com.aspose.tasks/extendedattributedefinition\#setValueList-List-Value--)). |
| [setRollupType(int value)](#setRollupType-int-) | Establece la forma en que se calculan los acumulados. |
| [setSecondaryGuid(String value)](#setSecondaryGuid-java.lang.String-) | Establece el guid secundario del atributo extendido. |
| [setSecondaryPid(String value)](#setSecondaryPid-java.lang.String-) | Establece el PID secundario de un campo personalizado. |
| [setSummaryRowsCalculationType(int value)](#setSummaryRowsCalculationType-int-) | Establece el tipo de cálculo del valor del atributo personalizado para filas de resumen. |
| [setUserDef(boolean value)](#setUserDef-boolean-) | Establece un valor que indica si un campo personalizado es definido por el usuario. |
| [setValuelistSortOrder(int value)](#setValuelistSortOrder-int-) | Establece la forma en que se ordenan las listas de valores. |
### addLookupValue(Value value) {#addLookupValue-com.aspose.tasks.Value-}
```
public final void addLookupValue(Value value)
```


Añade un valor a la lista de búsqueda interna. Esta es una forma preferible para manipulaciones con la `ValueList`([getValueList()](../../com.aspose.tasks/extendedattributedefinition\#getValueList--)/ [setValueList(List)](../../com.aspose.tasks/extendedattributedefinition\#setValueList-List-Value--)).

--------------------

&gt; ```
&gt; Use este código para agregar un nuevo Valor a la lista de búsqueda:
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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | lookupValue | [Value](../../com.aspose.tasks/value) | El elemento [Value](../../com.aspose.tasks/value) especificado. |

--------------------

`lookupValue` debe haberse añadido previamente a la [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) usando el método [addLookupValue(Value)](../../com.aspose.tasks/extendedattributedefinition\#addLookupValue-Value-) . |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class linked with specified [Value](../../com.aspose.tasks/value) item.
### createExtendedAttribute(String textValue) {#createExtendedAttribute-java.lang.String-}
```
public final ExtendedAttribute createExtendedAttribute(String textValue)
```


Crea un nuevo atributo extendido con el ID de campo que es igual al valor del ID de campo de este objeto y al valor de texto especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| textValue | java.lang.String | El valor de texto especificado. |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class with the fieldID which equals to this object's fieldID value.
### createExtendedAttribute(BigDecimal numericValue) {#createExtendedAttribute-java.math.BigDecimal-}
```
public final ExtendedAttribute createExtendedAttribute(BigDecimal numericValue)
```


Crea un nuevo atributo extendido con el ID de campo que es igual al valor del ID de campo de este objeto y al valor numérico especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| numericValue | java.math.BigDecimal | El valor numérico especificado. |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class with the fieldID which equals to this object's fieldID value.
### createExtendedAttribute(Date dateTimeValue) {#createExtendedAttribute-java.util.Date-}
```
public final ExtendedAttribute createExtendedAttribute(Date dateTimeValue)
```


Crea un nuevo atributo extendido con el ID de campo que es igual al valor del ID de campo de este objeto y al valor de fecha especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| dateTimeValue | java.util.Date | El valor de fecha y hora especificado. |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class with the fieldID which equals to this object's fieldID value.
### createLookupResourceDefinition(int customFieldType, int fieldId, String alias) {#createLookupResourceDefinition-int-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createLookupResourceDefinition(int customFieldType, int fieldId, String alias)
```


Método de fábrica que crea una definición de atributo extendido con búsqueda. Tiene `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) igual a [CalculationType.Lookup](../../com.aspose.tasks/calculationtype\#Lookup) y solo puede usarse en Recursos. Se requiere especificar `customFieldType`, `fieldId` y `alias` al llamar a este método.

--------------------

&gt; ```
&gt; Use este ejemplo para crear una definición de campo personalizado para un recurso con búsqueda y luego completarlo con valores de texto:
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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fieldId | int | El ID de campo especificado [ExtendedAttributeResource](../../com.aspose.tasks/extendedattributeresource). |
| alias | java.lang.String | El alias de String especificado. |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `fieldId` and `alias`.
### createLookupTaskDefinition(int customFieldType, int fieldId, String alias) {#createLookupTaskDefinition-int-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createLookupTaskDefinition(int customFieldType, int fieldId, String alias)
```


Método de fábrica que crea una definición de atributo extendido con búsqueda. Tiene `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) igual a [CalculationType.Lookup](../../com.aspose.tasks/calculationtype\#Lookup) y solo puede usarse en Tasks. Se requiere especificar `customFieldType`, `fieldId` y `alias` al llamar a este método.

--------------------

&gt; ```
&gt; Use este ejemplo para crear una definición de campo personalizado para una tarea con búsqueda y luego completarla con valores de texto:
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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fieldId | int | El ID de campo especificado [ExtendedAttributeTask](../../com.aspose.tasks/extendedattributetask). |
| alias | java.lang.String | El alias de String especificado. |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `fieldId` and `alias`.
### createResourceDefinition(int customFieldType, int fieldId, String alias) {#createResourceDefinition-int-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createResourceDefinition(int customFieldType, int fieldId, String alias)
```


Método de fábrica que crea una definición simple de atributo extendido, que Microsoft Project muestra como "None". Tiene `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) igual a [CalculationType.None](../../com.aspose.tasks/calculationtype\#None) y solo puede usarse en Resource. Se requiere especificar `customFieldType`, `fieldId` y `alias` al llamar a este método.

--------------------

&gt; ```
&gt; Use este ejemplo para crear una definición de campo de texto personalizado:
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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fieldId | int | El ID de campo especificado [ExtendedAttributeResource](../../com.aspose.tasks/extendedattributeresource). |
| alias | java.lang.String | El alias de String especificado. |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `fieldId` and `alias`.
### createTaskDefinition(int customFieldType, int fieldId, String alias) {#createTaskDefinition-int-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createTaskDefinition(int customFieldType, int fieldId, String alias)
```


Método de fábrica que crea una definición simple de atributo extendido, que Microsoft Project muestra como "None". Tiene `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) igual a [CalculationType.None](../../com.aspose.tasks/calculationtype\#None) y solo puede usarse en Tasks. Se requiere especificar `customFieldType`, `fieldId` y `alias` al llamar a este método.

--------------------

&gt; ```
&gt; Use este ejemplo para crear una definición de campo de texto personalizado:
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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fieldId | int | El ID de campo especificado [ExtendedAttributeTask](../../com.aspose.tasks/extendedattributetask). |
| alias | java.lang.String | El alias de String especificado. |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `fieldId` and `alias`.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Devuelve una bandera que indica si esta instancia es igual al objeto especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| obj | java.lang.Object | el objeto especificado para comparar con esta instancia. |

**Returns:**
boolean - una bandera que indica si esta instancia es igual al objeto especificado.
### getAlias() {#getAlias--}
```
public final String getAlias()
```


Obtiene el alias de un campo personalizado.

**Returns:**
java.lang.String - el alias de un campo personalizado.
### getAppendNewValues() {#getAppendNewValues--}
```
public final boolean getAppendNewValues()
```


Obtiene un valor que indica si los nuevos valores añadidos a un proyecto se añaden automáticamente a la lista.

--------------------

Actualmente compatible con los formatos Xml de MSP 2003/2007 y mpp de MSP 2003.

**Returns:**
boolean - un valor que indica si los nuevos valores añadidos a un proyecto se añaden automáticamente a la lista.
### getAutoRollDown() {#getAutoRollDown--}
```
public final boolean getAutoRollDown()
```


Obtiene un valor que indica si se habilita una reducción automática a asignaciones.

**Returns:**
boolean - un valor que indica si está habilitado un descenso automático a las asignaciones.
### getCalculationType() {#getCalculationType--}
```
public final int getCalculationType()
```


Obtiene el tipo de cálculo del valor del atributo personalizado.

**Returns:**
int - el tipo de cálculo del valor del atributo personalizado.
### getCfType() {#getCfType--}
```
public final int getCfType()
```


Obtiene el tipo de un campo personalizado.

**Returns:**
int - el tipo de un campo personalizado.
### getDefault() {#getDefault--}
```
public final String getDefault()
```


Obtiene el valor predeterminado en la lista.

--------------------

Actualmente compatible con los formatos Xml de MSP 2003/2007 y mpp de MSP 2003.

**Returns:**
java.lang.String - el valor predeterminado en la lista.
### getDefaultGuid() {#getDefaultGuid--}
```
public final String getDefaultGuid()
```


Obtiene el Guid de la entrada predeterminada de la tabla de búsqueda.

**Returns:**
java.lang.String - el Guid de la entrada predeterminada de la tabla de búsqueda.
### getElementType() {#getElementType--}
```
public final int getElementType()
```


Obtiene si el atributo extendido está asociado a una tarea, un recurso o una asignación.

**Returns:**
int - el atributo extendido está asociado a una tarea, un recurso o una asignación.
### getFieldId() {#getFieldId--}
```
public final String getFieldId()
```


Gets corresponde al id del proyecto de un campo personalizado. Utilice la representación en cadena de una constante de la clase [ExtendedAttributeTask](../../com.aspose.tasks/extendedattributetask) para especificar `FieldId`([getFieldId()](../../com.aspose.tasks/extendedattributedefinition\#getFieldId--)/ [setFieldId(String)](../../com.aspose.tasks/extendedattributedefinition\#setFieldId-String-)) propiedad.

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

La forma preferible de establecer la propiedad `FieldId`([getFieldId()](../../com.aspose/tasks/extendedattributedefinition\#getFieldId--)/ [setFieldId(String)](../../com.aspose/tasks/extendedattributedefinition\#setFieldId-String-)) es crear [ExtendedAttributeDefinition](../../com.aspose/tasks/extendedattributedefinition) utilizando uno de los métodos de fábrica dedicados como [createTaskDefinition(int, String)](../../com.aspose/tasks/extendedattributedefinition\#createTaskDefinition-int--String-) o [createLookupTaskDefinition(int, int, String)](../../com.aspose/tasks/extendedattributedefinition\#createLookupTaskDefinition-int--int--String-).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | corresponde al id del proyecto de un campo personalizado. |

### setFormula(String value) {#setFormula-java.lang.String-}
```
public final void setFormula(String value)
```


Establece la fórmula que Microsoft Project usa para rellenar un campo de tarea personalizado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | la fórmula que Microsoft Project utiliza para rellenar un campo de tarea personalizado. |

### setGraphicalIndicator(GraphicalIndicatorsInfo value) {#setGraphicalIndicator-com.aspose.tasks.GraphicalIndicatorsInfo-}
```
public final void setGraphicalIndicator(GraphicalIndicatorsInfo value)
```


Establece información de indicadores gráficos asociada al atributo extendido. Aplicable al formato MPP.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [GraphicalIndicatorsInfo](../../com.aspose.tasks/graphicalindicatorsinfo) | una información de indicadores gráficos asociada al atributo extendido. |

### setGuid(String value) {#setGuid-java.lang.String-}
```
public final void setGuid(String value)
```


Establece el Guid de un campo personalizado.

--------------------

Actualmente soportado solo para el formato Xml.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | el Guid de un campo personalizado. |

### setMaxMultiValues(int value) {#setMaxMultiValues-int-}
```
public final void setMaxMultiValues(int value)
```


Establece el número máximo de valores que puede establecer en una lista de selección.

--------------------

Actualmente soportado solo para el formato Xml.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | el número máximo de valores que puede establecer en una lista de selección. |

### setPhoneticsAlias(String value) {#setPhoneticsAlias-java.lang.String-}
```
public final void setPhoneticsAlias(String value)
```


Establece la pronunciación fonética del alias de un campo personalizado.

--------------------

Actualmente soportado solo para el formato Xml.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | la pronunciación fonética del alias de un campo personalizado. |

### setRestrictValues(boolean value) {#setRestrictValues-boolean-}
```
public final void setRestrictValues(boolean value)
```


Establece un valor que indica si los valores del campo personalizado están restringidos a los valores en la `ValueList`([getValueList()](../../com.aspose.tasks/extendedattributedefinition\#getValueList--)/ [setValueList(List)](../../com.aspose.tasks/extendedattributedefinition\#setValueList-List-Value--)).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si los valores del campo personalizado están restringidos a los valores en el |

### setRollupType(int value) {#setRollupType-int-}
```
public final void setRollupType(int value)
```


Establece la forma en que se calculan los acumulados.

--------------------

La escritura actualmente soportada solo para el formato Xml.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | la forma en que se calculan los rollups. |

### setSecondaryGuid(String value) {#setSecondaryGuid-java.lang.String-}
```
public final void setSecondaryGuid(String value)
```


Establece el guid secundario del atributo extendido.

--------------------

Esta es una nueva propiedad para MS Project 2010.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | el guid secundario del atributo extendido. |

### setSecondaryPid(String value) {#setSecondaryPid-java.lang.String-}
```
public final void setSecondaryPid(String value)
```


Establece el PID secundario de un campo personalizado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | el PID secundario de un campo personalizado. |

### setSummaryRowsCalculationType(int value) {#setSummaryRowsCalculationType-int-}
```
public final void setSummaryRowsCalculationType(int value)
```


Establece el tipo de cálculo del valor del atributo personalizado para filas de resumen.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | el tipo de cálculo del valor del atributo personalizado para filas de resumen. |

### setUserDef(boolean value) {#setUserDef-boolean-}
```
public final void setUserDef(boolean value)
```


Establece un valor que indica si un campo personalizado es definido por el usuario.

--------------------

Actualmente soportado solo para el formato Xml.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si un campo personalizado es definido por el usuario. |

### setValuelistSortOrder(int value) {#setValuelistSortOrder-int-}
```
public final void setValuelistSortOrder(int value)
```


Establece la forma en que se ordenan las listas de valores. Los valores son: 0=Descendente, 1=Ascendente.

--------------------

Actualmente compatible con los formatos Xml de MSP 2003/2007 y mpp de MSP 2003.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | la forma en que se ordenan las listas de valores. |

