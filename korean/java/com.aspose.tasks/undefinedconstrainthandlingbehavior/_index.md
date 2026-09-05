---
title: "UndefinedConstraintHandlingBehavior"
second_title: "Aspose.Tasks for Java API Reference"
description: "정의되지 않은 제약 조건을 가진 작업을 처리하는 데 사용되는 동작을 지정합니다."
type: docs
weight: 329
url: /ko/java/com.aspose.tasks/undefinedconstrainthandlingbehavior/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class UndefinedConstraintHandlingBehavior extends System.Enum
```

정의되지 않은 제약 조건을 가진 작업을 처리하는 데 사용되는 동작을 지정합니다.
## 필드

| 필드 | 설명 |
| --- | --- |
| [None](#None) | XER 형식에서 로드할 때의 기본 동작. |
| [SubstituteWithStartNoEarlierThan](#SubstituteWithStartNoEarlierThan) | 'ConstraintType.StartNoEarlierThan' 유형 및 date = Start인 제약 조건이 'Undefined' 제약을 가진 작업에 추가됩니다. |
### None {#None}
```
public static final int None
```


XER 형식에서 로드할 때의 기본 동작입니다. 아무 작업도 수행되지 않으며, 작업 제약 유형이 'ConstraintType.Undefined'으로 설정됩니다.

### SubstituteWithStartNoEarlierThan {#SubstituteWithStartNoEarlierThan}
```
public static final int SubstituteWithStartNoEarlierThan
```


'ConstraintType.StartNoEarlierThan' 유형 및 date = Start인 제약 조건이 'Undefined' 제약을 가진 작업에 추가됩니다.

