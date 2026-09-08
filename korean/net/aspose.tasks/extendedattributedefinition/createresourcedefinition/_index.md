---
title: "ExtendedAttributeDefinition.CreateResourceDefinition"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ExtendedAttributeDefinition 메서드. Microsoft Project에서 \"None\"으로 표시되는 간단한 확장 속성 정의를 생성하는 팩터리 메서드입니다. CalculationType이 None이며 리소스에서만 사용할 수 있습니다. 이 메서드를 호출할 때 customFieldType, fieldId 및 alias를 지정해야 합니다."
type: docs
weight: 30
url: /ko/net/aspose.tasks/extendedattributedefinition/createresourcedefinition/
---
## CreateResourceDefinition(CustomFieldType, ExtendedAttributeResource, string) {#createresourcedefinition}

Microsoft Project에서 "None"으로 표시되는 간단한 확장 속성 정의를 생성하는 팩터리 메서드입니다. [`CalculationType`](../calculationtype/)이 None이며 리소스에서만 사용할 수 있습니다. 이 메서드를 호출할 때 *customFieldType*, *fieldId*, *alias*를 지정해야 합니다.

```csharp
public static ExtendedAttributeDefinition CreateResourceDefinition(CustomFieldType customFieldType, 
    ExtendedAttributeResource fieldId, string alias)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| customFieldType | CustomFieldType | 지정된 [`CustomFieldType`](../../customfieldtype/) 유형입니다. |
| fieldId | ExtendedAttributeResource | 지정된 [`ExtendedAttributeResource`](../../extendedattributeresource/) 필드 ID입니다. |
| 별칭 | 문자열 | 지정된 문자열 별칭입니다. |

### 반환 값

지정된 *customFieldType*, *fieldId*, *alias*를 사용하여 [`ExtendedAttributeDefinition`](../) 클래스의 인스턴스를 생성했습니다.

## 예제

이 예제를 사용하여 사용자 정의 텍스트 필드 정의를 생성합니다:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateResourceDefinition(CustomFieldType.Text, ExtendedAttributeResource.Text27, "My custom field");
project.ExtendedAttributes.Add(resourceTextAttr);
```

리소스 할당에 확장 속성을 추가하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// 새 작업 및 리소스를 추가합니다
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Rsc");
var assignment = project.ResourceAssignments.Add(task, resource);
{
    // "Resource Usage" 보기에서 볼 수 있는 사용자 정의 속성은 ExtendedAttributeDefinition.CreateResourceDefinition 메서드를 사용하여 생성할 수 있습니다.
    var resCostAttributeDefinition = ExtendedAttributeDefinition.CreateResourceDefinition(
        CustomFieldType.Cost,
        ExtendedAttributeResource.Cost5,
        "My cost");

    project.ExtendedAttributes.Add(resCostAttributeDefinition);

    var value = resCostAttributeDefinition.CreateExtendedAttribute();

    // 속성의 유형은 "Cost"이므로 "NumericValue" 속성을 사용해야 합니다.
    value.NumericValue = 1500;

    assignment.ExtendedAttributes.Add(value);
}

{
    // "Task Usage" 보기에서 볼 수 있는 사용자 정의 속성은 ExtendedAttributeDefinition.CreateTaskDefinition 메서드를 사용하여 생성할 수 있습니다.
    var taskCostAttributeDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(
        CustomFieldType.Cost,
        ExtendedAttributeTask.Cost5,
        "My cost for task");

    project.ExtendedAttributes.Add(taskCostAttributeDefinition);

    var value = taskCostAttributeDefinition.CreateExtendedAttribute();

    // 속성의 유형은 "Cost"이므로 "NumericValue" 속성을 사용해야 합니다.
    value.NumericValue = 2300;

    assignment.ExtendedAttributes.Add(value);
}

project.Save(OutDir + "AddExtendedAttributesToResourceAssignment_out.mpp", SaveFileFormat.Mpp);
```

### 또 보기

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateResourceDefinition(ExtendedAttributeResource, string) {#createresourcedefinition_1}

Microsoft Project에서 "None"으로 표시되는 간단한 확장 속성 정의를 생성하는 팩터리 메서드입니다. [`CalculationType`](../calculationtype/)이 None이며 리소스에서만 사용할 수 있습니다. 이 메서드를 호출할 때 *fieldId*와 *alias*를 지정해야 합니다. 필드 유형은 field id에서 추론됩니다.

```csharp
public static ExtendedAttributeDefinition CreateResourceDefinition(
    ExtendedAttributeResource fieldId, string alias)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| fieldId | ExtendedAttributeResource | 지정된 [`ExtendedAttributeResource`](../../extendedattributeresource/) 필드 ID입니다. |
| 별칭 | 문자열 | 지정된 문자열 별칭입니다. |

### 반환 값

지정된 *fieldId*와 *alias*를 사용하여 [`ExtendedAttributeDefinition`](../) 클래스의 인스턴스를 생성했습니다.

## 예제

이 예제를 사용하여 사용자 정의 텍스트 필드 정의를 생성합니다:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateResourceDefinition(ExtendedAttributeResource.Text27, "My custom field");
project.ExtendedAttributes.Add(resourceTextAttr);
```

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

* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


