---
title: "ExtendedAttributeDefinition.CreateExtendedAttribute"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ExtendedAttributeDefinition 메서드. 이 객체의 필드 ID 값과 동일한 필드 ID를 가진 새로운 확장 속성을 생성합니다."
type: docs
weight: 310
url: /ko/net/aspose.tasks/extendedattributedefinition/createextendedattribute/
---
## CreateExtendedAttribute() {#createextendedattribute}

이 객체의 필드 ID 값과 같은 필드 ID를 사용하여 새 확장 속성을 생성합니다.

```csharp
public ExtendedAttribute CreateExtendedAttribute()
```

### 반환 값

생성된 인스턴스인 [`ExtendedAttribute`](../../extendedattribute/) 클래스를 반환하며, 해당 fieldID는 이 객체의 fieldID 값과 동일합니다.

## 예제

확장 속성을 생성하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var definition = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Text1);

// 프로젝트에 사용자 정의 필드가 없으면 생성합니다.
if (definition == null)
{
    definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, "My text field");
    project.ExtendedAttributes.Add(definition);
}

// 정의에서 확장 속성을 생성합니다.
var attribute = definition.CreateExtendedAttribute();
attribute.TextValue = "Text attribute value";

// 작업에 확장 속성을 추가합니다.
var task = project.RootTask.Children.Add("Task 1");
task.ExtendedAttributes.Add(attribute);

project.Save(OutDir + "CreateExtendedAttributes_out.mpp", SaveFileFormat.Mpp);
```

### 또 보기

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(string) {#createextendedattribute_6}

이 객체의 필드 ID 값과 같은 필드 ID와 지정된 텍스트 값을 사용하여 새 확장 속성을 생성합니다.

```csharp
public ExtendedAttribute CreateExtendedAttribute(string textValue)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| textValue | 문자열 | 지정된 텍스트 값입니다. |

### 반환 값

생성된 인스턴스인 [`ExtendedAttribute`](../../extendedattribute/) 클래스를 반환하며, 해당 fieldID는 이 객체의 fieldID 값과 동일합니다.

### 예외

| 예외 | 조건 |
| --- | --- |
| InvalidOperationException | 현재 [`CfType`](../cftype/)가 'Text'가 아닌 경우 |

## 예제

확장 속성 정의를 생성하고 구성 중에 속성의 문자열 값을 설정하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, "My Text");
project.ExtendedAttributes.Add(definition);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 22, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// 'Common Info'와 동일한 값을 가진 확장 속성을 생성합니다.
var extendedAttribute = definition.CreateExtendedAttribute("Common Info");

// 'Common Info' 값으로 초기화된 확장 속성을 추가합니다.
task.ExtendedAttributes.Add(extendedAttribute);
```

### 또 보기

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(decimal) {#createextendedattribute_5}

이 객체의 필드 ID 값과 같은 필드 ID와 지정된 숫자 값을 사용하여 새 확장 속성을 생성합니다.

```csharp
public ExtendedAttribute CreateExtendedAttribute(decimal numericValue)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| numericValue | Decimal | 지정된 숫자 값입니다. |

### 반환 값

생성된 인스턴스인 [`ExtendedAttribute`](../../extendedattribute/) 클래스를 반환하며, 해당 fieldID는 이 객체의 fieldID 값과 동일합니다.

### 예외

| 예외 | 조건 |
| --- | --- |
| InvalidOperationException | 현재 [`CfType`](../cftype/)가 'Number' 또는 'Cost'가 아닌 경우 |

## 예제

확장 속성 정의를 생성하고 구성 중에 속성의 소수점 값을 설정하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Cost1, "My Cost");
project.ExtendedAttributes.Add(definition);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 22, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// 값이 999m와 동일한 확장 속성을 생성합니다.
var extendedAttribute = definition.CreateExtendedAttribute(999m);

// 값 999m으로 초기화된 확장 속성을 추가합니다.
task.ExtendedAttributes.Add(extendedAttribute);
```

### 또 보기

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(DateTime) {#createextendedattribute_4}

이 객체의 필드 ID 값과 같은 필드 ID와 지정된 날짜 값을 사용하여 새 확장 속성을 생성합니다.

```csharp
public ExtendedAttribute CreateExtendedAttribute(DateTime dateTimeValue)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| dateTimeValue | DateTime | 지정된 날짜 및 시간 값입니다. |

### 반환 값

생성된 인스턴스인 [`ExtendedAttribute`](../../extendedattribute/) 클래스를 반환하며, 해당 fieldID는 이 객체의 fieldID 값과 동일합니다.

### 예외

| 예외 | 조건 |
| --- | --- |
| InvalidOperationException | 현재 [`CfType`](../cftype/)가 'Date', 'Start' 또는 'Finish'가 아닌 경우 |

## 예제

확장 속성 정의를 생성하고 속성을 구성하는 동안 날짜/시간 값을 설정하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var definitionWithDate = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Date1, "My Date");
project.ExtendedAttributes.Add(definitionWithDate);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 22, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// DateTime.Now와 같은 값을 가진 확장 속성을 생성합니다
var extendedAttribute = definitionWithDate.CreateExtendedAttribute(DateTime.Now);

