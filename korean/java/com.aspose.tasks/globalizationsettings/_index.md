---
title: "GlobalizationSettings"
second_title: "Aspose.Tasks for Java API Reference"
description: "프로젝트의 글로벌화 설정을 나타냅니다."
type: docs
weight: 114
url: /ko/java/com.aspose.tasks/globalizationsettings/
---

**Inheritance:**
java.lang.Object
```
public class GlobalizationSettings
```

프로젝트의 글로벌화 설정을 나타냅니다.

프로젝트 전체에서 문화에 독립적인 리터럴이나 형식을 사용하는 것이 권장됩니다. 그러나 프로젝트가 문화별 리터럴을 사용하는 경우, 이 클래스를 사용하여 수식 계산 엔진이 해당 리터럴을 구문 분석하도록 도울 수 있습니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [GlobalizationSettings()](#GlobalizationSettings--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getFalseLiteral()](#getFalseLiteral--) | 수식에서 사용되는 boolean 'false' 리터럴에 대한 문자열을 가져옵니다. |
| [getFormulaDateNA()](#getFormulaDateNA--) | 날짜 필드에 대한 수식에서 사용되는 "NA"(빈 값) 리터럴을 가져옵니다. |
| [getTrueLiteral()](#getTrueLiteral--) | 수식에서 사용되는 boolean 'true' 리터럴에 대한 문자열을 가져옵니다. |
### GlobalizationSettings() {#GlobalizationSettings--}
```
public GlobalizationSettings()
```


### getFalseLiteral() {#getFalseLiteral--}
```
public String getFalseLiteral()
```


수식에서 사용되는 boolean 'false' 리터럴에 대한 문자열을 가져옵니다.

**Returns:**
java.lang.String - 수식에서 사용되는 부울 'false' 리터럴 문자열.
### getFormulaDateNA() {#getFormulaDateNA--}
```
public String getFormulaDateNA()
```


날짜 필드에 대한 수식에서 사용되는 "NA"(빈 값) 리터럴을 가져옵니다.

**Returns:**
java.lang.String - "NA" (빈 값) 리터럴이 날짜 필드의 수식에서 사용됩니다.
### getTrueLiteral() {#getTrueLiteral--}
```
public String getTrueLiteral()
```


수식에서 사용되는 boolean 'true' 리터럴에 대한 문자열을 가져옵니다.

**Returns:**
java.lang.String - 수식에서 사용되는 부울 'true' 리터럴 문자열.
