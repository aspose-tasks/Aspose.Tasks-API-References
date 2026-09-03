---
title: "Aspose::Tasks::ExtendedAttributeDefinition 클래스"
linktitle: "ExtendedAttributeDefinition"
articleTitle: "ExtendedAttributeDefinition"
second_title: "C++용 Aspose.Tasks"
description: "프로젝트와 연관된 확장 속성 정의를 나타냅니다."
type: docs
weight: 10
url: /ko/cpp/aspose.tasks/extendedattributedefinition/
---

## ExtendedAttributeDefinition class

프로젝트와 연관된 확장 속성 정의를 나타냅니다.

## 메서드

| 이름 | 설명 |
| --- | --- |
| [AddLookupValue](./addlookupvalue/) | 내부 조회 목록에 값을 추가합니다. 이는 ValueList와의 조작에 권장되는 방법입니다. |
| [CreateExtendedAttribute (7 overloads)](./createextendedattribute/) | 이 객체의 필드 ID 값과 동일한 필드 ID를 가진 새로운 확장 속성을 생성합니다. |
| [CreateLookupResourceDefinition (2 overloads)](./createlookupresourcedefinition/) | 조회가 포함된 확장 속성 정의를 생성하는 팩터리 메서드입니다. CalculationType이 Tasks::CalculationType::Lookup과 같으며 리소스에서만 사용할 수 있습니다. 이 메서드를 호출할 때 customFieldType, fieldId 및 alias를 지정해야 합니다. |
| [CreateLookupTaskDefinition (2 overloads)](./createlookuptaskdefinition/) | 조회가 포함된 확장 속성 정의를 생성하는 팩터리 메서드입니다. CalculationType이 Tasks::CalculationType::Lookup과 같으며 작업에서만 사용할 수 있습니다. 이 메서드를 호출할 때 customFieldType, fieldId 및 alias를 지정해야 합니다. |
| [CreateResourceDefinition (2 overloads)](./createresourcedefinition/) | Microsoft Project에서 "None"으로 표시되는 간단한 확장 속성 정의를 생성하는 팩터리 메서드입니다. CalculationType이 Tasks::CalculationType::None과 같으며 리소스에서만 사용할 수 있습니다. 이 메서드를 호출할 때 customFieldType, fieldId 및 alias를 지정해야 합니다. |
| [CreateTaskDefinition (2 overloads)](./createtaskdefinition/) | Microsoft Project에서 "None"으로 표시되는 간단한 확장 속성 정의를 생성하는 팩터리 메서드입니다. CalculationType이 Tasks::CalculationType::None과 같으며 작업에서만 사용할 수 있습니다. 이 메서드를 호출할 때 customFieldType, fieldId 및 alias를 지정해야 합니다. |
| [Equals](./equals/) | 이 인스턴스가 지정된 객체와 동일한지 여부를 나타내는 플래그를 반환합니다. |
| [get_Alias](./get_alias/) | 사용자 정의 필드의 별칭을 가져옵니다. |
| [get_AppendNewValues](./get_appendnewvalues/) | 프로젝트에 추가된 새 값이 자동으로 목록에 추가되는지 여부를 나타내는 값을 가져옵니다. |
| [get_AutoRollDown](./get_autorolldown/) | 할당에 대한 자동 롤다운이 활성화되어 있는지 여부를 나타내는 값을 가져옵니다. |
| [get_CalculationType](./get_calculationtype/) | 사용자 정의 속성 값의 계산 유형을 가져옵니다. |
| [get_CfType](./get_cftype/) | 사용자 정의 필드의 유형을 가져옵니다. |
| [get_Default](./get_default/) | 목록의 기본값을 가져옵니다. |
| [get_DefaultGuid](./get_defaultguid/) | 기본 조회 테이블 항목의 Guid를 가져옵니다. |
| [get_ElementType](./get_elementtype/) | 확장 속성이 작업, 리소스 또는 할당과 연결되어 있는지를 가져옵니다. |
| [get_FieldId](./get_fieldid/) | 사용자 정의 필드의 프로젝트 ID에 해당하는 값을 가져옵니다. FieldId 속성을 지정하려면 Aspose::Tasks::ExtendedAttributeTask 클래스의 상수 문자열 표현을 사용합니다. |
| [get_FieldName](./get_fieldname/) | 사용자 정의 필드의 이름을 가져옵니다. |
| [get_Formula](./get_formula/) | Microsoft Project가 사용자 정의 작업 필드를 채우는 데 사용하는 수식을 가져옵니다. |
| [get_GraphicalIndicator](./get_graphicalindicator/) | 확장 속성과 연결된 그래픽 표시기 정보를 가져옵니다. MPP 형식에 적용됩니다. |
| [get_Guid](./get_guid/) | 사용자 정의 필드의 Guid를 가져옵니다. |
| [get_LookupUid](./get_lookupuid/) | 사용자 정의 필드와 연결된 조회 테이블의 Guid를 가져옵니다. |
| [get_MaxMultiValues](./get_maxmultivalues/) | 픽 리스트에 설정할 수 있는 최대 값 개수를 가져옵니다. |
| [get_ParentProject](./get_parentproject/) | ExtendedAttributeDefinition 인스턴스의 상위 프로젝트를 가져옵니다. |
| [get_PhoneticsAlias](./get_phoneticsalias/) | 사용자 정의 필드 별칭의 발음(음성)을 가져옵니다. |
| [get_RestrictValues](./get_restrictvalues/) | 사용자 정의 필드 값이 ValueList의 값으로 제한되는지 여부를 나타내는 값을 가져옵니다. |
| [get_RollupType](./get_rolluptype/) | 롤업이 계산되는 방식을 가져옵니다. |
| [get_SecondaryGuid](./get_secondaryguid/) | 확장 속성의 보조 guid를 가져옵니다. |
| [get_SecondaryPid](./get_secondarypid/) | 사용자 정의 필드의 보조 PID를 가져옵니다. |
| [get_SummaryRowsCalculationType](./get_summaryrowscalculationtype/) | 요약 행에 대한 사용자 정의 속성 값의 계산 유형을 가져옵니다. |
| [get_UserDef](./get_userdef/) | 사용자 정의 필드가 사용자 정의인지 여부를 나타내는 값을 가져옵니다. |
| [get_ValueList](./get_valuelist/) | List< Value > ValueList를 가져옵니다. |
| [get_ValuelistSortOrder](./get_valuelistsortorder/) | 값 목록이 정렬되는 방식을 가져옵니다. 값은: 0=내림차순, 1=오름차순. |
| [GetHashCode](./gethashcode/) | ExtendedAttributeDefinition 클래스 인스턴스에 대한 해시 코드를 반환합니다. |
| [RemoveLookupValue](./removelookupvalue/) | 내부 조회 목록에서 값을 제거합니다. 이는 ValueList와의 조작에 선호되는 방법입니다. |
| [set_Alias](./set_alias/) | 사용자 정의 필드의 별칭을 설정합니다. |
| [set_AppendNewValues](./set_appendnewvalues/) | 프로젝트에 추가된 새 값이 자동으로 목록에 추가되는지 여부를 나타내는 값을 설정합니다. |
| [set_AutoRollDown](./set_autorolldown/) | 할당에 대한 자동 롤다운이 활성화되는지 여부를 나타내는 값을 설정합니다. |
| [set_CalculationType](./set_calculationtype/) | 사용자 정의 속성 값의 계산 유형을 설정합니다. |
| [set_Default](./set_default/) | 목록의 기본 값을 설정합니다. |
| [set_DefaultGuid](./set_defaultguid/) | 기본 조회 테이블 항목의 Guid를 설정합니다. |
| [set_ElementType](./set_elementtype/) | 확장 속성이 작업, 리소스 또는 할당과 연결되도록 설정합니다. |
| [set_FieldId](./set_fieldid/) | 사용자 정의 필드의 프로젝트 ID에 해당하도록 설정합니다. FieldId 속성을 지정하려면 Aspose::Tasks::ExtendedAttributeTask 클래스의 상수 문자열 표현을 사용합니다. |
| [set_Formula](./set_formula/) | Microsoft Project가 사용자 정의 작업 필드를 채우는 데 사용하는 수식을 설정합니다. |
| [set_GraphicalIndicator](./set_graphicalindicator/) | 확장 속성과 연결된 그래픽 표시기 정보를 설정합니다. MPP 형식에 적용됩니다. |
| [set_Guid](./set_guid/) | 사용자 정의 필드의 Guid를 설정합니다. |
| [set_MaxMultiValues](./set_maxmultivalues/) | 픽 리스트에 설정할 수 있는 최대 값 개수를 설정합니다. |
| [set_PhoneticsAlias](./set_phoneticsalias/) | 사용자 정의 필드 별칭의 음성 발음을 설정합니다. |
| [set_RestrictValues](./set_restrictvalues/) | 사용자 정의 필드 값이 ValueList의 값으로 제한되는지 여부를 나타내는 값을 설정합니다. |
| [set_RollupType](./set_rolluptype/) | 롤업이 계산되는 방식을 설정합니다. |
| [set_SecondaryGuid](./set_secondaryguid/) | 확장 속성의 보조 guid를 설정합니다. |
| [set_SecondaryPid](./set_secondarypid/) | 사용자 정의 필드의 보조 PID를 설정합니다. |
| [set_SummaryRowsCalculationType](./set_summaryrowscalculationtype/) | 요약 행에 대한 사용자 정의 속성 값의 계산 유형을 설정합니다. |
| [set_UserDef](./set_userdef/) | 사용자 정의 필드가 사용자 정의인지 여부를 나타내는 값을 설정합니다. |
| [set_ValuelistSortOrder](./set_valuelistsortorder/) | 값 목록이 정렬되는 방식을 설정합니다. 값은: 0=내림차순, 1=오름차순. |

