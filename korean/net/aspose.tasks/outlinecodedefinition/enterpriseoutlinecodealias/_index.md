---
title: "OutlineCodeDefinition.EnterpriseOutlineCodeAlias"
second_title: "Aspose.Tasks for .NET API 참조"
description: "OutlineCodeDefinition 속성. 이 개요 코드 정의가 별칭인 다른 사용자 정의 필드에 대한 참조를 가져오거나 설정합니다"
type: docs
weight: 50
url: /ko/net/aspose.tasks/outlinecodedefinition/enterpriseoutlinecodealias/
---
## OutlineCodeDefinition.EnterpriseOutlineCodeAlias property

이 개요 코드 정의가 별칭인 다른 사용자 정의 필드에 대한 참조를 가져오거나 설정합니다.

```csharp
public int EnterpriseOutlineCodeAlias { get; set; }
```

## 예제

개요 코드 정의를 사용하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

// 새 개요 코드 정의를 생성합니다
var outline = new OutlineCodeDefinition();

// 개요 코드의 필드 번호를 설정합니다
outline.FieldId = ExtendedAttributeTask.OutlineCode7.ToString("D");

// 사용자 정의 개요 코드의 이름을 설정합니다
outline.FieldName = "Outline Code1";

// 개요 코드의 Guid를 설정합니다
outline.Guid = "e6afac06-0d86-4359-a96c-db705e3d2ca8";

// 이 개요 코드 필드에 지정된 값이 리프 값이어야 하는지 여부를 나타내는 값을 설정합니다
outline.LeafOnly = false;

// 사용자 정의 개요 코드의 별칭을 설정합니다
outline.Alias = "My Outline Code";

// 사용자 정의 개요 코드 별칭의 음성 발음을 설정합니다
outline.PhoneticAlias = "Outline Code";

// 새 코드는 모든 레벨을 가져야 하는지 여부를 나타내는 값을 설정합니다. 엔터프라이즈 코드에는 사용할 수 없습니다.
outline.AllLevelsRequired = true;

// 사용자 정의 개요 코드가 엔터프라이즈 사용자 정의 개요 코드인지 여부를 나타내는 값을 설정합니다
outline.Enterprise = false;

// 이 개요 코드 정의가 별칭인 다른 사용자 정의 필드에 대한 참조를 설정합니다
outline.EnterpriseOutlineCodeAlias = 0;

// 개요 마스크를 추가합니다
var mask = new OutlineMask();
mask.Type = MaskType.Characters;
outline.Masks.Add(mask);

// 지정된 값이 값 테이블에서 와야 하는지 여부를 나타내는 값을 설정합니다
outline.OnlyTableValuesAllowed = false;

// 사용자 정의 개요 코드를 사용할 수 있는지 여부를 나타내는 값을 설정합니다
// Microsoft Project의 리소스 대체 마법사에 의해
outline.ResourceSubstitutionEnabled = false;

// 이 개요 코드의 들여쓰기를 표시해야 하는지 여부를 나타내는 값을 설정합니다.
outline.ShowIndent = false;

project.OutlineCodes.Add(outline);

var value = new OutlineValue();
value.Value = "Text value 1";
value.ValueId = 1;
value.Type = OutlineValueType.Text;
value.Description = "Text value descr 1";
outline.Values.Add(value);

// ...
```

### 또 보기

* class [OutlineCodeDefinition](../)
* namespace [Aspose.Tasks](../../outlinecodedefinition/)
* assembly [Aspose.Tasks](../../../)


