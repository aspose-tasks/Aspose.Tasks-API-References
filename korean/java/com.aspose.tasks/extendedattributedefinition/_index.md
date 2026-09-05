---
title: "ExtendedAttributeDefinition"
second_title: "Aspose.Tasks for Java API Reference"
description: "프로젝트와 연관된 확장 속성 정의를 나타냅니다."
type: docs
weight: 83
url: /ko/java/com.aspose.tasks/extendedattributedefinition/
---

**Inheritance:**
java.lang.Object
```
public class ExtendedAttributeDefinition
```

프로젝트와 연관된 확장 속성 정의를 나타냅니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [addLookupValue(Value value)](#addLookupValue-com.aspose.tasks.Value-) | 내부 조회 목록에 값을 추가합니다. |
| [compareTo(ExtendedAttributeDefinition o)](#compareTo-com.aspose.tasks.ExtendedAttributeDefinition-) | 이 객체를 @\{code ExtendedAttributeDefinition\} 클래스의 다른 인스턴스와 비교합니다. |
| [createExtendedAttribute()](#createExtendedAttribute--) | 이 객체의 필드 ID 값과 동일한 필드 ID를 가진 새 확장 속성을 생성합니다. |
| [createExtendedAttribute(boolean flagValue)](#createExtendedAttribute-boolean-) | 이 객체의 필드 ID 값과 지정된 플래그 값을 가진 새 확장 속성을 생성합니다. |
| [createExtendedAttribute(Duration durationValue)](#createExtendedAttribute-com.aspose.tasks.Duration-) | 이 객체의 필드 ID 값과 지정된 기간 값을 가진 새 확장 속성을 생성합니다. |
| [createExtendedAttribute(Value lookupValue)](#createExtendedAttribute-com.aspose.tasks.Value-) | 지정된 [Value](../../com.aspose.tasks/value) 항목과 연결된 새 확장 속성을 생성합니다. |
| [createExtendedAttribute(String textValue)](#createExtendedAttribute-java.lang.String-) | 이 객체의 필드 ID 값과 지정된 텍스트 값을 가진 새 확장 속성을 생성합니다. |
| [createExtendedAttribute(BigDecimal numericValue)](#createExtendedAttribute-java.math.BigDecimal-) | 이 객체의 필드 ID 값과 지정된 숫자 값을 가진 새 확장 속성을 생성합니다. |
| [createExtendedAttribute(Date dateTimeValue)](#createExtendedAttribute-java.util.Date-) | 이 객체의 필드 ID 값과 지정된 날짜 값을 가진 새 확장 속성을 생성합니다. |
| [createLookupResourceDefinition(int customFieldType, int fieldId, String alias)](#createLookupResourceDefinition-int-int-java.lang.String-) | 조회가 포함된 확장 속성 정의를 생성하는 팩터리 메서드입니다. |
| [createLookupResourceDefinition(int fieldId, String alias)](#createLookupResourceDefinition-int-java.lang.String-) | 조회가 포함된 확장 속성 정의를 생성하는 팩터리 메서드입니다. |
| [createLookupTaskDefinition(int customFieldType, int fieldId, String alias)](#createLookupTaskDefinition-int-int-java.lang.String-) | 조회가 포함된 확장 속성 정의를 생성하는 팩터리 메서드입니다. |
| [createLookupTaskDefinition(int fieldId, String alias)](#createLookupTaskDefinition-int-java.lang.String-) | 조회가 포함된 확장 속성 정의를 생성하는 팩터리 메서드입니다. |
| [createResourceDefinition(int customFieldType, int fieldId, String alias)](#createResourceDefinition-int-int-java.lang.String-) | Microsoft Project에서 "None"으로 표시되는 간단한 확장 속성 정의를 생성하는 팩터리 메서드입니다. |
| [createResourceDefinition(int fieldId, String alias)](#createResourceDefinition-int-java.lang.String-) | Microsoft Project에서 "None"으로 표시되는 간단한 확장 속성 정의를 생성하는 팩터리 메서드입니다. |
| [createTaskDefinition(int customFieldType, int fieldId, String alias)](#createTaskDefinition-int-int-java.lang.String-) | Microsoft Project에서 "None"으로 표시되는 간단한 확장 속성 정의를 생성하는 팩터리 메서드입니다. |
| [createTaskDefinition(int fieldId, String alias)](#createTaskDefinition-int-java.lang.String-) | Microsoft Project에서 "None"으로 표시되는 간단한 확장 속성 정의를 생성하는 팩터리 메서드입니다. |
| [equals(Object obj)](#equals-java.lang.Object-) | 이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 플래그를 반환합니다. |
| [getAlias()](#getAlias--) | 사용자 정의 필드의 별칭을 가져옵니다. |
| [getAppendNewValues()](#getAppendNewValues--) | 프로젝트에 추가된 새 값이 자동으로 목록에 추가되는지 여부를 나타내는 값을 가져옵니다. |
| [getAutoRollDown()](#getAutoRollDown--) | 할당에 대한 자동 롤다운이 활성화되어 있는지 여부를 나타내는 값을 가져옵니다. |
| [getCalculationType()](#getCalculationType--) | 사용자 정의 속성 값의 계산 유형을 가져옵니다. |
| [getCfType()](#getCfType--) | 사용자 정의 필드의 유형을 가져옵니다. |
| [getDefault()](#getDefault--) | 목록의 기본값을 가져옵니다. |
| [getDefaultGuid()](#getDefaultGuid--) | 기본 조회 테이블 항목의 Guid를 가져옵니다. |
| [getElementType()](#getElementType--) | 확장 속성이 작업, 리소스 또는 할당과 연결되는지를 가져옵니다. |
| [getFieldId()](#getFieldId--) | 사용자 정의 필드의 프로젝트 ID에 해당하는 값을 가져옵니다. |
| [getFieldName()](#getFieldName--) | 사용자 정의 필드의 이름을 가져옵니다. |
| [getFormula()](#getFormula--) | Microsoft Project가 사용자 정의 작업 필드를 채우는 데 사용하는 수식을 가져옵니다. |
| [getGraphicalIndicator()](#getGraphicalIndicator--) | 확장 속성과 연결된 그래픽 표시기 정보를 가져옵니다. |
| [getGuid()](#getGuid--) | 사용자 정의 필드의 Guid를 가져옵니다. |
| [getLookupUid()](#getLookupUid--) | 사용자 정의 필드와 연결된 조회 테이블의 Guid를 가져옵니다. |
| [getMaxMultiValues()](#getMaxMultiValues--) | 선택 목록에 설정할 수 있는 최대 값 개수를 가져옵니다. |
| [getParentProject()](#getParentProject--) | [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) 인스턴스에 대한 상위 프로젝트를 가져옵니다. |
| [getPhoneticsAlias()](#getPhoneticsAlias--) | 사용자 정의 필드 별칭의 음성 발음을 가져옵니다. |
| [getRestrictValues()](#getRestrictValues--) | 사용자 정의 필드 값이 `ValueList`([getValueList()](../../com.aspose.tasks/extendedattributedefinition\#getValueList--)/ [setValueList(List)](../../com.aspose.tasks/extendedattributedefinition\#setValueList-List-Value--))에 있는 값으로 제한되는지 여부를 나타내는 값을 가져옵니다. |
| [getRollupType()](#getRollupType--) | 롤업이 계산되는 방식을 가져옵니다. |
| [getSecondaryGuid()](#getSecondaryGuid--) | 확장 속성의 보조 guid를 가져옵니다. |
| [getSecondaryPid()](#getSecondaryPid--) | 사용자 정의 필드의 보조 PID를 가져옵니다. |
| [getSummaryRowsCalculationType()](#getSummaryRowsCalculationType--) | 요약 행에 대한 사용자 정의 속성 값의 계산 유형을 가져옵니다. |
| [getUserDef()](#getUserDef--) | 사용자 정의 필드가 사용자 정의인지 여부를 나타내는 값을 가져옵니다. |
| [getValueList()](#getValueList--) | List&lt;Value&gt; ValueList를 가져옵니다. |
| [getValuelistSortOrder()](#getValuelistSortOrder--) | 값 목록이 정렬되는 방식을 가져옵니다. |
| [hashCode()](#hashCode--) | 인스턴스인 [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) 클래스에 대한 해시 코드를 반환합니다. |
| [removeLookupValue(Value value)](#removeLookupValue-com.aspose.tasks.Value-) | 내부 조회 목록에서 값을 제거합니다. |
| [setAlias(String value)](#setAlias-java.lang.String-) | 사용자 정의 필드의 별칭을 설정합니다. |
| [setAppendNewValues(boolean value)](#setAppendNewValues-boolean-) | 프로젝트에 추가된 새 값이 자동으로 목록에 추가되는지 여부를 나타내는 값을 설정합니다. |
| [setAutoRollDown(boolean value)](#setAutoRollDown-boolean-) | 할당에 대한 자동 롤다운이 활성화되어 있는지 여부를 나타내는 값을 설정합니다. |
| [setCalculationType(int value)](#setCalculationType-int-) | 사용자 정의 속성 값의 계산 유형을 설정합니다. |
| [setDefault(String value)](#setDefault-java.lang.String-) | 목록의 기본값을 설정합니다. |
| [setDefaultGuid(String value)](#setDefaultGuid-java.lang.String-) | 기본 조회 테이블 항목의 Guid를 설정합니다. |
| [setElementType(int value)](#setElementType-int-) | 확장 속성이 작업, 리소스 또는 할당과 연결되도록 설정합니다. |
| [setFieldId(String value)](#setFieldId-java.lang.String-) | 사용자 정의 필드의 프로젝트 ID에 해당하도록 설정합니다. |
| [setFormula(String value)](#setFormula-java.lang.String-) | Microsoft Project가 사용자 정의 작업 필드를 채우는 데 사용하는 수식을 설정합니다. |
| [setGraphicalIndicator(GraphicalIndicatorsInfo value)](#setGraphicalIndicator-com.aspose.tasks.GraphicalIndicatorsInfo-) | 확장 속성과 연결된 그래픽 표시기 정보를 설정합니다. |
| [setGuid(String value)](#setGuid-java.lang.String-) | 사용자 정의 필드의 Guid를 설정합니다. |
| [setMaxMultiValues(int value)](#setMaxMultiValues-int-) | 픽 리스트에 설정할 수 있는 최대 값 개수를 설정합니다. |
| [setPhoneticsAlias(String value)](#setPhoneticsAlias-java.lang.String-) | 사용자 정의 필드 별칭의 음성 발음을 설정합니다. |
| [setRestrictValues(boolean value)](#setRestrictValues-boolean-) | 사용자 정의 필드 값이 `ValueList`([getValueList()](../../com.aspose.tasks/extendedattributedefinition\#getValueList--)/ [setValueList(List)](../../com.aspose.tasks/extendedattributedefinition\#setValueList-List-Value--))의 값으로 제한되는지 여부를 나타내는 값을 설정합니다. |
| [setRollupType(int value)](#setRollupType-int-) | 롤업이 계산되는 방식을 설정합니다. |
| [setSecondaryGuid(String value)](#setSecondaryGuid-java.lang.String-) | 확장 속성의 보조 guid를 설정합니다. |
| [setSecondaryPid(String value)](#setSecondaryPid-java.lang.String-) | 사용자 정의 필드의 보조 PID를 설정합니다. |
| [setSummaryRowsCalculationType(int value)](#setSummaryRowsCalculationType-int-) | 요약 행에 대한 사용자 정의 속성 값의 계산 유형을 설정합니다. |
| [setUserDef(boolean value)](#setUserDef-boolean-) | 사용자 정의 필드가 사용자 정의인지 여부를 나타내는 값을 설정합니다. |
| [setValuelistSortOrder(int value)](#setValuelistSortOrder-int-) | 값 목록이 정렬되는 방식을 설정합니다. |
### addLookupValue(Value value) {#addLookupValue-com.aspose.tasks.Value-}
```
public final void addLookupValue(Value value)
```


내부 조회 목록에 값을 추가합니다. 이는 `ValueList`([getValueList()](../../com.aspose.tasks/extendedattributedefinition\#getValueList--)/ [setValueList(List)](../../com.aspose.tasks/extendedattributedefinition\#setValueList-List-Value--))를 조작하는 권장 방법입니다.

--------------------

&gt; ```
&gt; 조회 목록에 새 값을 추가하기 위해 이 코드를 사용하십시오:
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
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | lookupValue | [Value](../../com.aspose.tasks/value) | 지정된 [Value](../../com.aspose.tasks/value) 항목. |

--------------------

`lookupValue`는 이전에 [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition)에 [addLookupValue(Value)](../../com.aspose.tasks/extendedattributedefinition\#addLookupValue-Value-) 메서드를 사용하여 추가되어야 합니다. |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class linked with specified [Value](../../com.aspose.tasks/value) item.
### createExtendedAttribute(String textValue) {#createExtendedAttribute-java.lang.String-}
```
public final ExtendedAttribute createExtendedAttribute(String textValue)
```


이 객체의 필드 ID 값과 지정된 텍스트 값을 가진 새 확장 속성을 생성합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| textValue | java.lang.String | 지정된 텍스트 값. |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class with the fieldID which equals to this object's fieldID value.
### createExtendedAttribute(BigDecimal numericValue) {#createExtendedAttribute-java.math.BigDecimal-}
```
public final ExtendedAttribute createExtendedAttribute(BigDecimal numericValue)
```


이 객체의 필드 ID 값과 지정된 숫자 값을 가진 새 확장 속성을 생성합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| numericValue | java.math.BigDecimal | 지정된 숫자 값. |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class with the fieldID which equals to this object's fieldID value.
### createExtendedAttribute(Date dateTimeValue) {#createExtendedAttribute-java.util.Date-}
```
public final ExtendedAttribute createExtendedAttribute(Date dateTimeValue)
```


이 객체의 필드 ID 값과 지정된 날짜 값을 가진 새 확장 속성을 생성합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| dateTimeValue | java.util.Date | 지정된 날짜시간 값. |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class with the fieldID which equals to this object's fieldID value.
### createLookupResourceDefinition(int customFieldType, int fieldId, String alias) {#createLookupResourceDefinition-int-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createLookupResourceDefinition(int customFieldType, int fieldId, String alias)
```


조회가 포함된 확장 속성 정의를 생성하는 팩터리 메서드입니다. 이 메서드는 `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-))이 [CalculationType.Lookup](../../com.aspose.tasks/calculationtype\#Lookup)와 같으며 리소스에서만 사용할 수 있습니다. 이 메서드를 호출할 때 `customFieldType`, `fieldId` 및 `alias`를 지정해야 합니다.

--------------------

&gt; ```
&gt; 조회가 있는 리소스를 위한 사용자 정의 필드 정의를 생성하고 텍스트 값으로 채우는 예제 사용:
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
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| fieldId | int | 지정된 [ExtendedAttributeResource](../../com.aspose.tasks/extendedattributeresource) 필드 ID. |
| alias | java.lang.String | 지정된 String 별칭. |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `fieldId` and `alias`.
### createLookupTaskDefinition(int customFieldType, int fieldId, String alias) {#createLookupTaskDefinition-int-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createLookupTaskDefinition(int customFieldType, int fieldId, String alias)
```


조회가 포함된 확장 속성 정의를 생성하는 팩터리 메서드입니다. `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) 은 [CalculationType.Lookup](../../com.aspose.tasks/calculationtype\#Lookup) 와 같으며 Tasks에서만 사용할 수 있습니다. 이 메서드를 호출할 때 `customFieldType`, `fieldId` 및 `alias` 를 지정해야 합니다.

--------------------

&gt; ```
&gt; 이 예제를 사용하여 조회가 있는 작업에 대한 사용자 정의 필드 정의를 만든 다음 텍스트 값으로 채웁니다:
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
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| fieldId | int | 지정된 [ExtendedAttributeTask](../../com.aspose.tasks/extendedattributetask) 필드 ID. |
| alias | java.lang.String | 지정된 String 별칭. |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `fieldId` and `alias`.
### createResourceDefinition(int customFieldType, int fieldId, String alias) {#createResourceDefinition-int-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createResourceDefinition(int customFieldType, int fieldId, String alias)
```


Microsoft Project에서 "None" 으로 표시되는 간단한 확장 속성 정의를 생성하는 팩터리 메서드입니다. `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) 은 [CalculationType.None](../../com.aspose.tasks/calculationtype\#None) 와 같으며 Resource에서만 사용할 수 있습니다. 이 메서드를 호출할 때 `customFieldType`, `fieldId` 및 `alias` 를 지정해야 합니다.

--------------------

&gt; ```
&gt; 이 예제를 사용하여 사용자 정의 텍스트 필드 정의를 만듭니다:
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
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| fieldId | int | 지정된 [ExtendedAttributeResource](../../com.aspose.tasks/extendedattributeresource) 필드 ID. |
| alias | java.lang.String | 지정된 String 별칭. |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `fieldId` and `alias`.
### createTaskDefinition(int customFieldType, int fieldId, String alias) {#createTaskDefinition-int-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createTaskDefinition(int customFieldType, int fieldId, String alias)
```


Microsoft Project에서 "None" 으로 표시되는 간단한 확장 속성 정의를 생성하는 팩터리 메서드입니다. `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) 은 [CalculationType.None](../../com.aspose.tasks/calculationtype\#None) 와 같으며 Tasks에서만 사용할 수 있습니다. 이 메서드를 호출할 때 `customFieldType`, `fieldId` 및 `alias` 를 지정해야 합니다.

--------------------

&gt; ```
&gt; 이 예제를 사용하여 사용자 정의 텍스트 필드 정의를 만듭니다:
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
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| fieldId | int | 지정된 [ExtendedAttributeTask](../../com.aspose.tasks/extendedattributetask) 필드 ID. |
| alias | java.lang.String | 지정된 String 별칭. |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `fieldId` and `alias`.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 플래그를 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| obj | java.lang.Object | 이 인스턴스와 비교할 지정된 객체. |

**Returns:**
boolean - 이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 플래그.
### getAlias() {#getAlias--}
```
public final String getAlias()
```


사용자 정의 필드의 별칭을 가져옵니다.

**Returns:**
java.lang.String - 사용자 정의 필드의 별칭.
### getAppendNewValues() {#getAppendNewValues--}
```
public final boolean getAppendNewValues()
```


프로젝트에 추가된 새 값이 자동으로 목록에 추가되는지 여부를 나타내는 값을 가져옵니다.

--------------------

현재 MSP 2003/2007 Xml 및 MSP 2003 mpp 형식을 지원합니다.

**Returns:**
boolean - 프로젝트에 추가된 새 값이 자동으로 목록에 추가되는지 여부를 나타내는 값.
### getAutoRollDown() {#getAutoRollDown--}
```
public final boolean getAutoRollDown()
```


할당에 대한 자동 롤다운이 활성화되어 있는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - 할당에 대한 자동 롤다운이 활성화되어 있는지 여부를 나타내는 값.
### getCalculationType() {#getCalculationType--}
```
public final int getCalculationType()
```


사용자 정의 속성 값의 계산 유형을 가져옵니다.

**Returns:**
int - 사용자 정의 속성 값의 계산 유형.
### getCfType() {#getCfType--}
```
public final int getCfType()
```


사용자 정의 필드의 유형을 가져옵니다.

**Returns:**
int - 사용자 정의 필드의 유형.
### getDefault() {#getDefault--}
```
public final String getDefault()
```


목록의 기본값을 가져옵니다.

--------------------

현재 MSP 2003/2007 Xml 및 MSP 2003 mpp 형식을 지원합니다.

**Returns:**
java.lang.String - 목록의 기본값.
### getDefaultGuid() {#getDefaultGuid--}
```
public final String getDefaultGuid()
```


기본 조회 테이블 항목의 Guid를 가져옵니다.

**Returns:**
java.lang.String - 기본 조회 테이블 항목의 Guid.
### getElementType() {#getElementType--}
```
public final int getElementType()
```


확장 속성이 작업, 리소스 또는 할당과 연결되는지를 가져옵니다.

**Returns:**
int - 확장 속성이 작업, 리소스 또는 할당과 연결됩니다.
### getFieldId() {#getFieldId--}
```
public final String getFieldId()
```


Gets는 사용자 정의 필드의 프로젝트 ID에 해당합니다. 문자열 표현을 사용하여 [ExtendedAttributeTask](../../com.aspose.tasks/extendedattributetask) 클래스의 상수 중 하나를 지정하고 `FieldId`([getFieldId()](../../com.aspose.tasks/extendedattributedefinition\#getFieldId--)/ [setFieldId(String)](../../com.aspose.tasks/extendedattributedefinition\#setFieldId-String-)) 속성을 설정합니다.

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

`FieldId`([getFieldId()](../../com.aspose/tasks/extendedattributedefinition\#getFieldId--)/ [setFieldId(String)](../../com.aspose/tasks/extendedattributedefinition\#setFieldId-String-)) 속성을 설정하는 권장 방법은 [ExtendedAttributeDefinition](../../com.aspose/tasks/extendedattributedefinition) 을(를) 전용 팩터리 메서드 중 하나인 [createTaskDefinition(int, String)](../../com.aspose/tasks/extendedattributedefinition\#createTaskDefinition-int--String-) 또는 [createLookupTaskDefinition(int, int, String)](../../com.aspose/tasks/extendedattributedefinition\#createLookupTaskDefinition-int--int--String-) 를 사용하여 만드는 것입니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | 맞춤 필드의 프로젝트 ID에 해당합니다. |

### setFormula(String value) {#setFormula-java.lang.String-}
```
public final void setFormula(String value)
```


Microsoft Project가 사용자 정의 작업 필드를 채우는 데 사용하는 수식을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | Microsoft Project가 사용자 지정 작업 필드를 채우는 데 사용하는 수식입니다. |

### setGraphicalIndicator(GraphicalIndicatorsInfo value) {#setGraphicalIndicator-com.aspose.tasks.GraphicalIndicatorsInfo-}
```
public final void setGraphicalIndicator(GraphicalIndicatorsInfo value)
```


확장 속성과 연결된 그래픽 표시기 정보를 설정합니다. MPP 형식에 적용됩니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [GraphicalIndicatorsInfo](../../com.aspose.tasks/graphicalindicatorsinfo) | 확장 속성과 연결된 그래픽 표시기 정보. |

### setGuid(String value) {#setGuid-java.lang.String-}
```
public final void setGuid(String value)
```


사용자 정의 필드의 Guid를 설정합니다.

--------------------

현재 XML 형식에만 지원됩니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | 맞춤 필드의 Guid입니다. |

### setMaxMultiValues(int value) {#setMaxMultiValues-int-}
```
public final void setMaxMultiValues(int value)
```


픽 리스트에 설정할 수 있는 최대 값 개수를 설정합니다.

--------------------

현재 XML 형식에만 지원됩니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 픽리스트에 설정할 수 있는 최대 값 개수입니다. |

### setPhoneticsAlias(String value) {#setPhoneticsAlias-java.lang.String-}
```
public final void setPhoneticsAlias(String value)
```


사용자 정의 필드 별칭의 음성 발음을 설정합니다.

--------------------

현재 XML 형식에만 지원됩니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | 맞춤 필드 별칭의 음성 발음입니다. |

### setRestrictValues(boolean value) {#setRestrictValues-boolean-}
```
public final void setRestrictValues(boolean value)
```


사용자 정의 필드 값이 `ValueList`([getValueList()](../../com.aspose.tasks/extendedattributedefinition\#getValueList--)/ [setValueList(List)](../../com.aspose.tasks/extendedattributedefinition\#setValueList-List-Value--))의 값으로 제한되는지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | 맞춤 필드 값이 해당 범위 내의 값으로 제한되는지 여부를 나타내는 값 |

### setRollupType(int value) {#setRollupType-int-}
```
public final void setRollupType(int value)
```


롤업이 계산되는 방식을 설정합니다.

--------------------

쓰기 작업은 현재 XML 형식에만 지원됩니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 롤업이 계산되는 방식입니다. |

### setSecondaryGuid(String value) {#setSecondaryGuid-java.lang.String-}
```
public final void setSecondaryGuid(String value)
```


확장 속성의 보조 guid를 설정합니다.

--------------------

이 속성은 MS Project 2010에서 새롭게 추가되었습니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | 확장 속성의 보조 Guid입니다. |

### setSecondaryPid(String value) {#setSecondaryPid-java.lang.String-}
```
public final void setSecondaryPid(String value)
```


사용자 정의 필드의 보조 PID를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | 맞춤 필드의 보조 PID입니다. |

### setSummaryRowsCalculationType(int value) {#setSummaryRowsCalculationType-int-}
```
public final void setSummaryRowsCalculationType(int value)
```


요약 행에 대한 사용자 정의 속성 값의 계산 유형을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 요약 행에 대한 맞춤 속성 값의 계산 유형입니다. |

### setUserDef(boolean value) {#setUserDef-boolean-}
```
public final void setUserDef(boolean value)
```


사용자 정의 필드가 사용자 정의인지 여부를 나타내는 값을 설정합니다.

--------------------

현재 XML 형식에만 지원됩니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | 맞춤 필드가 사용자 정의인지 여부를 나타내는 값입니다. |

### setValuelistSortOrder(int value) {#setValuelistSortOrder-int-}
```
public final void setValuelistSortOrder(int value)
```


값 목록이 정렬되는 방식을 설정합니다. 값은: 0=내림차순, 1=오름차순입니다.

--------------------

현재 MSP 2003/2007 Xml 및 MSP 2003 mpp 형식을 지원합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 값 목록이 정렬되는 방식. |

