---
title: "ExtendedAttributeDefinition"
second_title: "Aspose.Tasks for Python via .NET API 참조"
description: 
type: docs
weight: 310
url: /ko/python-net/aspose.tasks/extendedattributedefinition/
---

## ExtendedAttributeDefinition class

프로젝트와 연관된 확장 속성 정의를 나타냅니다.

ExtendedAttributeDefinition 유형은 다음 멤버를 노출합니다:
## 속성
| 이름 | 설명 |
| :- | :- |
| field_id | 맞춤 필드의 프로젝트 ID에 해당하도록 가져오거나 설정합니다.<br/>            [ExtendedAttributeTask](/tasks/python-net/aspose.tasks/extendedattributetask/) 클래스의 상수 문자열 표현을 사용하여 [field_id](/tasks/python-net/aspose.tasks/extendedattributedefinition/) 속성을 지정합니다. |
| field_name | 맞춤 필드의 이름을 가져옵니다. |
| cf_type | 맞춤 필드의 유형을 가져옵니다. |
| guid | 맞춤 필드의 Guid를 가져오거나 설정합니다. |
| element_type | 확장 속성이 작업, 리소스 또는 할당과 연결되도록 가져오거나 설정합니다<br/>            작업, 리소스 또는 할당과 연결됩니다. |
| max_multi_values | 픽 리스트에서 설정할 수 있는 값의 최대 개수를 가져오거나 설정합니다. |
| user_def | 사용자 정의 필드인지 여부를 나타내는 값을 가져오거나 설정합니다. |
| alias | 사용자 정의 필드의 별칭을 가져오거나 설정합니다. |
| secondary_pid | 사용자 정의 필드의 보조 PID를 가져오거나 설정합니다. |
| auto_roll_down | 할당에 대한 자동 롤다운이 활성화되어 있는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| default_guid | 기본 조회 테이블 항목의 Guid를 가져오거나 설정합니다. |
| lookup_uid | 사용자 정의 필드와 연결된 조회 테이블의 Guid를 가져옵니다. |
| phonetics_alias | 사용자 정의 필드 별칭의 음성 발음을 가져오거나 설정합니다. |
| rollup_type | 롤업이 계산되는 방식을 가져오거나 설정합니다. |
| calculation_type | 사용자 정의 속성 값의 계산 유형을 가져오거나 설정합니다. |
| summary_rows_calculation_type | 요약 행에 대한 사용자 정의 속성 값의 계산 유형을 가져오거나 설정합니다. |
| formula | Microsoft Project가 사용자 정의 작업 필드를 채우는 데 사용하는 수식을 가져오거나 설정합니다. |
| graphical_indicator | 확장 속성과 연결된 그래픽 표시기 정보를 가져오거나 설정합니다.<br/>            MPP 형식에 적용됩니다. |
| restrict_values | 사용자 정의 필드 값이 [value_list](/tasks/python-net/aspose.tasks/extendedattributedefinition/)에 있는 값으로 제한되는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| valuelist_sort_order | 값 목록이 정렬되는 방식을 가져오거나 설정합니다. 값은: 0=내림차순, 1=오름차순. |
| append_new_values | 프로젝트에 추가된 새 값이 자동으로 목록에 추가되는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| default | 목록의 기본값을 가져오거나 설정합니다. |
| value_list | List<Value> ValueList를 가져옵니다. |
| secondary_guid | 확장 속성의 보조 GUID를 가져오거나 설정합니다. |
| parent_project | [ExtendedAttributeDefinition](/tasks/python-net/aspose.tasks/extendedattributedefinition/) 인스턴스의 상위 프로젝트를 가져옵니다. |
## 메서드
| 이름 | 설명 |
| :- | :- |
| create_extended_attribute() | 이 객체의 필드 ID 값과 동일한 필드 ID를 가진 새 확장 속성을 생성합니다. |
| create_extended_attribute(text_value) | 이 객체의 필드 ID 값과 동일한 필드 ID를 가지고 지정된 텍스트 값을 가진 새 확장 속성을 생성합니다. |
| create_extended_attribute(numeric_value) | 이 객체의 필드 ID 값과 동일한 필드 ID를 가지고 지정된 숫자 값을 가진 새 확장 속성을 생성합니다. |
| create_extended_attribute(date_time_value) | 이 객체의 필드 ID 값과 동일한 필드 ID를 가지고 지정된 날짜 값을 가진 새 확장 속성을 생성합니다. |
| create_extended_attribute(duration_value) | 이 객체의 필드 ID 값과 동일한 필드 ID를 가지고 지정된 기간 값을 가진 새 확장 속성을 생성합니다. |
| create_extended_attribute(flag_value) | 이 객체의 필드 ID 값과 동일한 필드 ID를 가지고 지정된 플래그 값을 가진 새 확장 속성을 생성합니다. |
| create_extended_attribute(lookup_value) | 지정된 [Value](/tasks/python-net/aspose.tasks/value/) 항목과 연결된 새로운 확장 속성을 생성합니다. |
| create_task_definition(custom_field_type, field_id, alias) | Microsoft Project에서 "None"으로 표시되는 간단한 확장 속성 정의를 생성하는 팩터리 메서드입니다.<br/>            [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/)이 [NONE](/tasks/python-net/aspose.tasks/calculationtype/)으로 설정되어 있으며 작업에만 사용할 수 있습니다.<br/>            지정해야 합니다. |
| create_task_definition(field_id, alias) | Microsoft Project에서 "None"으로 표시되는 간단한 확장 속성 정의를 생성하는 팩터리 메서드입니다.<br/>            [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/)이 [NONE](/tasks/python-net/aspose.tasks/calculationtype/)으로 설정되어 있으며 작업에만 사용할 수 있습니다.<br/>            지정해야 합니다. |
| create_resource_definition(custom_field_type, field_id, alias) | Microsoft Project에서 "None"으로 표시되는 간단한 확장 속성 정의를 생성하는 팩터리 메서드입니다.<br/>            [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/)이 [NONE](/tasks/python-net/aspose.tasks/calculationtype/)으로 설정되어 있으며 리소스에만 사용할 수 있습니다.<br/>            지정해야 합니다. |
| create_resource_definition(field_id, alias) | Microsoft Project에서 "None"으로 표시되는 간단한 확장 속성 정의를 생성하는 팩터리 메서드입니다.<br/>            [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/)이 [NONE](/tasks/python-net/aspose.tasks/calculationtype/)으로 설정되어 있으며 리소스에만 사용할 수 있습니다.<br/>            지정해야 합니다. |
| create_lookup_task_definition(field_id, alias) | 조회 기능이 있는 확장 속성 정의를 생성하는 팩터리 메서드입니다.<br/>            [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/)이 [LOOKUP](/tasks/python-net/aspose.tasks/calculationtype/)으로 설정되어 있으며 작업에만 사용할 수 있습니다.<br/>            지정해야 합니다. |
| create_lookup_task_definition(custom_field_type, field_id, alias) | 조회 기능이 있는 확장 속성 정의를 생성하는 팩터리 메서드입니다.<br/>            [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/)이 [LOOKUP](/tasks/python-net/aspose.tasks/calculationtype/)으로 설정되어 있으며 작업에만 사용할 수 있습니다.<br/>            지정해야 합니다. |
| create_lookup_resource_definition(field_id, alias) | 조회 기능이 있는 확장 속성 정의를 생성하는 팩터리 메서드입니다.<br/>            [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/)이 [LOOKUP](/tasks/python-net/aspose.tasks/calculationtype/)으로 설정되어 있으며 리소스에만 사용할 수 있습니다.<br/>            지정해야 합니다. |
| create_lookup_resource_definition(custom_field_type, field_id, alias) | 조회 기능이 있는 확장 속성 정의를 생성하는 팩터리 메서드입니다.<br/>            [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/)이 [LOOKUP](/tasks/python-net/aspose.tasks/calculationtype/)으로 설정되어 있으며 리소스에만 사용할 수 있습니다.<br/>            지정해야 합니다. |
| add_lookup_value(value) | 내부 조회 목록에 값을 추가합니다. 이는 [value_list](/tasks/python-net/aspose.tasks/extendedattributedefinition/)를 조작하는 권장 방법입니다. |
| remove_lookup_value(value) | 내부 조회 목록에서 값을 제거합니다. 이는 [value_list](/tasks/python-net/aspose.tasks/extendedattributedefinition/)를 조작하는 권장 방법입니다. |

### 또 보기

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

