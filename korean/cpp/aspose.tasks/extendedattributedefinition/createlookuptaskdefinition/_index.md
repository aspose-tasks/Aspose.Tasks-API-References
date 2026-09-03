---
title: "Aspose::Tasks::ExtendedAttributeDefinition::CreateLookupTaskDefinition 메서드"
linktitle: "CreateLookupTaskDefinition"
articleTitle: "CreateLookupTaskDefinition"
second_title: "C++용 Aspose.Tasks"
description: "조회 기능이 포함된 확장 속성 정의를 생성하는 팩터리 메서드입니다."
type: docs
weight: 40
url: /ko/cpp/aspose.tasks/extendedattributedefinition/createlookuptaskdefinition/
---

## CreateLookupTaskDefinition (1 of 2) {#createlookuptaskdefinition_1}

조회가 포함된 확장 속성 정의를 생성하는 팩터리 메서드입니다. CalculationType이 Tasks::CalculationType::Lookup과 같으며 작업에서만 사용할 수 있습니다. 이 메서드를 호출할 때 customFieldType, fieldId 및 alias를 지정해야 합니다.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified customFieldType , fieldId and alias .

```cpp
CreateLookupTaskDefinition(CustomFieldType customFieldType, ExtendedAttributeTask fieldId, const System::String & alias)
```

| 매개변수 | 설명 |
| --- | --- |
| customFieldType | 지정된 CustomFieldType 유형입니다. |
| fieldId | 지정된 ExtendedAttributeTask 필드 ID입니다. |
| alias | 지정된 System::String 별칭입니다. |

---

## CreateLookupTaskDefinition (2 of 2) {#createlookuptaskdefinition_2}

조회가 포함된 확장 속성 정의를 생성하는 팩터리 메서드입니다. CalculationType이 Tasks::CalculationType::Lookup과 같으며 Tasks에서만 사용할 수 있습니다. 이 메서드를 호출할 때 fieldId와 alias를 지정해야 합니다. 필드 유형은 field id에서 추론됩니다.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified fieldId and alias .

```cpp
CreateLookupTaskDefinition(ExtendedAttributeTask fieldId, const System::String & alias)
```

| 매개변수 | 설명 |
| --- | --- |
| fieldId | 지정된 ExtendedAttributeTask 필드 ID입니다. |
| alias | 지정된 System::String 별칭입니다. |

