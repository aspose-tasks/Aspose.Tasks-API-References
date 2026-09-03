---
title: "Aspose::Tasks::ExtendedAttributeDefinition::CreateResourceDefinition 메서드"
linktitle: "CreateResourceDefinition"
articleTitle: "CreateResourceDefinition"
second_title: "C++용 Aspose.Tasks"
description: "Microsoft Project에서 \"None\"으로 표시되는 단순 확장 속성 정의를 생성하는 팩터리 메서드입니다."
type: docs
weight: 50
url: /ko/cpp/aspose.tasks/extendedattributedefinition/createresourcedefinition/
---

## CreateResourceDefinition (1 of 2) {#createresourcedefinition_1}

Microsoft Project에서 "None"으로 표시되는 간단한 확장 속성 정의를 생성하는 팩터리 메서드입니다. CalculationType이 Tasks::CalculationType::None과 같으며 리소스에서만 사용할 수 있습니다. 이 메서드를 호출할 때 customFieldType, fieldId 및 alias를 지정해야 합니다.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified customFieldType , fieldId and alias .

```cpp
CreateResourceDefinition(CustomFieldType customFieldType, ExtendedAttributeResource fieldId, const System::String & alias)
```

| 매개변수 | 설명 |
| --- | --- |
| customFieldType | 지정된 CustomFieldType 유형입니다. |
| fieldId | 지정된 ExtendedAttributeResource 필드 ID입니다. |
| alias | 지정된 System::String 별칭입니다. |

---

## CreateResourceDefinition (2 of 2) {#createresourcedefinition_2}

간단한 확장 속성 정의를 생성하는 팩토리 메서드이며, Microsoft Project에서 "None"으로 표시됩니다. CalculationType이 Tasks::CalculationType::None과 같으며 Resource에서만 사용할 수 있습니다. 이 메서드를 호출할 때 fieldId와 alias를 지정해야 합니다. 필드 유형은 field id에서 추론됩니다.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified fieldId and alias .

```cpp
CreateResourceDefinition(ExtendedAttributeResource fieldId, const System::String & alias)
```

| 매개변수 | 설명 |
| --- | --- |
| fieldId | 지정된 ExtendedAttributeResource 필드 ID입니다. |
| alias | 지정된 System::String 별칭입니다. |

