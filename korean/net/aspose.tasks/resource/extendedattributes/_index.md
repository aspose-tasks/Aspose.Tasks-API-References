---
title: "Resource.ExtendedAttributes"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Resource 속성. 확장 속성의 값을 가져옵니다."
type: docs
weight: 320
url: /ko/net/aspose.tasks/resource/extendedattributes/
---
## Resource.ExtendedAttributes property

확장 속성의 값을 가져옵니다.

```csharp
public ExtendedAttributeCollection ExtendedAttributes { get; }
```

## 비고

두 개의 데이터가 필요합니다 - 고유 ID 또는 필드 ID 중 하나로 지정되는 확장 속성 테이블에 대한 포인터와, 값 자체로 지정되거나 값 목록에 대한 포인터로 지정되는 값.

## 예제

리소스 확장 속성을 추가하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "ResourceExtendedAttributes.mpp");

// 확장 속성 정의
var definition = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Number1);
if (definition == null)
{
    definition = ExtendedAttributeDefinition.CreateResourceDefinition(ExtendedAttributeResource.Number1, "Age");
    project.ExtendedAttributes.Add(definition);
}

// 확장 속성을 생성하고 값을 설정합니다
var attribute = definition.CreateExtendedAttribute();
attribute.NumericValue = 30.5345m;

// 새 리소스를 추가하고 해당 확장 속성을 추가합니다
var resource = project.Resources.Add("R1");
resource.ExtendedAttributes.Add(attribute);

project.Save(OutDir + "ResourceExtendedAttributes_out.mpp", SaveFileFormat.Mpp);
```

### 또 보기

* class [ExtendedAttributeCollection](../../extendedattributecollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


