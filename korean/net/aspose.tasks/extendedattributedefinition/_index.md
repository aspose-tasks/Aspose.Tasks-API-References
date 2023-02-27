---
title: ExtendedAttributeDefinition
second_title: .NET API 참조용 Aspose.Tasks
description: 프로젝트와 연결된 확장된 속성 정의를 나타냅니다.
type: docs
weight: 540
url: /ko/net/aspose.tasks/extendedattributedefinition/
---
## ExtendedAttributeDefinition class

프로젝트와 연결된 확장된 속성 정의를 나타냅니다.

```csharp
public class ExtendedAttributeDefinition
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [Alias](../../aspose.tasks/extendedattributedefinition/alias/) { get; set; } | 사용자 정의 필드의 별칭을 가져오거나 설정합니다. |
| [AppendNewValues](../../aspose.tasks/extendedattributedefinition/appendnewvalues/) { get; set; } | 프로젝트에 추가된 새 값이 목록에 자동으로 추가되는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [AutoRollDown](../../aspose.tasks/extendedattributedefinition/autorolldown/) { get; set; } | 할당에 대한 자동 롤다운이 활성화되었는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [CalculationType](../../aspose.tasks/extendedattributedefinition/calculationtype/) { get; set; } | 사용자 정의 속성 값의 계산 유형을 가져오거나 설정합니다. |
| [CfType](../../aspose.tasks/extendedattributedefinition/cftype/) { get; } | 사용자 정의 필드의 유형을 가져옵니다. |
| [Default](../../aspose.tasks/extendedattributedefinition/default/) { get; set; } | 목록의 기본값을 가져오거나 설정합니다. |
| [DefaultGuid](../../aspose.tasks/extendedattributedefinition/defaultguid/) { get; set; } | 기본 조회 테이블 항목의 Guid를 가져오거나 설정합니다. |
| [ElementType](../../aspose.tasks/extendedattributedefinition/elementtype/) { get; set; } | 가져오거나 설정하는 확장 속성은 작업, 리소스 또는 할당과 연관 됩니다. |
| [FieldId](../../aspose.tasks/extendedattributedefinition/fieldid/) { get; set; } | 사용자 정의 필드의 프로젝트 ID에 해당하는 가져오기 또는 설정. 상수의 문자열 표현 사용[`ExtendedAttributeTask`](../extendedattributetask/) 지정할 클래스[`FieldId`](./fieldid/) 속성. |
| [FieldName](../../aspose.tasks/extendedattributedefinition/fieldname/) { get; } | 사용자 정의 필드의 이름을 가져옵니다. |
| [Formula](../../aspose.tasks/extendedattributedefinition/formula/) { get; set; } | Microsoft Project에서 사용자 지정 작업 필드를 채우는 데 사용하는 수식을 가져오거나 설정합니다. |
| [Guid](../../aspose.tasks/extendedattributedefinition/guid/) { get; set; } | 사용자 정의 필드의 Guid를 가져오거나 설정합니다. |
| [LookupUid](../../aspose.tasks/extendedattributedefinition/lookupuid/) { get; } | 사용자 정의 필드와 연결된 조회 테이블의 Guid를 가져옵니다. |
| [MaxMultiValues](../../aspose.tasks/extendedattributedefinition/maxmultivalues/) { get; set; } | 선택 목록에서 설정할 수 있는 최대 값 수를 가져오거나 설정합니다. |
| [ParentProject](../../aspose.tasks/extendedattributedefinition/parentproject/) { get; } | 에 대한 상위 프로젝트를 가져옵니다.`ExtendedAttributeDefinition` 인스턴스. |
| [PhoneticsAlias](../../aspose.tasks/extendedattributedefinition/phoneticsalias/) { get; set; } | 사용자 정의 필드 별칭의 음성 발음을 가져오거나 설정합니다. |
| [RestrictValues](../../aspose.tasks/extendedattributedefinition/restrictvalues/) { get; set; } | 사용자 정의 필드 값이[`ValueList`](./valuelist/) . |
| [RollupType](../../aspose.tasks/extendedattributedefinition/rolluptype/) { get; set; } | 롤업이 계산되는 방식을 가져오거나 설정합니다. |
| [SecondaryGuid](../../aspose.tasks/extendedattributedefinition/secondaryguid/) { get; set; } | 확장 속성의 보조 GUID를 가져오거나 설정합니다. |
| [SecondaryPid](../../aspose.tasks/extendedattributedefinition/secondarypid/) { get; set; } | 사용자 정의 필드의 보조 PID를 가져오거나 설정합니다. |
| [SummaryRowsCalculationType](../../aspose.tasks/extendedattributedefinition/summaryrowscalculationtype/) { get; set; } | 요약 행에 대한 사용자 정의 속성 값의 계산 유형을 가져오거나 설정합니다. |
| [UserDef](../../aspose.tasks/extendedattributedefinition/userdef/) { get; set; } | 사용자 정의 필드가 사용자 정의인지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [ValueList](../../aspose.tasks/extendedattributedefinition/valuelist/) { get; } | List&lt;Value&gt; ValueList를 가져옵니다. |
| [ValuelistSortOrder](../../aspose.tasks/extendedattributedefinition/valuelistsortorder/) { get; set; } | 값 목록이 정렬되는 방식을 가져오거나 설정합니다. 값: 0=내림차순, 1=오름차순. |

## 행동 양식

| 이름 | 설명 |
| --- | --- |
| static [CreateLookupResourceDefinition](../../aspose.tasks/extendedattributedefinition/createlookupresourcedefinition/#createlookupresourcedefinition_1)(ExtendedAttributeResource, string) | 조회를 통해 확장된 속성 정의를 생성하는 팩토리 메서드입니다. [`CalculationType`](./calculationtype/) 와 같다Lookup 리소스에서만 사용할 수 있습니다. 지정해야 합니다.*fieldId* 그리고*alias* 이 메소드를 호출할 때. 필드 유형은 필드 id. 에서 유추됩니다. |
| static [CreateLookupResourceDefinition](../../aspose.tasks/extendedattributedefinition/createlookupresourcedefinition/#createlookupresourcedefinition)(CustomFieldType, ExtendedAttributeResource, string) | 조회를 통해 확장된 속성 정의를 생성하는 팩토리 메서드입니다. [`CalculationType`](./calculationtype/) 와 같다Lookup 리소스에서만 사용할 수 있습니다. 지정해야 합니다.*customFieldType* ,*fieldId* 그리고*alias* 이 메서드를 호출할 때. |
| static [CreateLookupTaskDefinition](../../aspose.tasks/extendedattributedefinition/createlookuptaskdefinition/#createlookuptaskdefinition_1)(ExtendedAttributeTask, string) | 조회를 통해 확장된 속성 정의를 생성하는 팩토리 메서드입니다. [`CalculationType`](./calculationtype/) 와 같다Lookup 작업에서만 사용할 수 있습니다. 지정해야 합니다.*fieldId* 그리고*alias* 이 메소드를 호출할 때. 필드 유형은 필드 id. 에서 유추됩니다. |
| static [CreateLookupTaskDefinition](../../aspose.tasks/extendedattributedefinition/createlookuptaskdefinition/#createlookuptaskdefinition)(CustomFieldType, ExtendedAttributeTask, string) | 조회를 통해 확장된 속성 정의를 생성하는 팩토리 메서드입니다. [`CalculationType`](./calculationtype/) 와 같다Lookup 작업에서만 사용할 수 있습니다. 지정해야 합니다.*customFieldType* ,*fieldId* 그리고*alias* 이 메서드를 호출할 때. |
| static [CreateResourceDefinition](../../aspose.tasks/extendedattributedefinition/createresourcedefinition/#createresourcedefinition_1)(ExtendedAttributeResource, string) | Microsoft Project에서 "없음"으로 표시되는 단순 확장 속성 정의를 생성하는 팩터리 메서드입니다. [`CalculationType`](./calculationtype/) 와 같다None 리소스에서만 사용할 수 있습니다. 지정해야 합니다.*fieldId* 그리고*alias* 이 메소드를 호출할 때. 필드 유형은 필드 id. 에서 유추됩니다. |
| static [CreateResourceDefinition](../../aspose.tasks/extendedattributedefinition/createresourcedefinition/#createresourcedefinition)(CustomFieldType, ExtendedAttributeResource, string) | Microsoft Project에서 "없음"으로 표시되는 단순 확장 속성 정의를 생성하는 팩터리 메서드입니다. [`CalculationType`](./calculationtype/) 와 같다None 리소스에서만 사용할 수 있습니다. 지정해야 합니다.*customFieldType* ,*fieldId* 그리고*alias* 이 메서드를 호출할 때. |
| static [CreateTaskDefinition](../../aspose.tasks/extendedattributedefinition/createtaskdefinition/#createtaskdefinition_1)(ExtendedAttributeTask, string) | Microsoft Project에서 "없음"으로 표시되는 단순 확장 속성 정의를 생성하는 팩터리 메서드입니다. [`CalculationType`](./calculationtype/) 와 같다None 작업에서만 사용할 수 있습니다. 지정해야 합니다.*fieldId* 그리고*alias* 이 메서드를 호출할 때. 필드 유형은 필드 id. 에서 유추됩니다. |
| static [CreateTaskDefinition](../../aspose.tasks/extendedattributedefinition/createtaskdefinition/#createtaskdefinition)(CustomFieldType, ExtendedAttributeTask, string) | Microsoft Project에서 "없음"으로 표시되는 단순 확장 속성 정의를 생성하는 팩터리 메서드입니다. [`CalculationType`](./calculationtype/) 와 같다None 작업에서만 사용할 수 있습니다. 지정해야 합니다.*customFieldType* ,*fieldId* 그리고*alias* 이 메서드를 호출할 때. |
| [AddLookupValue](../../aspose.tasks/extendedattributedefinition/addlookupvalue/)(Value) | 내부 조회 목록에 값을 추가합니다. 이것은 다음과 같은 조작에 바람직한 방법입니다.[`ValueList`](./valuelist/) . |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute)() | 이 개체의 필드 ID 값과 동일한 필드 ID를 사용하여 새 확장 특성을 만듭니다. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_3)(bool) | 이 개체의 필드 ID 값 및 지정된 플래그 값과 동일한 필드 ID를 사용하여 새 확장 특성을 만듭니다. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_4)(DateTime) | 이 개체의 필드 ID 값 및 지정된 날짜 값과 동일한 필드 ID를 사용하여 새 확장 특성을 만듭니다. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_5)(decimal) | 이 개체의 필드 ID 값 및 지정된 숫자 값과 동일한 필드 ID를 사용하여 새 확장 특성을 만듭니다. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_1)(Duration) | 이 개체의 필드 ID 값 및 지정된 기간 값과 동일한 필드 ID를 사용하여 새 확장 특성을 만듭니다. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_6)(string) | 이 개체의 필드 ID 값 및 지정된 텍스트 값과 동일한 필드 ID를 사용하여 새 확장 특성을 만듭니다. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_2)(Value) | 지정된 새 확장 속성을 생성합니다.[`Value`](../value/) 항목. |
| override [Equals](../../aspose.tasks/extendedattributedefinition/equals/)(object) | 이 인스턴스가 지정된 개체와 같은지 여부를 나타내는 플래그를 반환합니다. |
| override [GetHashCode](../../aspose.tasks/extendedattributedefinition/gethashcode/)() | 인스턴스의 해시 코드를 반환합니다.`ExtendedAttributeDefinition` 클래스. |
| [RemoveLookupValue](../../aspose.tasks/extendedattributedefinition/removelookupvalue/)(Value) | 내부 조회 목록에서 값을 제거합니다. 이것은 다음과 같은 조작에 바람직한 방법입니다.[`ValueList`](./valuelist/) . |

### 또한보십시오

* 네임스페이스 [Aspose.Tasks](../../aspose.tasks/)
* 집회 [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
