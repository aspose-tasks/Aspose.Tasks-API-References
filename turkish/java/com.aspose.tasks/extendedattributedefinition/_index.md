---
title: "ExtendedAttributeDefinition"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Bir projeye bağlı genişletilmiş öznitelik tanımını temsil eder."
type: docs
weight: 83
url: /tr/java/com.aspose.tasks/extendedattributedefinition/
---

**Inheritance:**
java.lang.Object
```
public class ExtendedAttributeDefinition
```

Bir projeye bağlı genişletilmiş öznitelik tanımını temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [addLookupValue(Value value)](#addLookupValue-com.aspose.tasks.Value-) | İç arama listesine bir değer ekler. |
| [compareTo(ExtendedAttributeDefinition o)](#compareTo-com.aspose.tasks.ExtendedAttributeDefinition-) | Bu nesneyi, @{code ExtendedAttributeDefinition} sınıfının başka bir örneğiyle karşılaştırır. |
| [createExtendedAttribute()](#createExtendedAttribute--) | Bu nesnenin alan kimliği değerine eşit alan kimliğiyle yeni bir genişletilmiş öznitelik oluşturur. |
| [createExtendedAttribute(boolean flagValue)](#createExtendedAttribute-boolean-) | Bu nesnenin alan kimliği değerine ve belirtilen bayrak değerine eşit alan kimliğiyle yeni bir genişletilmiş öznitelik oluşturur. |
| [createExtendedAttribute(Duration durationValue)](#createExtendedAttribute-com.aspose.tasks.Duration-) | Bu nesnenin alan kimliği değerine ve belirtilen süre değerine eşit alan kimliğiyle yeni bir genişletilmiş öznitelik oluşturur. |
| [createExtendedAttribute(Value lookupValue)](#createExtendedAttribute-com.aspose.tasks.Value-) | Belirtilen [Value](../../com.aspose.tasks/value) öğesiyle bağlantılı yeni bir genişletilmiş öznitelik oluşturur. |
| [createExtendedAttribute(String textValue)](#createExtendedAttribute-java.lang.String-) | Bu nesnenin alan kimliği değerine ve belirtilen metin değerine eşit alan kimliğiyle yeni bir genişletilmiş öznitelik oluşturur. |
| [createExtendedAttribute(BigDecimal numericValue)](#createExtendedAttribute-java.math.BigDecimal-) | Bu nesnenin alan kimliği değerine ve belirtilen sayısal değere eşit alan kimliğiyle yeni bir genişletilmiş öznitelik oluşturur. |
| [createExtendedAttribute(Date dateTimeValue)](#createExtendedAttribute-java.util.Date-) | Bu nesnenin alan kimliği değerine ve belirtilen tarih değerine eşit alan kimliğiyle yeni bir genişletilmiş öznitelik oluşturur. |
| [createLookupResourceDefinition(int customFieldType, int fieldId, String alias)](#createLookupResourceDefinition-int-int-java.lang.String-) | Arama içeren bir genişletilmiş öznitelik tanımı oluşturan fabrika yöntemi. |
| [createLookupResourceDefinition(int fieldId, String alias)](#createLookupResourceDefinition-int-java.lang.String-) | Arama içeren bir genişletilmiş öznitelik tanımı oluşturan fabrika yöntemi. |
| [createLookupTaskDefinition(int customFieldType, int fieldId, String alias)](#createLookupTaskDefinition-int-int-java.lang.String-) | Arama içeren bir genişletilmiş öznitelik tanımı oluşturan fabrika yöntemi. |
| [createLookupTaskDefinition(int fieldId, String alias)](#createLookupTaskDefinition-int-java.lang.String-) | Arama içeren bir genişletilmiş öznitelik tanımı oluşturan fabrika yöntemi. |
| [createResourceDefinition(int customFieldType, int fieldId, String alias)](#createResourceDefinition-int-int-java.lang.String-) | Microsoft Project'in "None" olarak gösterdiği basit bir genişletilmiş öznitelik tanımı oluşturan fabrika yöntemi. |
| [createResourceDefinition(int fieldId, String alias)](#createResourceDefinition-int-java.lang.String-) | Microsoft Project'in "None" olarak gösterdiği basit bir genişletilmiş öznitelik tanımı oluşturan fabrika yöntemi. |
| [createTaskDefinition(int customFieldType, int fieldId, String alias)](#createTaskDefinition-int-int-java.lang.String-) | Microsoft Project'in "None" olarak gösterdiği basit bir genişletilmiş öznitelik tanımı oluşturan fabrika yöntemi. |
| [createTaskDefinition(int fieldId, String alias)](#createTaskDefinition-int-java.lang.String-) | Microsoft Project'in "None" olarak gösterdiği basit bir genişletilmiş öznitelik tanımı oluşturan fabrika yöntemi. |
| [equals(Object obj)](#equals-java.lang.Object-) | Bu örneğin belirtilen nesneye eşit olup olmadığını gösteren bir bayrak döndürür. |
| [getAlias()](#getAlias--) | Özel bir alanın takma adını alır. |
| [getAppendNewValues()](#getAppendNewValues--) | Projeye eklenen yeni değerlerin otomatik olarak listeye eklenip eklenmediğini gösteren bir değeri alır. |
| [getAutoRollDown()](#getAutoRollDown--) | Atamalara otomatik olarak aşağı kaydırmanın etkin olup olmadığını gösteren bir değeri alır. |
| [getCalculationType()](#getCalculationType--) | Özel özniteliğin değerinin hesaplama türünü alır. |
| [getCfType()](#getCfType--) | Özel bir alanın türünü alır. |
| [getDefault()](#getDefault--) | Listedeki varsayılan değeri alır. |
| [getDefaultGuid()](#getDefaultGuid--) | Varsayılan arama tablosu girişinin GUID'sini alır. |
| [getElementType()](#getElementType--) | Genişletilmiş özniteliğin bir görev, bir kaynak veya bir atama ile ilişkili olup olmadığını alır. |
| [getFieldId()](#getFieldId--) | Özel bir alanın proje kimliğine karşılık gelen değeri alır. |
| [getFieldName()](#getFieldName--) | Özel bir alanın adını alır. |
| [getFormula()](#getFormula--) | Microsoft Project'in özel bir görev alanını doldurmak için kullandığı formülü alır. |
| [getGraphicalIndicator()](#getGraphicalIndicator--) | Genişletilmiş öznitelikle ilişkili grafik gösterge bilgilerini alır. |
| [getGuid()](#getGuid--) | Özel bir alanın GUID'sini alır. |
| [getLookupUid()](#getLookupUid--) | Özel bir alanla ilişkili arama tablosunun GUID'sini alır. |
| [getMaxMultiValues()](#getMaxMultiValues--) | Seçim listesine ayarlayabileceğiniz maksimum değer sayısını alır. |
| [getParentProject()](#getParentProject--) | [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) örneği için üst projeyi alır. |
| [getPhoneticsAlias()](#getPhoneticsAlias--) | Özel bir alanın takma adının fonetik telaffuzunu alır. |
| [getRestrictValues()](#getRestrictValues--) | Özel alan değerlerinin `ValueList`([getValueList()](../../com.aspose.tasks/extendedattributedefinition\#getValueList--)/ [setValueList(List)](../../com.aspose.tasks/extendedattributedefinition\#setValueList-List-Value--)) içindeki değerlerle sınırlı olup olmadığını gösteren bir değeri alır. |
| [getRollupType()](#getRollupType--) | Toplamaların nasıl hesaplandığını alır. |
| [getSecondaryGuid()](#getSecondaryGuid--) | Genişletilmiş özniteliğin ikincil GUID'sini alır. |
| [getSecondaryPid()](#getSecondaryPid--) | Özel bir alanın ikincil PID'sini alır. |
| [getSummaryRowsCalculationType()](#getSummaryRowsCalculationType--) | Özet satırlar için özel özniteliğin değerinin hesaplama türünü alır. |
| [getUserDef()](#getUserDef--) | Özel bir alanın kullanıcı tarafından tanımlanıp tanımlanmadığını gösteren bir değeri alır. |
| [getValueList()](#getValueList--) | List&lt;Value&gt; ValueList'i alır. |
| [getValuelistSortOrder()](#getValuelistSortOrder--) | Değer listelerinin nasıl sıralandığını alır. |
| [hashCode()](#hashCode--) | Bir [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) sınıfının örneği için bir karma kodu döndürür. |
| [removeLookupValue(Value value)](#removeLookupValue-com.aspose.tasks.Value-) | İç arama listesinden bir değeri kaldırır. |
| [setAlias(String value)](#setAlias-java.lang.String-) | Özel bir alanın takma adını ayarlar. |
| [setAppendNewValues(boolean value)](#setAppendNewValues-boolean-) | Projeye eklenen yeni değerlerin otomatik olarak listeye eklenip eklenmeyeceğini gösteren bir değeri ayarlar. |
| [setAutoRollDown(boolean value)](#setAutoRollDown-boolean-) | Atamalara otomatik aşağı kaydırmanın etkin olup olmadığını gösteren bir değeri ayarlar. |
| [setCalculationType(int value)](#setCalculationType-int-) | Özel özniteliğin değerinin hesaplama türünü ayarlar. |
| [setDefault(String value)](#setDefault-java.lang.String-) | Listedeki varsayılan değeri ayarlar. |
| [setDefaultGuid(String value)](#setDefaultGuid-java.lang.String-) | Varsayılan arama tablosu girişinin GUID'sini ayarlar. |
| [setElementType(int value)](#setElementType-int-) | Uzatılmış öznitelik bir görev, bir kaynak veya bir atama ile ilişkilendirildiğini ayarlar. |
| [setFieldId(String value)](#setFieldId-java.lang.String-) | Özel bir alanın proje kimliğine karşılık gelen değeri ayarlar. |
| [setFormula(String value)](#setFormula-java.lang.String-) | Microsoft Project'in özel görev alanını doldurmak için kullandığı formülü ayarlar. |
| [setGraphicalIndicator(GraphicalIndicatorsInfo value)](#setGraphicalIndicator-com.aspose.tasks.GraphicalIndicatorsInfo-) | Uzatılmış öznitelikle ilişkili grafik gösterge bilgilerini ayarlar. |
| [setGuid(String value)](#setGuid-java.lang.String-) | Özel bir alanın GUID'sini ayarlar. |
| [setMaxMultiValues(int value)](#setMaxMultiValues-int-) | Seçim listesindeki ayarlanabilecek maksimum değer sayısını belirler. |
| [setPhoneticsAlias(String value)](#setPhoneticsAlias-java.lang.String-) | Özel bir alanın takma adının fonetik telaffuzunu ayarlar. |
| [setRestrictValues(boolean value)](#setRestrictValues-boolean-) | Özel alan değerlerinin `ValueList`([getValueList()](../../com.aspose.tasks/extendedattributedefinition\\#getValueList--)/ [setValueList(List)](../../com.aspose.tasks/extendedattributedefinition\\#setValueList-List-Value--)) içinde sınırlı olup olmadığını gösteren bir değeri ayarlar. |
| [setRollupType(int value)](#setRollupType-int-) | Toplamların nasıl hesaplandığını ayarlar. |
| [setSecondaryGuid(String value)](#setSecondaryGuid-java.lang.String-) | Uzatılmış özniteliğin ikincil GUID'sini ayarlar. |
| [setSecondaryPid(String value)](#setSecondaryPid-java.lang.String-) | Özel bir alanın ikincil PID'sini ayarlar. |
| [setSummaryRowsCalculationType(int value)](#setSummaryRowsCalculationType-int-) | Özet satırları için özel özniteliğin değerinin hesaplama türünü ayarlar. |
| [setUserDef(boolean value)](#setUserDef-boolean-) | Özel bir alanın kullanıcı tarafından tanımlanıp tanımlanmadığını gösteren bir değeri ayarlar. |
| [setValuelistSortOrder(int value)](#setValuelistSortOrder-int-) | Değer listelerinin nasıl sıralandığını ayarlar. |
### addLookupValue(Value value) {#addLookupValue-com.aspose.tasks.Value-}
```
public final void addLookupValue(Value value)
```


İç arama listesine bir değer ekler. Bu, `ValueList`([getValueList()](../../com.aspose.tasks/extendedattributedefinition\\#getValueList--)/ [setValueList(List)](../../com.aspose.tasks/extendedattributedefinition\\#setValueList-List-Value--)) ile manipülasyonlar için tercih edilen bir yoldur.

--------------------

&gt; ```
&gt; Yeni bir Değeri arama listesine eklemek için bu kodu kullanın:
&gt; ``````

taskTextAttr.addLookupValue(new Value() {{
this.setId(1);
this.setVal("Metin değeri 1");
this.setDescription("Metin değeri açıklaması 1");
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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | lookupValue | [Value](../../com.aspose.tasks/value) | Belirtilen [Value](../../com.aspose.tasks/value) öğesi. |

--------------------

`lookupValue` daha önce [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) kullanılarak [addLookupValue(Value)](../../com.aspose.tasks/extendedattributedefinition\#addLookupValue-Value-) yöntemiyle eklenmiş olmalıdır. |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class linked with specified [Value](../../com.aspose.tasks/value) item.
### createExtendedAttribute(String textValue) {#createExtendedAttribute-java.lang.String-}
```
public final ExtendedAttribute createExtendedAttribute(String textValue)
```


Bu nesnenin alan kimliği değerine ve belirtilen metin değerine eşit alan kimliğiyle yeni bir genişletilmiş öznitelik oluşturur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| textValue | java.lang.String | Belirtilen metin değeri. |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class with the fieldID which equals to this object's fieldID value.
### createExtendedAttribute(BigDecimal numericValue) {#createExtendedAttribute-java.math.BigDecimal-}
```
public final ExtendedAttribute createExtendedAttribute(BigDecimal numericValue)
```


Bu nesnenin alan kimliği değerine ve belirtilen sayısal değere eşit alan kimliğiyle yeni bir genişletilmiş öznitelik oluşturur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| numericValue | java.math.BigDecimal | Belirtilen sayısal değer. |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class with the fieldID which equals to this object's fieldID value.
### createExtendedAttribute(Date dateTimeValue) {#createExtendedAttribute-java.util.Date-}
```
public final ExtendedAttribute createExtendedAttribute(Date dateTimeValue)
```


Bu nesnenin alan kimliği değerine ve belirtilen tarih değerine eşit alan kimliğiyle yeni bir genişletilmiş öznitelik oluşturur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dateTimeValue | java.util.Date | Belirtilen tarih saat değeri. |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class with the fieldID which equals to this object's fieldID value.
### createLookupResourceDefinition(int customFieldType, int fieldId, String alias) {#createLookupResourceDefinition-int-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createLookupResourceDefinition(int customFieldType, int fieldId, String alias)
```


Arama ile genişletilmiş öznitelik tanımı oluşturan fabrika yöntemi. `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) değeri [CalculationType.Lookup](../../com.aspose.tasks/calculationtype\#Lookup) eşittir ve yalnızca Kaynaklarda kullanılabilir. Bu yöntemi çağırırken `customFieldType`, `fieldId` ve `alias` belirtmeniz gerekir.

--------------------

&gt; ```
&gt; Bu örneği, arama içeren bir kaynak için özel alan tanımı oluşturmak ve ardından metin değerleriyle doldurmak için kullanın:
&gt; ``````

ExtendedAttributeDefinition resourceTextAttr = ExtendedAttributeDefinition.createLookupResourceDefinition(ExtendedAttributeResource.Text27, "Özel alanım");
resourceTextAttr.addLookupValue(new Value() {{
this.setId(1);
this.setVal("Metin değeri 1");
this.setDescription("Metin değeri açıklaması 1");
}});
resourceTextAttr.addLookupValue(new Value() {{
this.setId(2);
this.setVal("Metin değeri 2");
this.setDescription("Metin değeri açıklaması 2");
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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fieldId | int | Belirtilen [ExtendedAttributeResource](../../com.aspose.tasks/extendedattributeresource) alan kimliği. |
| alias | java.lang.String | Belirtilen String alias. |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `fieldId` and `alias`.
### createLookupTaskDefinition(int customFieldType, int fieldId, String alias) {#createLookupTaskDefinition-int-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createLookupTaskDefinition(int customFieldType, int fieldId, String alias)
```


Arama ile genişletilmiş öznitelik tanımı oluşturan fabrika yöntemi. `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) değeri [CalculationType.Lookup](../../com.aspose.tasks/calculationtype\#Lookup) olarak eşittir ve yalnızca Görevlerde kullanılabilir. Bu yöntemi çağırırken `customFieldType`, `fieldId` ve `alias` belirtmeniz gerekir.

--------------------

&gt; ```
&gt; Bu örneği, arama içeren bir görev için özel alan tanımı oluşturmak ve ardından metin değerleriyle doldurmak için kullanın:
&gt; ``````

ExtendedAttributeDefinition taskTextAttr = ExtendedAttributeDefinition.createLookupTaskDefinition(CustomFieldType.Text, ExtendedAttributeResource.Text27, "My custom field");
taskTextAttr.addLookupValue(new Value() {{
this.setId(1);
this.setVal("Metin değeri 1");
this.setDescription("Metin değeri açıklaması 1");
}});
taskTextAttr.addLookupValue(new Value() {{
this.setId(2);
this.setVal("Metin değeri 2");
this.setDescription("Metin değeri açıklaması 2");
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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fieldId | int | Belirtilen [ExtendedAttributeTask](../../com.aspose.tasks/extendedattributetask) alan kimliği. |
| alias | java.lang.String | Belirtilen String alias. |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `fieldId` and `alias`.
### createResourceDefinition(int customFieldType, int fieldId, String alias) {#createResourceDefinition-int-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createResourceDefinition(int customFieldType, int fieldId, String alias)
```


Basit bir genişletilmiş öznitelik tanımı oluşturan fabrika yöntemi, Microsoft Project'te "None" olarak gösterilir. `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) değeri [CalculationType.None](../../com.aspose.tasks/calculationtype\#None) olarak eşittir ve yalnızca Kaynakta kullanılabilir. Bu yöntemi çağırırken `customFieldType`, `fieldId` ve `alias` belirtmeniz gerekir.

--------------------

&gt; ```
&gt; Özel metin alanı tanımı oluşturmak için bu örneği kullanın:
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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fieldId | int | Belirtilen [ExtendedAttributeResource](../../com.aspose.tasks/extendedattributeresource) alan kimliği. |
| alias | java.lang.String | Belirtilen String alias. |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `fieldId` and `alias`.
### createTaskDefinition(int customFieldType, int fieldId, String alias) {#createTaskDefinition-int-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createTaskDefinition(int customFieldType, int fieldId, String alias)
```


Basit bir genişletilmiş öznitelik tanımı oluşturan fabrika yöntemi, Microsoft Project'te "None" olarak gösterilir. `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) değeri [CalculationType.None](../../com.aspose.tasks/calculationtype\#None) olarak eşittir ve yalnızca Görevlerde kullanılabilir. Bu yöntemi çağırırken `customFieldType`, `fieldId` ve `alias` belirtmeniz gerekir.

--------------------

&gt; ```
&gt; Özel metin alanı tanımı oluşturmak için bu örneği kullanın:
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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fieldId | int | Belirtilen [ExtendedAttributeTask](../../com.aspose.tasks/extendedattributetask) alan kimliği. |
| alias | java.lang.String | Belirtilen String alias. |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `fieldId` and `alias`.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Bu örneğin belirtilen nesneye eşit olup olmadığını gösteren bir bayrak döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| obj | java.lang.Object | bu örnek ile karşılaştırılacak belirtilen nesne. |

**Returns:**
boolean - bu örneğin belirtilen nesneye eşit olup olmadığını gösteren bir işaret.
### getAlias() {#getAlias--}
```
public final String getAlias()
```


Özel bir alanın takma adını alır.

**Returns:**
java.lang.String - bir özel alanın alias'ı.
### getAppendNewValues() {#getAppendNewValues--}
```
public final boolean getAppendNewValues()
```


Projeye eklenen yeni değerlerin otomatik olarak listeye eklenip eklenmediğini gösteren bir değeri alır.

--------------------

Şu anda MSP 2003/2007 Xml ve MSP 2003 mpp formatları için desteklenmektedir.

**Returns:**
boolean - bir projeye eklenen yeni değerlerin otomatik olarak listeye eklenip eklenmediğini gösteren bir değer.
### getAutoRollDown() {#getAutoRollDown--}
```
public final boolean getAutoRollDown()
```


Atamalara otomatik olarak aşağı kaydırmanın etkin olup olmadığını gösteren bir değeri alır.

**Returns:**
boolean - atamalara otomatik olarak aşağı kaydırmanın etkin olup olmadığını gösteren bir değer.
### getCalculationType() {#getCalculationType--}
```
public final int getCalculationType()
```


Özel özniteliğin değerinin hesaplama türünü alır.

**Returns:**
int - özel öznitelik değerinin hesaplama türü.
### getCfType() {#getCfType--}
```
public final int getCfType()
```


Özel bir alanın türünü alır.

**Returns:**
int - bir özel alanın türü.
### getDefault() {#getDefault--}
```
public final String getDefault()
```


Listedeki varsayılan değeri alır.

--------------------

Şu anda MSP 2003/2007 Xml ve MSP 2003 mpp formatları için desteklenmektedir.

**Returns:**
java.lang.String - listedeki varsayılan değer.
### getDefaultGuid() {#getDefaultGuid--}
```
public final String getDefaultGuid()
```


Varsayılan arama tablosu girişinin GUID'sini alır.

**Returns:**
java.lang.String - varsayılan arama tablosu girişinin Guid'i.
### getElementType() {#getElementType--}
```
public final int getElementType()
```


Genişletilmiş özniteliğin bir görev, bir kaynak veya bir atama ile ilişkili olup olmadığını alır.

**Returns:**
int - genişletilmiş öznitelik bir görev, bir kaynak veya bir atama ile ilişkilidir.
### getFieldId() {#getFieldId--}
```
public final String getFieldId()
```


Gets, özel bir alanın proje kimliğine karşılık gelir. [ExtendedAttributeTask](../../com.aspose.tasks/extendedattributetask) sınıfından bir sabitin dize temsilini kullanarak `FieldId`([getFieldId()](../../com.aspose.tasks/extendedattributedefinition\#getFieldId--)/ [setFieldId(String)](../../com.aspose.tasks/extendedattributedefinition\#setFieldId-String-)) özelliğini belirtin.

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

Tercih edilen yol `FieldId`([getFieldId()](../../com.aspose/tasks/extendedattributedefinition\#getFieldId--)/ [setFieldId(String)](../../com.aspose/tasks/extendedattributedefinition\#setFieldId-String-)) özelliğini ayarlamaktır; bunun için [ExtendedAttributeDefinition](../../com.aspose/tasks/extendedattributedefinition) kullanılarak, [createTaskDefinition(int, String)](../../com.aspose/tasks/extendedattributedefinition\#createTaskDefinition-int--String-) veya [createLookupTaskDefinition(int, int, String)](../../com.aspose/tasks/extendedattributedefinition\#createLookupTaskDefinition-int--int--String-) gibi özel fabrika yöntemlerinden biriyle oluşturulur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | özel bir alanın proje kimliğine karşılık gelir. |

### setFormula(String value) {#setFormula-java.lang.String-}
```
public final void setFormula(String value)
```


Microsoft Project'in özel görev alanını doldurmak için kullandığı formülü ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | Microsoft Project'in özel bir görev alanını doldurmak için kullandığı formül. |

### setGraphicalIndicator(GraphicalIndicatorsInfo value) {#setGraphicalIndicator-com.aspose.tasks.GraphicalIndicatorsInfo-}
```
public final void setGraphicalIndicator(GraphicalIndicatorsInfo value)
```


Genişletilmiş öznitelikle ilişkili grafik göstergeler bilgisini ayarlar. MPP formatı için geçerlidir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [GraphicalIndicatorsInfo](../../com.aspose.tasks/graphicalindicatorsinfo) | Genişletilmiş öznitelikle ilişkili grafik göstergeler bilgisi. |

### setGuid(String value) {#setGuid-java.lang.String-}
```
public final void setGuid(String value)
```


Özel bir alanın GUID'sini ayarlar.

--------------------

Şu anda yalnızca Xml formatı için desteklenmektedir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | özel bir alanın Guid'i. |

### setMaxMultiValues(int value) {#setMaxMultiValues-int-}
```
public final void setMaxMultiValues(int value)
```


Seçim listesindeki ayarlanabilecek maksimum değer sayısını belirler.

--------------------

Şu anda yalnızca Xml formatı için desteklenmektedir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | seçim listesine ayarlayabileceğiniz maksimum değer sayısı. |

### setPhoneticsAlias(String value) {#setPhoneticsAlias-java.lang.String-}
```
public final void setPhoneticsAlias(String value)
```


Özel bir alanın takma adının fonetik telaffuzunu ayarlar.

--------------------

Şu anda yalnızca Xml formatı için desteklenmektedir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | özel bir alanın takma adının fonetik telaffuzu. |

### setRestrictValues(boolean value) {#setRestrictValues-boolean-}
```
public final void setRestrictValues(boolean value)
```


Özel alan değerlerinin `ValueList`([getValueList()](../../com.aspose.tasks/extendedattributedefinition\\#getValueList--)/ [setValueList(List)](../../com.aspose.tasks/extendedattributedefinition\\#setValueList-List-Value--)) içinde sınırlı olup olmadığını gösteren bir değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | özel alan değerlerinin, içinde bulunan değerlere sınırlı olup olmadığını gösteren bir değer |

### setRollupType(int value) {#setRollupType-int-}
```
public final void setRollupType(int value)
```


Toplamların nasıl hesaplandığını ayarlar.

--------------------

Yazma şu anda yalnızca Xml formatı için desteklenmektedir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | toplamların hesaplanma şekli. |

### setSecondaryGuid(String value) {#setSecondaryGuid-java.lang.String-}
```
public final void setSecondaryGuid(String value)
```


Uzatılmış özniteliğin ikincil GUID'sini ayarlar.

--------------------

Bu, MS Project 2010 özelliği için yenidir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | genişletilmiş öznitelğin ikincil guid'i. |

### setSecondaryPid(String value) {#setSecondaryPid-java.lang.String-}
```
public final void setSecondaryPid(String value)
```


Özel bir alanın ikincil PID'sini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | özel bir alanın ikincil PID'si. |

### setSummaryRowsCalculationType(int value) {#setSummaryRowsCalculationType-int-}
```
public final void setSummaryRowsCalculationType(int value)
```


Özet satırları için özel özniteliğin değerinin hesaplama türünü ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | özet satırlar için özel öznitelik değerinin hesaplama türü. |

### setUserDef(boolean value) {#setUserDef-boolean-}
```
public final void setUserDef(boolean value)
```


Özel bir alanın kullanıcı tarafından tanımlanıp tanımlanmadığını gösteren bir değeri ayarlar.

--------------------

Şu anda yalnızca Xml formatı için desteklenmektedir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | özel bir alanın kullanıcı tarafından tanımlanıp tanımlanmadığını gösteren bir değer. |

### setValuelistSortOrder(int value) {#setValuelistSortOrder-int-}
```
public final void setValuelistSortOrder(int value)
```


Değer listelerinin sıralama şeklini ayarlar. Değerler: 0=Azalan, 1=Artan.

--------------------

Şu anda MSP 2003/2007 Xml ve MSP 2003 mpp formatları için desteklenmektedir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | değer listelerinin sıralanma şekli. |

