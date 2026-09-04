---
title: "ExtendedAttributeDefinition"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل تعريف سمة موسعة مرتبطة بمشروع."
type: docs
weight: 83
url: /ar/java/com.aspose.tasks/extendedattributedefinition/
---

**Inheritance:**
java.lang.Object
```
public class ExtendedAttributeDefinition
```

يمثل تعريف سمة موسعة مرتبطة بمشروع.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [addLookupValue(Value value)](#addLookupValue-com.aspose.tasks.Value-) | يضيف قيمة إلى قائمة البحث الداخلية. |
| [compareTo(ExtendedAttributeDefinition o)](#compareTo-com.aspose.tasks.ExtendedAttributeDefinition-) | يقارن هذا الكائن مع كائن آخر من فئة @\\{code ExtendedAttributeDefinition\\}. |
| [createExtendedAttribute()](#createExtendedAttribute--) | ينشئ سمة موسعة جديدة بمعرف الحقل الذي يساوي قيمة معرف الحقل لهذا الكائن. |
| [createExtendedAttribute(boolean flagValue)](#createExtendedAttribute-boolean-) | ينشئ سمة موسعة جديدة بمعرف الحقل الذي يساوي قيمة معرف الحقل لهذا الكائن والقيمة المحددة للعلامة. |
| [createExtendedAttribute(Duration durationValue)](#createExtendedAttribute-com.aspose.tasks.Duration-) | ينشئ سمة موسعة جديدة بمعرف الحقل الذي يساوي قيمة معرف الحقل لهذا الكائن والقيمة المحددة للمدة. |
| [createExtendedAttribute(Value lookupValue)](#createExtendedAttribute-com.aspose.tasks.Value-) | ينشئ سمة موسعة جديدة مرتبطة بالعنصر [Value](../../com.aspose.tasks/value) المحدد. |
| [createExtendedAttribute(String textValue)](#createExtendedAttribute-java.lang.String-) | ينشئ سمة موسعة جديدة بمعرف الحقل الذي يساوي قيمة معرف الحقل لهذا الكائن والقيمة المحددة للنص. |
| [createExtendedAttribute(BigDecimal numericValue)](#createExtendedAttribute-java.math.BigDecimal-) | ينشئ سمة موسعة جديدة بمعرف الحقل الذي يساوي قيمة معرف الحقل لهذا الكائن والقيمة المحددة للرقم. |
| [createExtendedAttribute(Date dateTimeValue)](#createExtendedAttribute-java.util.Date-) | ينشئ سمة موسعة جديدة بمعرف الحقل الذي يساوي قيمة معرف الحقل لهذا الكائن والقيمة المحددة للتاريخ. |
| [createLookupResourceDefinition(int customFieldType, int fieldId, String alias)](#createLookupResourceDefinition-int-int-java.lang.String-) | طريقة المصنع التي تنشئ تعريف سمة موسعة مع البحث. |
| [createLookupResourceDefinition(int fieldId, String alias)](#createLookupResourceDefinition-int-java.lang.String-) | طريقة المصنع التي تنشئ تعريف سمة موسعة مع البحث. |
| [createLookupTaskDefinition(int customFieldType, int fieldId, String alias)](#createLookupTaskDefinition-int-int-java.lang.String-) | طريقة المصنع التي تنشئ تعريف سمة موسعة مع البحث. |
| [createLookupTaskDefinition(int fieldId, String alias)](#createLookupTaskDefinition-int-java.lang.String-) | طريقة المصنع التي تنشئ تعريف سمة موسعة مع البحث. |
| [createResourceDefinition(int customFieldType, int fieldId, String alias)](#createResourceDefinition-int-int-java.lang.String-) | طريقة المصنع التي تنشئ تعريف سمة موسعة بسيطة، والتي يظهرها Microsoft Project كـ \"None\". |
| [createResourceDefinition(int fieldId, String alias)](#createResourceDefinition-int-java.lang.String-) | طريقة المصنع التي تنشئ تعريف سمة موسعة بسيطة، والتي يظهرها Microsoft Project كـ \"None\". |
| [createTaskDefinition(int customFieldType, int fieldId, String alias)](#createTaskDefinition-int-int-java.lang.String-) | طريقة المصنع التي تنشئ تعريف سمة موسعة بسيطة، والتي يظهرها Microsoft Project كـ \"None\". |
| [createTaskDefinition(int fieldId, String alias)](#createTaskDefinition-int-java.lang.String-) | طريقة المصنع التي تنشئ تعريف سمة موسعة بسيطة، والتي يظهرها Microsoft Project كـ \"None\". |
| [equals(Object obj)](#equals-java.lang.Object-) | يرجع علامة تشير إلى ما إذا كان هذا الكائن مساويًا للكيان المحدد. |
| [getAlias()](#getAlias--) | يحصل على الاسم المستعار لحقل مخصص. |
| [getAppendNewValues()](#getAppendNewValues--) | يحصل على قيمة تشير إلى ما إذا كانت القيم الجديدة المضافة إلى المشروع تُضاف تلقائيًا إلى القائمة. |
| [getAutoRollDown()](#getAutoRollDown--) | يحصل على قيمة تشير إلى ما إذا كان الانحدار التلقائي إلى التعيينات مفعلاً. |
| [getCalculationType()](#getCalculationType--) | يحصل على نوع حساب قيمة السمة المخصصة. |
| [getCfType()](#getCfType--) | يحصل على نوع الحقل المخصص. |
| [getDefault()](#getDefault--) | يحصل على القيمة الافتراضية في القائمة. |
| [getDefaultGuid()](#getDefaultGuid--) | يحصل على الـ Guid لمدخل جدول البحث الافتراضي. |
| [getElementType()](#getElementType--) | يحصل على ما إذا كانت السمة الموسعة مرتبطة بمهمة أو مورد أو تعيين. |
| [getFieldId()](#getFieldId--) | يحصل على معرف المشروع المقابل لحقل مخصص. |
| [getFieldName()](#getFieldName--) | يحصل على اسم الحقل المخصص. |
| [getFormula()](#getFormula--) | يحصل على الصيغة التي يستخدمها Microsoft Project لملء حقل مهمة مخصص. |
| [getGraphicalIndicator()](#getGraphicalIndicator--) | يحصل على معلومات المؤشرات الرسومية المرتبطة بالسمة الموسعة. |
| [getGuid()](#getGuid--) | يحصل على الـ Guid لحقل مخصص. |
| [getLookupUid()](#getLookupUid--) | يحصل على Guid لجدول البحث المرتبط بحقل مخصص. |
| [getMaxMultiValues()](#getMaxMultiValues--) | يحصل على الحد الأقصى لعدد القيم التي يمكنك تعيينها في قائمة اختيار. |
| [getParentProject()](#getParentProject--) | يحصل على المشروع الأب لـمثيل [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition). |
| [getPhoneticsAlias()](#getPhoneticsAlias--) | يحصل على النطق الصوتي للاسم المستعار لحقل مخصص. |
| [getRestrictValues()](#getRestrictValues--) | يحصل على قيمة تشير إلى ما إذا كانت قيم الحقل المخصص مقيدة بالقيم الموجودة في `ValueList`([getValueList()](../../com.aspose.tasks/extendedattributedefinition\#getValueList--)/ [setValueList(List)](../../com.aspose.tasks/extendedattributedefinition\#setValueList-List-Value--)). |
| [getRollupType()](#getRollupType--) | يحصل على طريقة حساب التجميعات. |
| [getSecondaryGuid()](#getSecondaryGuid--) | يحصل على الـ guid الثانوي للسمة الموسعة. |
| [getSecondaryPid()](#getSecondaryPid--) | يحصل على الـ PID الثانوي لحقل مخصص. |
| [getSummaryRowsCalculationType()](#getSummaryRowsCalculationType--) | يحصل على نوع حساب قيمة السمة المخصصة لصفوف الملخص. |
| [getUserDef()](#getUserDef--) | يحصل على قيمة تشير إلى ما إذا كان الحقل المخصص معرفًا من قبل المستخدم. |
| [getValueList()](#getValueList--) | يحصل على List&lt;Value&gt; ValueList. |
| [getValuelistSortOrder()](#getValuelistSortOrder--) | يحصل على طريقة فرز قوائم القيم. |
| [hashCode()](#hashCode--) | يعيد رمز تجزئة للنسخة من الفئة [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition). |
| [removeLookupValue(Value value)](#removeLookupValue-com.aspose.tasks.Value-) | يزيل قيمة من قائمة البحث الداخلية. |
| [setAlias(String value)](#setAlias-java.lang.String-) | يضبط الاسم المستعار لحقل مخصص. |
| [setAppendNewValues(boolean value)](#setAppendNewValues-boolean-) | يضبط قيمة تشير إلى ما إذا كانت القيم الجديدة المضافة إلى المشروع تُضاف تلقائيًا إلى القائمة. |
| [setAutoRollDown(boolean value)](#setAutoRollDown-boolean-) | يضبط قيمة تشير إلى ما إذا كان الانحدار التلقائي إلى التعيينات مفعلاً. |
| [setCalculationType(int value)](#setCalculationType-int-) | يضبط نوع حساب قيمة السمة المخصصة. |
| [setDefault(String value)](#setDefault-java.lang.String-) | يضبط القيمة الافتراضية في القائمة. |
| [setDefaultGuid(String value)](#setDefaultGuid-java.lang.String-) | يضبط الـ Guid لمدخل جدول البحث الافتراضي. |
| [setElementType(int value)](#setElementType-int-) | يضبط ما إذا كانت السمة الموسعة مرتبطة بمهمة أو مورد أو تعيين. |
| [setFieldId(String value)](#setFieldId-java.lang.String-) | يضبط ما يتCorrespond إلى معرف المشروع لحقل مخصص. |
| [setFormula(String value)](#setFormula-java.lang.String-) | يضبط الصيغة التي يستخدمها Microsoft Project لملء حقل مهمة مخصص. |
| [setGraphicalIndicator(GraphicalIndicatorsInfo value)](#setGraphicalIndicator-com.aspose.tasks.GraphicalIndicatorsInfo-) | يضبط معلومات المؤشرات الرسومية المرتبطة بالسمة الموسعة. |
| [setGuid(String value)](#setGuid-java.lang.String-) | يضبط الـ Guid لحقل مخصص. |
| [setMaxMultiValues(int value)](#setMaxMultiValues-int-) | يضبط الحد الأقصى لعدد القيم التي يمكنك ضبطها في قائمة اختيار. |
| [setPhoneticsAlias(String value)](#setPhoneticsAlias-java.lang.String-) | يضبط النطق الفونيمي للاسم المستعار لحقل مخصص. |
| [setRestrictValues(boolean value)](#setRestrictValues-boolean-) | يضبط قيمة تشير إلى ما إذا كانت قيم الحقل المخصص مقيدة بالقيم الموجودة في `ValueList`([getValueList()](../../com.aspose.tasks/extendedattributedefinition\#getValueList--)/ [setValueList(List)](../../com.aspose.tasks/extendedattributedefinition\#setValueList-List-Value--)). |
| [setRollupType(int value)](#setRollupType-int-) | يضبط طريقة حساب التجميعات. |
| [setSecondaryGuid(String value)](#setSecondaryGuid-java.lang.String-) | يضبط الـ guid الثانوي للسمة الموسعة. |
| [setSecondaryPid(String value)](#setSecondaryPid-java.lang.String-) | يضبط الـ PID الثانوي لحقل مخصص. |
| [setSummaryRowsCalculationType(int value)](#setSummaryRowsCalculationType-int-) | يضبط نوع حساب قيمة السمة المخصصة لصفوف الملخص. |
| [setUserDef(boolean value)](#setUserDef-boolean-) | يضبط قيمة تشير إلى ما إذا كان الحقل المخصص معرفًا من قبل المستخدم. |
| [setValuelistSortOrder(int value)](#setValuelistSortOrder-int-) | يضبط طريقة فرز قوائم القيم. |
### addLookupValue(Value value) {#addLookupValue-com.aspose.tasks.Value-}
```
public final void addLookupValue(Value value)
```


يضيف قيمة إلى قائمة البحث الداخلية. هذه طريقة مفضلة للتعامل مع `ValueList`([getValueList()](../../com.aspose.tasks/extendedattributedefinition\#getValueList--)/ [setValueList(List)](../../com.aspose.tasks/extendedattributedefinition\#setValueList-List-Value--)).

--------------------

&gt; ```
&gt; استخدم هذا الكود لإضافة قيمة جديدة إلى قائمة البحث:
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
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | lookupValue | [Value](../../com.aspose.tasks/value) | العنصر [Value](../../com.aspose.tasks/value) المحدد. |

--------------------

`lookupValue` يجب أن يُضاف مسبقًا إلى [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) باستخدام طريقة [addLookupValue(Value)](../../com.aspose.tasks/extendedattributedefinition\#addLookupValue-Value-) . |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class linked with specified [Value](../../com.aspose.tasks/value) item.
### createExtendedAttribute(String textValue) {#createExtendedAttribute-java.lang.String-}
```
public final ExtendedAttribute createExtendedAttribute(String textValue)
```


ينشئ سمة موسعة جديدة بمعرف الحقل الذي يساوي قيمة معرف الحقل لهذا الكائن والقيمة المحددة للنص.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| textValue | java.lang.String | قيمة النص المحددة. |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class with the fieldID which equals to this object's fieldID value.
### createExtendedAttribute(BigDecimal numericValue) {#createExtendedAttribute-java.math.BigDecimal-}
```
public final ExtendedAttribute createExtendedAttribute(BigDecimal numericValue)
```


ينشئ سمة موسعة جديدة بمعرف الحقل الذي يساوي قيمة معرف الحقل لهذا الكائن والقيمة المحددة للرقم.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| numericValue | java.math.BigDecimal | قيمة عددية محددة. |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class with the fieldID which equals to this object's fieldID value.
### createExtendedAttribute(Date dateTimeValue) {#createExtendedAttribute-java.util.Date-}
```
public final ExtendedAttribute createExtendedAttribute(Date dateTimeValue)
```


ينشئ سمة موسعة جديدة بمعرف الحقل الذي يساوي قيمة معرف الحقل لهذا الكائن والقيمة المحددة للتاريخ.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| dateTimeValue | java.util.Date | قيمة تاريخ/وقت محددة. |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class with the fieldID which equals to this object's fieldID value.
### createLookupResourceDefinition(int customFieldType, int fieldId, String alias) {#createLookupResourceDefinition-int-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createLookupResourceDefinition(int customFieldType, int fieldId, String alias)
```


طريقة المصنع التي تنشئ تعريف سمة ممتدة مع lookup. لديها `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) تساوي [CalculationType.Lookup](../../com.aspose.tasks/calculationtype\#Lookup) ويمكن استخدامها في الموارد فقط. يُطلب منك تحديد `customFieldType` و `fieldId` و `alias` عند استدعاء هذه الطريقة.

--------------------

&gt; ```
&gt; استخدم هذا المثال لإنشاء تعريف حقل مخصص لمورد مع lookup ثم ملئه بقيم نصية:
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
| معامل | نوع | الوصف |
| --- | --- | --- |
| fieldId | int | معرف الحقل المحدد لـ [ExtendedAttributeResource](../../com.aspose.tasks/extendedattributeresource). |
| الاسم المستعار | java.lang.String | الاسم المستعار من نوع String المحدد. |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `fieldId` and `alias`.
### createLookupTaskDefinition(int customFieldType, int fieldId, String alias) {#createLookupTaskDefinition-int-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createLookupTaskDefinition(int customFieldType, int fieldId, String alias)
```


طريقة المصنع التي تنشئ تعريف سمة موسعة مع بحث. تحتوي على `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) وتساوي [CalculationType.Lookup](../../com.aspose.tasks/calculationtype\#Lookup) ويمكن استخدامها في المهام فقط. يجب عليك تحديد `customFieldType` و `fieldId` و `alias` عند استدعاء هذه الطريقة.

--------------------

&gt; ```
&gt; استخدم هذا المثال لإنشاء تعريف حقل مخصص لمهمة مع بحث ثم ملئه بقيم نصية:
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
| معامل | نوع | الوصف |
| --- | --- | --- |
| fieldId | int | معرف الحقل المحدد لـ [ExtendedAttributeTask](../../com.aspose.tasks/extendedattributetask). |
| الاسم المستعار | java.lang.String | الاسم المستعار من نوع String المحدد. |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `fieldId` and `alias`.
### createResourceDefinition(int customFieldType, int fieldId, String alias) {#createResourceDefinition-int-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createResourceDefinition(int customFieldType, int fieldId, String alias)
```


طريقة المصنع التي تنشئ تعريف سمة موسعة بسيط، حيث يعرض Microsoft Project القيمة "None". تحتوي على `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) وتساوي [CalculationType.None](../../com.aspose.tasks/calculationtype\#None) ويمكن استخدامها في الموارد فقط. يجب عليك تحديد `customFieldType` و `fieldId` و `alias` عند استدعاء هذه الطريقة.

--------------------

&gt; ```
&gt; استخدم هذا المثال لإنشاء تعريف حقل نصي مخصص:
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
| معامل | نوع | الوصف |
| --- | --- | --- |
| fieldId | int | معرف الحقل المحدد لـ [ExtendedAttributeResource](../../com.aspose.tasks/extendedattributeresource). |
| الاسم المستعار | java.lang.String | الاسم المستعار من نوع String المحدد. |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `fieldId` and `alias`.
### createTaskDefinition(int customFieldType, int fieldId, String alias) {#createTaskDefinition-int-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createTaskDefinition(int customFieldType, int fieldId, String alias)
```


طريقة المصنع التي تنشئ تعريف سمة موسعة بسيط، حيث يعرض Microsoft Project القيمة "None". تحتوي على `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) وتساوي [CalculationType.None](../../com.aspose.tasks/calculationtype\#None) ويمكن استخدامها في المهام فقط. يجب عليك تحديد `customFieldType` و `fieldId` و `alias` عند استدعاء هذه الطريقة.

--------------------

&gt; ```
&gt; استخدم هذا المثال لإنشاء تعريف حقل نصي مخصص:
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
| معامل | نوع | الوصف |
| --- | --- | --- |
| fieldId | int | معرف الحقل المحدد لـ [ExtendedAttributeTask](../../com.aspose.tasks/extendedattributetask). |
| الاسم المستعار | java.lang.String | الاسم المستعار من نوع String المحدد. |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `fieldId` and `alias`.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


يرجع علامة تشير إلى ما إذا كان هذا الكائن مساويًا للكيان المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| obj | java.lang.Object | الكائن المحدد للمقارنة مع هذه الحالة. |

**Returns:**
boolean - علامة تشير إلى ما إذا كانت هذه الحالة مساوية للكائن المحدد.
### getAlias() {#getAlias--}
```
public final String getAlias()
```


يحصل على الاسم المستعار لحقل مخصص.

**Returns:**
java.lang.String - الاسم المستعار لحقل مخصص.
### getAppendNewValues() {#getAppendNewValues--}
```
public final boolean getAppendNewValues()
```


يحصل على قيمة تشير إلى ما إذا كانت القيم الجديدة المضافة إلى المشروع تُضاف تلقائيًا إلى القائمة.

--------------------

مدعوم حاليًا لتنسيقات MSP 2003/2007 Xml و MSP 2003 mpp.

**Returns:**
boolean - قيمة تشير إلى ما إذا كانت القيم الجديدة المضافة إلى المشروع تُضاف تلقائيًا إلى القائمة.
### getAutoRollDown() {#getAutoRollDown--}
```
public final boolean getAutoRollDown()
```


يحصل على قيمة تشير إلى ما إذا كان الانحدار التلقائي إلى التعيينات مفعلاً.

**Returns:**
boolean - قيمة تشير إلى ما إذا كان التوزيع التلقائي إلى التعيينات مفعلاً.
### getCalculationType() {#getCalculationType--}
```
public final int getCalculationType()
```


يحصل على نوع حساب قيمة السمة المخصصة.

**Returns:**
int - نوع حساب قيمة السمة المخصصة.
### getCfType() {#getCfType--}
```
public final int getCfType()
```


يحصل على نوع الحقل المخصص.

**Returns:**
int - نوع الحقل المخصص.
### getDefault() {#getDefault--}
```
public final String getDefault()
```


يحصل على القيمة الافتراضية في القائمة.

--------------------

مدعوم حاليًا لتنسيقات MSP 2003/2007 Xml و MSP 2003 mpp.

**Returns:**
java.lang.String - القيمة الافتراضية في القائمة.
### getDefaultGuid() {#getDefaultGuid--}
```
public final String getDefaultGuid()
```


يحصل على الـ Guid لمدخل جدول البحث الافتراضي.

**Returns:**
java.lang.String - Guid للمدخل الافتراضي في جدول البحث.
### getElementType() {#getElementType--}
```
public final int getElementType()
```


يحصل على ما إذا كانت السمة الموسعة مرتبطة بمهمة أو مورد أو تعيين.

**Returns:**
int - السمة الموسعة مرتبطة بمهمة أو مورد أو تعيين.
### getFieldId() {#getFieldId--}
```
public final String getFieldId()
```


Gets تتطابق مع معرف المشروع لحقل مخصص. استخدم تمثيل السلسلة لثابت من الفئة [ExtendedAttributeTask](../../com.aspose.tasks/extendedattributetask) لتحديد `FieldId`([getFieldId()](../../com.aspose.tasks/extendedattributedefinition\#getFieldId--)/ [setFieldId(String)](../../com.aspose.tasks/extendedattributedefinition\#setFieldId-String-)) الخاصية.

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

الطريقة المفضلة لتعيين `FieldId`([getFieldId()](../../com.aspose/tasks/extendedattributedefinition\#getFieldId--)/ [setFieldId(String)](../../com.aspose/tasks/extendedattributedefinition\#setFieldId-String-)) الخاصية هي إنشاء [ExtendedAttributeDefinition](../../com.aspose/tasks/extendedattributedefinition) باستخدام إحدى طرق المصنع المخصصة مثل [createTaskDefinition(int, String)](../../com.aspose/tasks/extendedattributedefinition\#createTaskDefinition-int--String-) أو [createLookupTaskDefinition(int, int, String)](../../com.aspose/tasks/extendedattributedefinition\#createLookupTaskDefinition-int--int--String-).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | يتطابق مع معرف المشروع لحقل مخصص. |

### setFormula(String value) {#setFormula-java.lang.String-}
```
public final void setFormula(String value)
```


يضبط الصيغة التي يستخدمها Microsoft Project لملء حقل مهمة مخصص.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | الصيغة التي يستخدمها Microsoft Project لملء حقل مهمة مخصص. |

### setGraphicalIndicator(GraphicalIndicatorsInfo value) {#setGraphicalIndicator-com.aspose.tasks.GraphicalIndicatorsInfo-}
```
public final void setGraphicalIndicator(GraphicalIndicatorsInfo value)
```


يضبط معلومات مؤشرات رسومية مرتبطة بالخاصية الموسعة. ينطبق على تنسيق MPP.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [GraphicalIndicatorsInfo](../../com.aspose.tasks/graphicalindicatorsinfo) | معلومات مؤشرات رسومية مرتبطة بالخاصية الموسعة. |

### setGuid(String value) {#setGuid-java.lang.String-}
```
public final void setGuid(String value)
```


يضبط الـ Guid لحقل مخصص.

--------------------

مدعوم حاليًا لتنسيق Xml فقط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | معرف GUID لحقل مخصص. |

### setMaxMultiValues(int value) {#setMaxMultiValues-int-}
```
public final void setMaxMultiValues(int value)
```


يضبط الحد الأقصى لعدد القيم التي يمكنك ضبطها في قائمة اختيار.

--------------------

مدعوم حاليًا لتنسيق Xml فقط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | الحد الأقصى لعدد القيم التي يمكنك تعيينها في قائمة اختيار. |

### setPhoneticsAlias(String value) {#setPhoneticsAlias-java.lang.String-}
```
public final void setPhoneticsAlias(String value)
```


يضبط النطق الفونيمي للاسم المستعار لحقل مخصص.

--------------------

مدعوم حاليًا لتنسيق Xml فقط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | النطق الصوتي للكنية لحقل مخصص. |

### setRestrictValues(boolean value) {#setRestrictValues-boolean-}
```
public final void setRestrictValues(boolean value)
```


يضبط قيمة تشير إلى ما إذا كانت قيم الحقل المخصص مقيدة بالقيم الموجودة في `ValueList`([getValueList()](../../com.aspose.tasks/extendedattributedefinition\#getValueList--)/ [setValueList(List)](../../com.aspose.tasks/extendedattributedefinition\#setValueList-List-Value--)).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كانت قيم الحقل المخصص مقيدة بالقيم في الـ |

### setRollupType(int value) {#setRollupType-int-}
```
public final void setRollupType(int value)
```


يضبط طريقة حساب التجميعات.

--------------------

الكتابة مدعومة حاليًا لتنسيق Xml فقط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | طريقة حساب التجميعات. |

### setSecondaryGuid(String value) {#setSecondaryGuid-java.lang.String-}
```
public final void setSecondaryGuid(String value)
```


يضبط الـ guid الثانوي للسمة الموسعة.

--------------------

هذا جديد لخاصية MS Project 2010.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | معرف GUID الثانوي للخاصية الموسعة. |

### setSecondaryPid(String value) {#setSecondaryPid-java.lang.String-}
```
public final void setSecondaryPid(String value)
```


يضبط الـ PID الثانوي لحقل مخصص.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | معرف PID الثانوي لحقل مخصص. |

### setSummaryRowsCalculationType(int value) {#setSummaryRowsCalculationType-int-}
```
public final void setSummaryRowsCalculationType(int value)
```


يضبط نوع حساب قيمة السمة المخصصة لصفوف الملخص.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | نوع حساب قيمة الخاصية المخصصة للصفوف المجمعة. |

### setUserDef(boolean value) {#setUserDef-boolean-}
```
public final void setUserDef(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان الحقل المخصص معرفًا من قبل المستخدم.

--------------------

مدعوم حاليًا لتنسيق Xml فقط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان الحقل المخصص معرفًا من قبل المستخدم. |

### setValuelistSortOrder(int value) {#setValuelistSortOrder-int-}
```
public final void setValuelistSortOrder(int value)
```


يضبط طريقة فرز قوائم القيم. القيم هي: 0=تنازلي، 1=تصاعدي.

--------------------

مدعوم حاليًا لتنسيقات MSP 2003/2007 Xml و MSP 2003 mpp.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | طريقة فرز قوائم القيم. |

