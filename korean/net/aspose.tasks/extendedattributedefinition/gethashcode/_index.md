---
title: "ExtendedAttributeDefinition.GetHashCode"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ExtendedAttributeDefinition 메서드. ExtendedAttributeDefinition 클래스 인스턴스에 대한 해시 코드를 반환합니다."
type: docs
weight: 330
url: /ko/net/aspose.tasks/extendedattributedefinition/gethashcode/
---
## ExtendedAttributeDefinition.GetHashCode method

`[`ExtendedAttributeDefinition`](../) 클래스 인스턴스에 대한 해시 코드를 반환합니다.`

```csharp
public override int GetHashCode()
```

### 반환 값

이 객체에 대한 해시 코드.

## 예제

확장 속성 정의의 해시 코드를 가져오는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "MultipleOutlineValues2016.mpp");

var attributeDefinition1 = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Start3);
var attributeDefinition2 = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Duration2);

// 확장 속성 정의의 해시 코드는 필드 ID와 같습니다.
Console.WriteLine("Extended Attribute Field Id: {0} Hash Code: {1}", attributeDefinition1.FieldId, attributeDefinition1.GetHashCode());
Console.WriteLine("Extended Attribute Field Id: {0} Hash Code: {1}", attributeDefinition2.FieldId, attributeDefinition2.GetHashCode());
```

### 또 보기

* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


