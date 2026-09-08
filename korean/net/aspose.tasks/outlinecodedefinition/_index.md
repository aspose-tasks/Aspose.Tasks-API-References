---
title: "클래스 OutlineCodeDefinition"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.OutlineCodeDefinition 클래스. 개요 코드 정의를 나타냅니다."
type: docs
weight: 1170
url: /ko/net/aspose.tasks/outlinecodedefinition/
---
## OutlineCodeDefinition class

아웃라인 코드 정의를 나타냅니다.

```csharp
public sealed class OutlineCodeDefinition
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [OutlineCodeDefinition](outlinecodedefinition/)() | `OutlineCodeDefinition` 클래스의 새 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [Alias](../../aspose.tasks/outlinecodedefinition/alias/) { get; set; } | 사용자 정의 개요 코드의 별칭을 가져오거나 설정합니다. |
| [AllLevelsRequired](../../aspose.tasks/outlinecodedefinition/alllevelsrequired/) { get; set; } | 새 코드가 모든 레벨을 가져야 하는지 여부를 나타내는 값을 가져오거나 설정합니다. 엔터프라이즈 코드에는 사용할 수 없습니다. |
| [Enterprise](../../aspose.tasks/outlinecodedefinition/enterprise/) { get; set; } | 사용자 정의 개요 코드가 엔터프라이즈 사용자 정의 개요 코드인지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [EnterpriseOutlineCodeAlias](../../aspose.tasks/outlinecodedefinition/enterpriseoutlinecodealias/) { get; set; } | 이 개요 코드 정의가 별칭인 다른 사용자 정의 필드에 대한 참조를 가져오거나 설정합니다. |
| [FieldId](../../aspose.tasks/outlinecodedefinition/fieldid/) { get; set; } | 개요 코드의 필드 번호를 가져오거나 설정합니다. |
| [FieldName](../../aspose.tasks/outlinecodedefinition/fieldname/) { get; set; } | 사용자 정의 개요 코드의 이름을 가져오거나 설정합니다. |
| [Guid](../../aspose.tasks/outlinecodedefinition/guid/) { get; set; } | 개요 코드의 Guid를 가져오거나 설정합니다. |
| [LeafOnly](../../aspose.tasks/outlinecodedefinition/leafonly/) { get; set; } | 이 개요 코드 필드에 지정된 값이 리프 값이어야 하는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [Masks](../../aspose.tasks/outlinecodedefinition/masks/) { get; } | OutlineMaskCollection 객체를 가져옵니다. 개요 코드 마스크를 정의하는 항목 테이블입니다. 읽기 전용 [`OutlineMaskCollection`](../outlinemaskcollection/) 인스턴스. |
| [OnlyTableValuesAllowed](../../aspose.tasks/outlinecodedefinition/onlytablevaluesallowed/) { get; set; } | 지정된 값이 값 테이블에서 가져와야 하는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [PhoneticAlias](../../aspose.tasks/outlinecodedefinition/phoneticalias/) { get; set; } | 사용자 정의 개요 코드 별칭의 음성 발음을 가져오거나 설정합니다. |
| [ResourceSubstitutionEnabled](../../aspose.tasks/outlinecodedefinition/resourcesubstitutionenabled/) { get; set; } | 사용자 정의 개요 코드를 Microsoft Project의 리소스 대체 마법사에서 사용할 수 있는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [ShowIndent](../../aspose.tasks/outlinecodedefinition/showindent/) { get; set; } | 이 개요 코드의 들여쓰기를 표시해야 하는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [Values](../../aspose.tasks/outlinecodedefinition/values/) { get; } | OutlineValueCollection 객체를 가져옵니다. 이 개요 코드와 연결된 테이블의 값들입니다. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


