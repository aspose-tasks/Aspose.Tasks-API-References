---
title: "OutlineCodeDefinition.Values"
second_title: "Aspose.Tasks for .NET API 참조"
description: "OutlineCodeDefinition 속성. OutlineValueCollection 객체를 가져옵니다. 이 개요 코드와 연관된 테이블의 값들"
type: docs
weight: 150
url: /ko/net/aspose.tasks/outlinecodedefinition/values/
---
## OutlineCodeDefinition.Values property

OutlineValueCollection 객체를 가져옵니다. 이 개요 코드와 연결된 테이블의 값들입니다.

```csharp
public OutlineValueCollection Values { get; }
```

## 예제

새 개요 코드를 만드는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "project.mpp");

// 개요 코드와 그 개요 마스크를 정의합니다.
var code1 = new OutlineCodeDefinition();
code1.Alias = "New task outline code1";
code1.FieldId = ((int)ExtendedAttributeTask.OutlineCode1).ToString();
code1.FieldName = "Outline Code1";
var mask = new OutlineMask();
mask.Separator = "+";
mask.Level = 1;
mask.Type = MaskType.Numbers;
code1.Masks.Add(mask);

// 개요 값 추가
var value = new OutlineValue();
value.Description = "Value description";
value.ValueId = 1;
value.Value = "123456";
value.Type = OutlineValueType.Number;
code1.Values.Add(value);

// 프로젝트에 개요 코드 추가
project.OutlineCodes.Add(code1);

// 개요 코드와 그 개요 마스크를 정의합니다.
var code2 = new OutlineCodeDefinition();
code2.Alias = "New rsc outline code2";
code2.FieldId = ((int)ExtendedAttributeResource.OutlineCode2).ToString();
code2.FieldName = "Outline Code2";
var mask2 = new OutlineMask();
mask2.Separator = "/";
mask2.Level = 1;
mask2.Type = MaskType.Numbers;
code2.Masks.Add(mask2);

// 개요 값 추가
var value2 = new OutlineValue();
value2.Description = "Value2 description";
value2.ValueId = 2;
value2.Value = "987654";
value2.Type = OutlineValueType.Number;
code2.Values.Add(value2);

// 프로젝트에 개요 코드 추가
project.OutlineCodes.Add(code2);

project.Save(OutDir + "Updated_project_out.mpp", SaveFileFormat.Mpp);
```

### 또 보기

* class [OutlineValueCollection](../../outlinevaluecollection/)
* class [OutlineCodeDefinition](../)
* namespace [Aspose.Tasks](../../outlinecodedefinition/)
* assembly [Aspose.Tasks](../../../)


