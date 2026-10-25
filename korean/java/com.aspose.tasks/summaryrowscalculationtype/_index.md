---
title: "SummaryRowsCalculationType"
second_title: "Aspose.Tasks for Java API Reference"
description: "요약 행에 대한 사용자 지정 속성 값 계산 유형을 지정합니다."
type: docs
weight: 282
url: /ko/java/com.aspose.tasks/summaryrowscalculationtype/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class SummaryRowsCalculationType extends System.Enum
```

요약 행에 대한 사용자 정의 속성 값 계산 유형을 지정합니다.
## 필드

| 필드 | 설명 |
| --- | --- |
| [None](#None) | 요약 행에 대한 사용자 정의 속성 값이 계산되지 않음을 의미합니다. |
| [Rollup](#Rollup) | 요약 행에 대한 사용자 정의 속성 값이 `ExtendedAttributeDefinition.RollupType`에 정의된 롤업 함수를 사용하여 계산됨을 의미합니다(`ExtendedAttributeDefinition.RollupType`([ExtendedAttributeDefinition.getRollupType()](../../com.aspose/tasks/extendedattributedefinition\#getRollupType--)/ [ExtendedAttributeDefinition.setRollupType(int)](../../com.aspose/tasks/extendedattributedefinition\#setRollupType-int-)). |
| [UseFormula](#UseFormula) | 요약 행에 대한 사용자 정의 속성 값이 `ExtendedAttributeDefinition.Formula`에 정의된 수식을 사용하여 계산됨을 의미합니다(`ExtendedAttributeDefinition.Formula`([ExtendedAttributeDefinition.getFormula()](../../com.aspose/tasks/extendedattributedefinition\#getFormula--)/ [ExtendedAttributeDefinition.setFormula(String)](../../com.aspose/tasks/extendedattributedefinition\#setFormula-String-)). |
### None {#None}
```
public static final int None
```


요약 행에 대한 사용자 정의 속성 값이 계산되지 않음을 의미합니다.

### Rollup {#Rollup}
```
public static final int Rollup
```


요약 행에 대한 사용자 정의 속성 값이 `ExtendedAttributeDefinition.RollupType`에 정의된 롤업 함수를 사용하여 계산됨을 의미합니다(`ExtendedAttributeDefinition.RollupType`([ExtendedAttributeDefinition.getRollupType()](../../com.aspose/tasks/extendedattributedefinition\#getRollupType--)/ [ExtendedAttributeDefinition.setRollupType(int)](../../com.aspose/tasks/extendedattributedefinition\#setRollupType-int-)).

### UseFormula {#UseFormula}
```
public static final int UseFormula
```


요약 행에 대한 사용자 정의 속성 값이 `ExtendedAttributeDefinition.Formula`에 정의된 수식을 사용하여 계산됨을 의미합니다(`ExtendedAttributeDefinition.Formula`([ExtendedAttributeDefinition.getFormula()](../../com.aspose/tasks/extendedattributedefinition\#getFormula--)/ [ExtendedAttributeDefinition.setFormula(String)](../../com.aspose/tasks/extendedattributedefinition\#setFormula-String-)).

--------------------

이 설정이 작동하려면 `ExtendedAttributeDefinition.CalculationType`([ExtendedAttributeDefinition.getCalculationType()](../../com.aspose/tasks/extendedattributedefinition\#getCalculationType--)/ [ExtendedAttributeDefinition.setCalculationType(int)](../../com.aspose/tasks/extendedattributedefinition\#setCalculationType-int-))을 'Formula'로 설정해야 합니다.