// 확장 속성을 추가합니다
task.ExtendedAttributes.Add(extendedAttribute);
```

### 또 보기

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(Duration) {#createextendedattribute_1}

이 객체의 필드 ID 값과 같은 필드 ID와 지정된 기간 값을 사용하여 새 확장 속성을 생성합니다.

```csharp
public ExtendedAttribute CreateExtendedAttribute(Duration durationValue)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| durationValue | Duration | 지정된 기간 값입니다. |

### 반환 값

생성된 인스턴스인 [`ExtendedAttribute`](../../extendedattribute/) 클래스를 반환하며, 해당 fieldID는 이 객체의 fieldID 값과 동일합니다.

### 예외

| 예외 | 조건 |
| --- | --- |
| InvalidOperationException | 현재 [`CfType`](../cftype/)가 'Duration'이 아닌 경우 |

## 예제

확장 속성 정의를 생성하고 속성을 구성하는 동안 기간을 설정하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project2.mpp");
var task = project.RootTask.Children.Add("Test");
task.Set(Tsk.Start, new DateTime(2020, 4, 22, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Duration1, "Custom Duration");
project.ExtendedAttributes.Add(definition);

// 확장 속성 Duration1 = 2일
var extendedAttribute = definition.CreateExtendedAttribute(project.GetDuration(2, TimeUnitType.Day));

// 작업에 확장 속성을 추가합니다
task.ExtendedAttributes.Add(extendedAttribute);
```

### 또 보기

* class [ExtendedAttribute](../../extendedattribute/)
* struct [Duration](../../duration/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(bool) {#createextendedattribute_3}

이 객체의 필드 ID 값과 같은 필드 ID와 지정된 플래그 값을 사용하여 새 확장 속성을 생성합니다.

```csharp
public ExtendedAttribute CreateExtendedAttribute(bool flagValue)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| flagValue | Boolean | 지정된 플래그 값입니다. |

### 반환 값

생성된 인스턴스인 [`ExtendedAttribute`](../../extendedattribute/) 클래스를 반환하며, 해당 fieldID는 이 객체의 fieldID 값과 동일합니다.

### 예외

| 예외 | 조건 |
| --- | --- |
| InvalidOperationException | 현재 [`CfType`](../cftype/)가 'Flag'가 아닌 경우 |

## 예제

확장 속성 정의를 만들고 구성 중에 플래그 값을 설정하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var resource = project.Resources.Add("Resource 1");
resource.Set(Rsc.Type, ResourceType.Cost);

// 불리언 사용자 정의 필드에 대한 정의를 생성합니다
var definition = ExtendedAttributeDefinition.CreateResourceDefinition(ExtendedAttributeResource.Flag7, "My Custom Flag");

// 속성을 생성하고 초기 값을 'true' 로 설정합니다
var attribute = definition.CreateExtendedAttribute(true);
resource.ExtendedAttributes.Add(attribute);
```

### 또 보기

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(Value) {#createextendedattribute_2}

지정된 [`Value`](../../value/) 항목과 연결된 새 확장 속성을 생성합니다.

```csharp
public ExtendedAttribute CreateExtendedAttribute(Value lookupValue)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| lookupValue | Value | 지정된 [`Value`](../../value/) 항목입니다. |

### 반환 값

지정된 [`Value`](../../value/) 항목과 연결된 [`ExtendedAttribute`](../../extendedattribute/) 클래스의 생성된 인스턴스를 반환합니다.

## 비고

*lookupValue* should be previously added to the [`ExtendedAttributeDefinition`](../) using [`AddLookupValue`](../addlookupvalue/) method.

## 예제

특정 값을 사용하여 새 [`ExtendedAttribute`](../../extendedattribute/)을 생성하려면 이 코드를 사용하십시오:

```csharp
taskTextAttr.AddLookupValue(value1);
taskTextAttr.AddLookupValue(value2);
var extendedAttribute = taskTextAttr.CreateExtendedAttribute(value2);
```

확장 속성 정의를 생성하고 속성을 구성하는 동안 값을 설정하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// 위에서 선언한 조회 테이블을 기반으로 사용자 정의 필드 정의를 생성합니다.
var customFieldDefinition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(CustomFieldType.Number, ExtendedAttributeTask.Number10, "Status");

var value1 = new Value { Id = 1, Val = "25", Description = "Active" };
var value2 = new Value { Id = 2, Val = "12", Description = "Inactive" };
customFieldDefinition.AddLookupValue(value1);
customFieldDefinition.AddLookupValue(value2);
project.ExtendedAttributes.Add(customFieldDefinition);

var task = project.RootTask.Children.Add("Task");

// 값에 대한 확장 속성을 생성합니다
var extendedAttribute = customFieldDefinition.CreateExtendedAttribute(value2);

// 작업에 확장 속성을 추가합니다
task.ExtendedAttributes.Add(extendedAttribute);
```

### 또 보기

* class [ExtendedAttribute](../../extendedattribute/)
* class [Value](../../value/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


