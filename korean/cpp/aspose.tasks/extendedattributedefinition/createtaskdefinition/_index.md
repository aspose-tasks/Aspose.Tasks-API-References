---
title: "Aspose::Tasks::ExtendedAttributeDefinition::CreateTaskDefinition 메서드"
linktitle: "CreateTaskDefinition"
articleTitle: "CreateTaskDefinition"
second_title: "C++용 Aspose.Tasks"
description: "Microsoft Project에서 \"None\"으로 표시되는 단순 확장 속성 정의를 생성하는 팩터리 메서드입니다."
type: docs
weight: 60
url: /ko/cpp/aspose.tasks/extendedattributedefinition/createtaskdefinition/
---

## CreateTaskDefinition (1 of 2) {#createtaskdefinition_1}

Microsoft Project에서 "None"으로 표시되는 간단한 확장 속성 정의를 생성하는 팩터리 메서드입니다. CalculationType이 Tasks::CalculationType::None과 같으며 작업에서만 사용할 수 있습니다. 이 메서드를 호출할 때 customFieldType, fieldId 및 alias를 지정해야 합니다.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified customFieldType , fieldId and alias .

```cpp
CreateTaskDefinition(CustomFieldType customFieldType, ExtendedAttributeTask fieldId, const System::String & alias)
```

| 매개변수 | 설명 |
| --- | --- |
| customFieldType | 지정된 CustomFieldType 유형입니다. |
| fieldId | 지정된 ExtendedAttributeTask 필드 ID입니다. |
| alias | 지정된 System::String 별칭입니다. |

---

## CreateTaskDefinition (2 of 2) {#createtaskdefinition_2}

Microsoft Project에서 "None"으로 표시되는 단순 확장 속성 정의를 생성하는 팩터리 메서드입니다. CalculationType이 Tasks::CalculationType::None과 같으며 Tasks에서만 사용할 수 있습니다. 이 메서드를 호출할 때 fieldId와 alias를 지정해야 합니다. 필드 유형은 field id에서 추론됩니다.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified fieldId and alias .

```cpp
CreateTaskDefinition(ExtendedAttributeTask fieldId, const System::String & alias)
```

| 매개변수 | 설명 |
| --- | --- |
| fieldId | 지정된 ExtendedAttributeTask 필드 ID입니다. |
| alias | 지정된 System::String 별칭입니다. |

