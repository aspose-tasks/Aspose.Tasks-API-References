---
title: "ExtendedAttributeDefinition"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "परियोजना से जुड़ी विस्तारित विशेषता परिभाषा को दर्शाता है।"
type: docs
weight: 83
url: /hi/java/com.aspose.tasks/extendedattributedefinition/
---

**Inheritance:**
java.lang.Object
```
public class ExtendedAttributeDefinition
```

परियोजना से जुड़ी विस्तारित विशेषता परिभाषा को दर्शाता है।
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [addLookupValue(Value value)](#addLookupValue-com.aspose.tasks.Value-) | आंतरिक लुकअप सूची में एक मान जोड़ता है। |
| [compareTo(ExtendedAttributeDefinition o)](#compareTo-com.aspose.tasks.ExtendedAttributeDefinition-) | इस वस्तु की तुलना @\{code ExtendedAttributeDefinition\} वर्ग की दूसरी उदाहरण से करता है। |
| [createExtendedAttribute()](#createExtendedAttribute--) | इस वस्तु के फ़ील्ड ID मान के बराबर फ़ील्ड ID के साथ एक नया विस्तारित गुण बनाता है। |
| [createExtendedAttribute(boolean flagValue)](#createExtendedAttribute-boolean-) | इस वस्तु के फ़ील्ड ID मान के बराबर फ़ील्ड ID और निर्दिष्ट फ़्लैग मान के साथ एक नया विस्तारित गुण बनाता है। |
| [createExtendedAttribute(Duration durationValue)](#createExtendedAttribute-com.aspose.tasks.Duration-) | इस वस्तु के फ़ील्ड ID मान के बराबर फ़ील्ड ID और निर्दिष्ट अवधि मान के साथ एक नया विस्तारित गुण बनाता है। |
| [createExtendedAttribute(Value lookupValue)](#createExtendedAttribute-com.aspose.tasks.Value-) | निर्दिष्ट [Value](../../com.aspose.tasks/value) आइटम के साथ जुड़ा नया विस्तारित गुण बनाता है। |
| [createExtendedAttribute(String textValue)](#createExtendedAttribute-java.lang.String-) | इस वस्तु के फ़ील्ड ID मान के बराबर फ़ील्ड ID और निर्दिष्ट पाठ मान के साथ एक नया विस्तारित गुण बनाता है। |
| [createExtendedAttribute(BigDecimal numericValue)](#createExtendedAttribute-java.math.BigDecimal-) | इस वस्तु के फ़ील्ड ID मान के बराबर फ़ील्ड ID और निर्दिष्ट संख्यात्मक मान के साथ एक नया विस्तारित गुण बनाता है। |
| [createExtendedAttribute(Date dateTimeValue)](#createExtendedAttribute-java.util.Date-) | इस वस्तु के फ़ील्ड ID मान के बराबर फ़ील्ड ID और निर्दिष्ट तिथि मान के साथ एक नया विस्तारित गुण बनाता है। |
| [createLookupResourceDefinition(int customFieldType, int fieldId, String alias)](#createLookupResourceDefinition-int-int-java.lang.String-) | फ़ैक्टरी मेथड जो लुकअप के साथ एक विस्तारित गुण परिभाषा बनाता है। |
| [createLookupResourceDefinition(int fieldId, String alias)](#createLookupResourceDefinition-int-java.lang.String-) | फ़ैक्टरी मेथड जो लुकअप के साथ एक विस्तारित गुण परिभाषा बनाता है। |
| [createLookupTaskDefinition(int customFieldType, int fieldId, String alias)](#createLookupTaskDefinition-int-int-java.lang.String-) | फ़ैक्टरी मेथड जो लुकअप के साथ एक विस्तारित गुण परिभाषा बनाता है। |
| [createLookupTaskDefinition(int fieldId, String alias)](#createLookupTaskDefinition-int-java.lang.String-) | फ़ैक्टरी मेथड जो लुकअप के साथ एक विस्तारित गुण परिभाषा बनाता है। |
| [createResourceDefinition(int customFieldType, int fieldId, String alias)](#createResourceDefinition-int-int-java.lang.String-) | फ़ैक्टरी मेथड जो एक सरल विस्तारित गुण परिभाषा बनाता है, जिसे Microsoft Project "None" के रूप में दिखाता है। |
| [createResourceDefinition(int fieldId, String alias)](#createResourceDefinition-int-java.lang.String-) | फ़ैक्टरी मेथड जो एक सरल विस्तारित गुण परिभाषा बनाता है, जिसे Microsoft Project "None" के रूप में दिखाता है। |
| [createTaskDefinition(int customFieldType, int fieldId, String alias)](#createTaskDefinition-int-int-java.lang.String-) | फ़ैक्टरी मेथड जो एक सरल विस्तारित गुण परिभाषा बनाता है, जिसे Microsoft Project "None" के रूप में दिखाता है। |
| [createTaskDefinition(int fieldId, String alias)](#createTaskDefinition-int-java.lang.String-) | फ़ैक्टरी मेथड जो एक सरल विस्तारित गुण परिभाषा बनाता है, जिसे Microsoft Project "None" के रूप में दिखाता है। |
| [equals(Object obj)](#equals-java.lang.Object-) | एक फ़्लैग लौटाता है जो दर्शाता है कि यह उदाहरण निर्दिष्ट वस्तु के बराबर है या नहीं। |
| [getAlias()](#getAlias--) | कस्टम फ़ील्ड का उपनाम प्राप्त करता है। |
| [getAppendNewValues()](#getAppendNewValues--) | एक मान प्राप्त करता है जो यह दर्शाता है कि प्रोजेक्ट में जोड़े गए नए मान स्वचालित रूप से सूची में जोड़ दिए जाते हैं या नहीं। |
| [getAutoRollDown()](#getAutoRollDown--) | एक मान प्राप्त करता है जो यह दर्शाता है कि असाइनमेंट्स में स्वचालित रोल डाउन सक्षम है या नहीं। |
| [getCalculationType()](#getCalculationType--) | कस्टम एट्रिब्यूट के मान की गणना प्रकार प्राप्त करता है। |
| [getCfType()](#getCfType--) | कस्टम फ़ील्ड का प्रकार प्राप्त करता है। |
| [getDefault()](#getDefault--) | सूची में डिफ़ॉल्ट मान प्राप्त करता है। |
| [getDefaultGuid()](#getDefaultGuid--) | डिफ़ॉल्ट लुकअप टेबल एंट्री का Guid प्राप्त करता है। |
| [getElementType()](#getElementType--) | जाँचता है कि विस्तारित एट्रिब्यूट कार्य, संसाधन या असाइनमेंट से जुड़ा है। |
| [getFieldId()](#getFieldId--) | कस्टम फ़ील्ड के प्रोजेक्ट आईडी के अनुरूप प्राप्त करता है। |
| [getFieldName()](#getFieldName--) | कस्टम फ़ील्ड का नाम प्राप्त करता है। |
| [getFormula()](#getFormula--) | Microsoft Project द्वारा कस्टम टास्क फ़ील्ड को भरने के लिए उपयोग किए जाने वाले फ़ॉर्मूला को प्राप्त करता है। |
| [getGraphicalIndicator()](#getGraphicalIndicator--) | विस्तारित एट्रिब्यूट से जुड़ी ग्राफ़िकल इंडिकेटर जानकारी प्राप्त करता है। |
| [getGuid()](#getGuid--) | कस्टम फ़ील्ड का Guid प्राप्त करता है। |
| [getLookupUid()](#getLookupUid--) | कस्टम फ़ील्ड से जुड़ी लुकअप टेबल का Guid प्राप्त करता है। |
| [getMaxMultiValues()](#getMaxMultiValues--) | पिक लिस्ट में आप जितने अधिकतम मान सेट कर सकते हैं, वह संख्या प्राप्त करता है। |
| [getParentProject()](#getParentProject--) | इस [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) इंस्टेंस के लिए पैरेंट प्रोजेक्ट प्राप्त करता है। |
| [getPhoneticsAlias()](#getPhoneticsAlias--) | कस्टम फ़ील्ड के उपनाम की ध्वन्यात्मक उच्चारण प्राप्त करता है। |
| [getRestrictValues()](#getRestrictValues--) | एक मान प्राप्त करता है जो यह दर्शाता है कि कस्टम फ़ील्ड मान `ValueList`([getValueList()](../../com.aspose.tasks/extendedattributedefinition\#getValueList--)/ [setValueList(List)](../../com.aspose.tasks/extendedattributedefinition\#setValueList-List-Value--)) में मौजूद मानों तक सीमित हैं या नहीं। |
| [getRollupType()](#getRollupType--) | रोलअप्स की गणना का तरीका प्राप्त करता है। |
| [getSecondaryGuid()](#getSecondaryGuid--) | विस्तारित एट्रिब्यूट का सेकेंडरी guid प्राप्त करता है। |
| [getSecondaryPid()](#getSecondaryPid--) | कस्टम फ़ील्ड का सेकेंडरी PID प्राप्त करता है। |
| [getSummaryRowsCalculationType()](#getSummaryRowsCalculationType--) | सारांश पंक्तियों के लिए कस्टम एट्रिब्यूट के मान की गणना प्रकार प्राप्त करता है। |
| [getUserDef()](#getUserDef--) | एक मान प्राप्त करता है जो यह दर्शाता है कि कस्टम फ़ील्ड उपयोगकर्ता द्वारा परिभाषित है या नहीं। |
| [getValueList()](#getValueList--) | List&lt;Value&gt; ValueList प्राप्त करता है। |
| [getValuelistSortOrder()](#getValuelistSortOrder--) | वैल्यू लिस्ट्स को सॉर्ट करने का तरीका प्राप्त करता है। |
| [hashCode()](#hashCode--) | इंस्टेंस के लिए हैश कोड लौटाता है [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) क्लास का। |
| [removeLookupValue(Value value)](#removeLookupValue-com.aspose.tasks.Value-) | आंतरिक लुकअप सूची से एक मान हटाता है। |
| [setAlias(String value)](#setAlias-java.lang.String-) | कस्टम फ़ील्ड का उपनाम सेट करता है। |
| [setAppendNewValues(boolean value)](#setAppendNewValues-boolean-) | एक मान सेट करता है जो दर्शाता है कि प्रोजेक्ट में जोड़े गए नए मान स्वचालित रूप से सूची में जोड़ें गए हैं या नहीं। |
| [setAutoRollDown(boolean value)](#setAutoRollDown-boolean-) | एक मान सेट करता है जो दर्शाता है कि असाइनमेंट्स में स्वचालित रोल डाउन सक्षम है या नहीं। |
| [setCalculationType(int value)](#setCalculationType-int-) | कस्टम एट्रिब्यूट के मान की गणना प्रकार सेट करता है। |
| [setDefault(String value)](#setDefault-java.lang.String-) | सूची में डिफ़ॉल्ट मान सेट करता है। |
| [setDefaultGuid(String value)](#setDefaultGuid-java.lang.String-) | डिफ़ॉल्ट लुकअप टेबल एंट्री का GUID सेट करता है। |
| [setElementType(int value)](#setElementType-int-) | सेट करता है कि विस्तारित एट्रिब्यूट टास्क, रिसोर्स या असाइनमेंट से जुड़ा है। |
| [setFieldId(String value)](#setFieldId-java.lang.String-) | सेट करता है जो कस्टम फ़ील्ड के प्रोजेक्ट आईडी से मेल खाता है। |
| [setFormula(String value)](#setFormula-java.lang.String-) | फ़ॉर्मूला सेट करता है जो Microsoft Project कस्टम टास्क फ़ील्ड को भरने के लिए उपयोग करता है। |
| [setGraphicalIndicator(GraphicalIndicatorsInfo value)](#setGraphicalIndicator-com.aspose.tasks.GraphicalIndicatorsInfo-) | विस्तारित एट्रिब्यूट से जुड़े ग्राफ़िकल इंडिकेटर जानकारी सेट करता है। |
| [setGuid(String value)](#setGuid-java.lang.String-) | कस्टम फ़ील्ड का GUID सेट करता है। |
| [setMaxMultiValues(int value)](#setMaxMultiValues-int-) | पिक सूची में आप जितने अधिकतम मान सेट कर सकते हैं, उसकी संख्या सेट करता है। |
| [setPhoneticsAlias(String value)](#setPhoneticsAlias-java.lang.String-) | कस्टम फ़ील्ड के उपनाम की ध्वन्यात्मक उच्चारण सेट करता है। |
| [setRestrictValues(boolean value)](#setRestrictValues-boolean-) | एक मान सेट करता है जो दर्शाता है कि कस्टम फ़ील्ड मान `ValueList`([getValueList()](../../com.aspose.tasks/extendedattributedefinition\#getValueList--)/ [setValueList(List)](../../com.aspose.tasks/extendedattributedefinition\#setValueList-List-Value--)) में मानों तक सीमित हैं या नहीं। |
| [setRollupType(int value)](#setRollupType-int-) | रोलअप्स की गणना का तरीका सेट करता है। |
| [setSecondaryGuid(String value)](#setSecondaryGuid-java.lang.String-) | विस्तारित एट्रिब्यूट का द्वितीयक GUID सेट करता है। |
| [setSecondaryPid(String value)](#setSecondaryPid-java.lang.String-) | कस्टम फ़ील्ड का द्वितीयक PID सेट करता है। |
| [setSummaryRowsCalculationType(int value)](#setSummaryRowsCalculationType-int-) | सारांश पंक्तियों के लिए कस्टम एट्रिब्यूट के मान की गणना प्रकार सेट करता है। |
| [setUserDef(boolean value)](#setUserDef-boolean-) | एक मान सेट करता है जो दर्शाता है कि कस्टम फ़ील्ड उपयोगकर्ता द्वारा परिभाषित है या नहीं। |
| [setValuelistSortOrder(int value)](#setValuelistSortOrder-int-) | मान सूचियों के क्रमबद्ध करने का तरीका सेट करता है। |
### addLookupValue(Value value) {#addLookupValue-com.aspose.tasks.Value-}
```
public final void addLookupValue(Value value)
```


आंतरिक लुकअप सूची में एक मान जोड़ता है। यह `ValueList`([getValueList()](../../com.aspose.tasks/extendedattributedefinition\#getValueList--)/ [setValueList(List)](../../com.aspose.tasks/extendedattributedefinition\#setValueList-List-Value--)) के साथ हेरफेर करने का पसंदीदा तरीका है।

--------------------

&gt; ```
&gt; इस कोड का उपयोग करके लुकअप सूची में नया मान जोड़ें:
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
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | lookupValue | [Value](../../com.aspose.tasks/value) | निर्दिष्ट [Value](../../com.aspose.tasks/value) आइटम। |

--------------------

`lookupValue` को पहले [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) में [addLookupValue(Value)](../../com.aspose.tasks/extendedattributedefinition\#addLookupValue-Value-) विधि का उपयोग करके जोड़ा जाना चाहिए। |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class linked with specified [Value](../../com.aspose.tasks/value) item.
### createExtendedAttribute(String textValue) {#createExtendedAttribute-java.lang.String-}
```
public final ExtendedAttribute createExtendedAttribute(String textValue)
```


इस वस्तु के फ़ील्ड ID मान के बराबर फ़ील्ड ID और निर्दिष्ट पाठ मान के साथ एक नया विस्तारित गुण बनाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| textValue | java.lang.String | निर्दिष्ट टेक्स्ट मान। |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class with the fieldID which equals to this object's fieldID value.
### createExtendedAttribute(BigDecimal numericValue) {#createExtendedAttribute-java.math.BigDecimal-}
```
public final ExtendedAttribute createExtendedAttribute(BigDecimal numericValue)
```


इस वस्तु के फ़ील्ड ID मान के बराबर फ़ील्ड ID और निर्दिष्ट संख्यात्मक मान के साथ एक नया विस्तारित गुण बनाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| numericValue | java.math.BigDecimal | निर्दिष्ट संख्यात्मक मान। |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class with the fieldID which equals to this object's fieldID value.
### createExtendedAttribute(Date dateTimeValue) {#createExtendedAttribute-java.util.Date-}
```
public final ExtendedAttribute createExtendedAttribute(Date dateTimeValue)
```


इस वस्तु के फ़ील्ड ID मान के बराबर फ़ील्ड ID और निर्दिष्ट तिथि मान के साथ एक नया विस्तारित गुण बनाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| dateTimeValue | java.util.Date | निर्दिष्ट दिनांक‑समय मान। |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class with the fieldID which equals to this object's fieldID value.
### createLookupResourceDefinition(int customFieldType, int fieldId, String alias) {#createLookupResourceDefinition-int-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createLookupResourceDefinition(int customFieldType, int fieldId, String alias)
```


एक फ़ैक्टरी मेथड जो लुकअप के साथ विस्तारित एट्रिब्यूट परिभाषा बनाता है। इसमें `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) का मान [CalculationType.Lookup](../../com.aspose.tasks/calculationtype\#Lookup) के बराबर है और यह केवल संसाधनों में उपयोग किया जा सकता है। इस मेथड को कॉल करते समय आपको `customFieldType`, `fieldId` और `alias` निर्दिष्ट करना आवश्यक है।

--------------------

&gt; ```
&gt; लुकअप के साथ एक संसाधन के लिए कस्टम फ़ील्ड परिभाषा बनाने और फिर इसे टेक्स्ट मानों से भरने के लिए इस उदाहरण का उपयोग करें:
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
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| fieldId | int | निर्दिष्ट [ExtendedAttributeResource](../../com.aspose.tasks/extendedattributeresource) फ़ील्ड आईडी। |
| alias | java.lang.String | निर्दिष्ट String उपनाम। |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `fieldId` and `alias`.
### createLookupTaskDefinition(int customFieldType, int fieldId, String alias) {#createLookupTaskDefinition-int-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createLookupTaskDefinition(int customFieldType, int fieldId, String alias)
```


फ़ैक्टरी मेथड जो लुकअप के साथ विस्तारित एट्रिब्यूट परिभाषा बनाता है। इसमें `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) बराबर है [CalculationType.Lookup](../../com.aspose.tasks/calculationtype\#Lookup) और केवल टास्क्स में उपयोग किया जा सकता है। आपको इस मेथड को कॉल करते समय `customFieldType`, `fieldId` और `alias` निर्दिष्ट करना आवश्यक है।

--------------------

&gt; ```
&gt; इस उदाहरण का उपयोग करके लुकअप के साथ टास्क के लिए एक कस्टम फ़ील्ड परिभाषा बनाएं और फिर इसे टेक्स्ट मानों से भरें:
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
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| fieldId | int | निर्दिष्ट [ExtendedAttributeTask](../../com.aspose.tasks/extendedattributetask) फ़ील्ड आईडी। |
| alias | java.lang.String | निर्दिष्ट String उपनाम। |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `fieldId` and `alias`.
### createResourceDefinition(int customFieldType, int fieldId, String alias) {#createResourceDefinition-int-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createResourceDefinition(int customFieldType, int fieldId, String alias)
```


फ़ैक्टरी मेथड जो एक सरल विस्तारित एट्रिब्यूट परिभाषा बनाता है, जिसे Microsoft Project \"None\" के रूप में दिखाता है। इसमें `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) बराबर है [CalculationType.None](../../com.aspose.tasks/calculationtype\#None) और यह केवल रिसोर्स में उपयोग किया जा सकता है। आपको इस मेथड को कॉल करते समय `customFieldType`, `fieldId` और `alias` निर्दिष्ट करने की आवश्यकता है।

--------------------

&gt; ```
&gt; इस उदाहरण का उपयोग करके एक कस्टम टेक्स्ट फ़ील्ड परिभाषा बनाएं:
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
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| fieldId | int | निर्दिष्ट [ExtendedAttributeResource](../../com.aspose.tasks/extendedattributeresource) फ़ील्ड आईडी। |
| alias | java.lang.String | निर्दिष्ट String उपनाम। |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `fieldId` and `alias`.
### createTaskDefinition(int customFieldType, int fieldId, String alias) {#createTaskDefinition-int-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createTaskDefinition(int customFieldType, int fieldId, String alias)
```


फ़ैक्टरी मेथड जो एक सरल विस्तारित एट्रिब्यूट परिभाषा बनाता है, जिसे Microsoft Project \"None\" के रूप में दिखाता है। इसमें `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) बराबर है [CalculationType.None](../../com.aspose.tasks/calculationtype\#None) और यह केवल टास्क्स में उपयोग किया जा सकता है। आपको इस मेथड को कॉल करते समय `customFieldType`, `fieldId` और `alias` निर्दिष्ट करने की आवश्यकता है।

--------------------

&gt; ```
&gt; इस उदाहरण का उपयोग करके एक कस्टम टेक्स्ट फ़ील्ड परिभाषा बनाएं:
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
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| fieldId | int | निर्दिष्ट [ExtendedAttributeTask](../../com.aspose.tasks/extendedattributetask) फ़ील्ड आईडी। |
| alias | java.lang.String | निर्दिष्ट String उपनाम। |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `fieldId` and `alias`.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


एक फ़्लैग लौटाता है जो दर्शाता है कि यह उदाहरण निर्दिष्ट वस्तु के बराबर है या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| obj | java.lang.Object | इस उदाहरण से तुलना करने के लिए निर्दिष्ट ऑब्जेक्ट। |

**Returns:**
boolean - एक फ़्लैग जो यह दर्शाता है कि यह उदाहरण निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं।
### getAlias() {#getAlias--}
```
public final String getAlias()
```


कस्टम फ़ील्ड का उपनाम प्राप्त करता है।

**Returns:**
java.lang.String - एक कस्टम फ़ील्ड का उपनाम।
### getAppendNewValues() {#getAppendNewValues--}
```
public final boolean getAppendNewValues()
```


एक मान प्राप्त करता है जो यह दर्शाता है कि प्रोजेक्ट में जोड़े गए नए मान स्वचालित रूप से सूची में जोड़ दिए जाते हैं या नहीं।

--------------------

वर्तमान में MSP 2003/2007 Xml और MSP 2003 mpp फ़ॉर्मैट्स के लिए समर्थित है।

**Returns:**
boolean - एक मान जो यह दर्शाता है कि प्रोजेक्ट में जोड़े गए नए मान स्वचालित रूप से सूची में जोड़े जाते हैं या नहीं।
### getAutoRollDown() {#getAutoRollDown--}
```
public final boolean getAutoRollDown()
```


एक मान प्राप्त करता है जो यह दर्शाता है कि असाइनमेंट्स में स्वचालित रोल डाउन सक्षम है या नहीं।

**Returns:**
boolean - एक मान जो यह दर्शाता है कि असाइनमेंट्स में स्वचालित रोल डाउन सक्षम है या नहीं।
### getCalculationType() {#getCalculationType--}
```
public final int getCalculationType()
```


कस्टम एट्रिब्यूट के मान की गणना प्रकार प्राप्त करता है।

**Returns:**
int - कस्टम एट्रिब्यूट मान की गणना का प्रकार।
### getCfType() {#getCfType--}
```
public final int getCfType()
```


कस्टम फ़ील्ड का प्रकार प्राप्त करता है।

**Returns:**
int - एक कस्टम फ़ील्ड का प्रकार।
### getDefault() {#getDefault--}
```
public final String getDefault()
```


सूची में डिफ़ॉल्ट मान प्राप्त करता है।

--------------------

वर्तमान में MSP 2003/2007 Xml और MSP 2003 mpp फ़ॉर्मैट्स के लिए समर्थित है।

**Returns:**
java.lang.String - सूची में डिफ़ॉल्ट मान.
### getDefaultGuid() {#getDefaultGuid--}
```
public final String getDefaultGuid()
```


डिफ़ॉल्ट लुकअप टेबल एंट्री का Guid प्राप्त करता है।

**Returns:**
java.lang.String - डिफ़ॉल्ट लुकअप टेबल एंट्री का Guid.
### getElementType() {#getElementType--}
```
public final int getElementType()
```


जाँचता है कि विस्तारित एट्रिब्यूट कार्य, संसाधन या असाइनमेंट से जुड़ा है।

**Returns:**
int - विस्तारित एट्रिब्यूट एक टास्क, एक रिसोर्स या एक असाइनमेंट से जुड़ा है.
### getFieldId() {#getFieldId--}
```
public final String getFieldId()
```


Gets कस्टम फ़ील्ड के प्रोजेक्ट आईडी से संबंधित है। एक स्थिरांक की स्ट्रिंग प्रतिनिधित्व का उपयोग करें [ExtendedAttributeTask](../../com.aspose.tasks/extendedattributetask) क्लास से `FieldId`([getFieldId()](../../com.aspose.tasks/extendedattributedefinition\#getFieldId--)/ [setFieldId(String)](../../com.aspose.tasks/extendedattributedefinition\#setFieldId-String-)) प्रॉपर्टी को निर्दिष्ट करने के लिए।

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

फ़ील्डId सेट करने का पसंदीदा तरीका `FieldId`([getFieldId()](../../com.aspose/tasks/extendedattributedefinition\#getFieldId--)/ [setFieldId(String)](../../com.aspose/tasks/extendedattributedefinition\#setFieldId-String-)) प्रॉपर्टी है कि आप [ExtendedAttributeDefinition](../../com.aspose/tasks/extendedattributedefinition) को समर्पित फ़ैक्टरी मेथड्स में से किसी एक का उपयोग करके बनाएँ, जैसे कि [createTaskDefinition(int, String)](../../com.aspose/tasks/extendedattributedefinition\#createTaskDefinition-int--String-) या [createLookupTaskDefinition(int, int, String)](../../com.aspose/tasks/extendedattributedefinition\#createLookupTaskDefinition-int--int--String-).

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | कस्टम फ़ील्ड के प्रोजेक्ट आईडी के अनुरूप है। |

### setFormula(String value) {#setFormula-java.lang.String-}
```
public final void setFormula(String value)
```


फ़ॉर्मूला सेट करता है जो Microsoft Project कस्टम टास्क फ़ील्ड को भरने के लिए उपयोग करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | Microsoft Project द्वारा कस्टम टास्क फ़ील्ड को भरने के लिए उपयोग किया जाने वाला फ़ॉर्मूला। |

### setGraphicalIndicator(GraphicalIndicatorsInfo value) {#setGraphicalIndicator-com.aspose.tasks.GraphicalIndicatorsInfo-}
```
public final void setGraphicalIndicator(GraphicalIndicatorsInfo value)
```


विस्तारित एट्रिब्यूट से जुड़ी ग्राफ़िकल इंडिकेटर जानकारी सेट करता है। MPP फ़ॉर्मेट के लिए लागू।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [GraphicalIndicatorsInfo](../../com.aspose.tasks/graphicalindicatorsinfo) | विस्तारित एट्रिब्यूट से जुड़ी ग्राफ़िकल इंडिकेटर जानकारी। |

### setGuid(String value) {#setGuid-java.lang.String-}
```
public final void setGuid(String value)
```


कस्टम फ़ील्ड का GUID सेट करता है।

--------------------

वर्तमान में केवल XML फ़ॉर्मेट के लिए समर्थित है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | कस्टम फ़ील्ड का GUID। |

### setMaxMultiValues(int value) {#setMaxMultiValues-int-}
```
public final void setMaxMultiValues(int value)
```


पिक सूची में आप जितने अधिकतम मान सेट कर सकते हैं, उसकी संख्या सेट करता है।

--------------------

वर्तमान में केवल XML फ़ॉर्मेट के लिए समर्थित है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | पिक लिस्ट में आप सेट कर सकते अधिकतम मानों की संख्या। |

### setPhoneticsAlias(String value) {#setPhoneticsAlias-java.lang.String-}
```
public final void setPhoneticsAlias(String value)
```


कस्टम फ़ील्ड के उपनाम की ध्वन्यात्मक उच्चारण सेट करता है।

--------------------

वर्तमान में केवल XML फ़ॉर्मेट के लिए समर्थित है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | कस्टम फ़ील्ड के उपनाम की ध्वन्यात्मक उच्चारण। |

### setRestrictValues(boolean value) {#setRestrictValues-boolean-}
```
public final void setRestrictValues(boolean value)
```


एक मान सेट करता है जो दर्शाता है कि कस्टम फ़ील्ड मान `ValueList`([getValueList()](../../com.aspose.tasks/extendedattributedefinition\#getValueList--)/ [setValueList(List)](../../com.aspose.tasks/extendedattributedefinition\#setValueList-List-Value--)) में मानों तक सीमित हैं या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | एक मान जो दर्शाता है कि कस्टम फ़ील्ड मानों को ... में मानों तक सीमित किया गया है। |

### setRollupType(int value) {#setRollupType-int-}
```
public final void setRollupType(int value)
```


रोलअप्स की गणना का तरीका सेट करता है।

--------------------

लेखन वर्तमान में केवल XML फ़ॉर्मेट के लिए समर्थित है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | रोलअप्स की गणना करने का तरीका। |

### setSecondaryGuid(String value) {#setSecondaryGuid-java.lang.String-}
```
public final void setSecondaryGuid(String value)
```


विस्तारित एट्रिब्यूट का द्वितीयक GUID सेट करता है।

--------------------

यह MS Project 2010 प्रॉपर्टी के लिए नया है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | विस्तारित एट्रिब्यूट का द्वितीयक GUID। |

### setSecondaryPid(String value) {#setSecondaryPid-java.lang.String-}
```
public final void setSecondaryPid(String value)
```


कस्टम फ़ील्ड का द्वितीयक PID सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | कस्टम फ़ील्ड का द्वितीयक PID। |

### setSummaryRowsCalculationType(int value) {#setSummaryRowsCalculationType-int-}
```
public final void setSummaryRowsCalculationType(int value)
```


सारांश पंक्तियों के लिए कस्टम एट्रिब्यूट के मान की गणना प्रकार सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | सारांश पंक्तियों के लिए कस्टम एट्रिब्यूट मान की गणना का प्रकार। |

### setUserDef(boolean value) {#setUserDef-boolean-}
```
public final void setUserDef(boolean value)
```


एक मान सेट करता है जो दर्शाता है कि कस्टम फ़ील्ड उपयोगकर्ता द्वारा परिभाषित है या नहीं।

--------------------

वर्तमान में केवल XML फ़ॉर्मेट के लिए समर्थित है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | एक मान जो दर्शाता है कि कस्टम फ़ील्ड उपयोगकर्ता द्वारा परिभाषित है या नहीं। |

### setValuelistSortOrder(int value) {#setValuelistSortOrder-int-}
```
public final void setValuelistSortOrder(int value)
```


मान सूची को सॉर्ट करने का तरीका सेट करता है। मान हैं: 0=अवरोही, 1=आरोही।

--------------------

वर्तमान में MSP 2003/2007 Xml और MSP 2003 mpp फ़ॉर्मैट्स के लिए समर्थित है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | मूल्य सूचियों को क्रमबद्ध करने का तरीका। |

