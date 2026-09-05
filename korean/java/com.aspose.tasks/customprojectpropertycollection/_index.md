---
title: "CustomProjectPropertyCollection"
second_title: "Aspose.Tasks for Java API Reference"
description: "사용자 정의 프로젝트 속성 컬렉션을 나타냅니다."
type: docs
weight: 61
url: /ko/java/com.aspose.tasks/customprojectpropertycollection/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.PropertyCollection, com.aspose.tasks.PropertyKeyedCollection
```
public final class CustomProjectPropertyCollection extends PropertyKeyedCollection<CustomProjectProperty>
```

사용자 정의 프로젝트 속성 컬렉션을 나타냅니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [CustomProjectPropertyCollection()](#CustomProjectPropertyCollection--) | 새 인스턴스를 초기화합니다 [CustomProjectPropertyCollection](../../com.aspose.tasks/customprojectpropertycollection) 클래스. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [add(String name, boolean value)](#add-java.lang.String-boolean-) | 새 사용자 정의 속성을 생성합니다. |
| [add(String name, double value)](#add-java.lang.String-double-) | 새 사용자 정의 속성을 생성합니다. |
| [add(String name, String value)](#add-java.lang.String-java.lang.String-) | 새 사용자 정의 속성을 생성합니다. |
| [add(String name, Date value)](#add-java.lang.String-java.util.Date-) | 새 사용자 정의 속성을 생성합니다. |
| [clear()](#clear--) | PropertyCollection를 비웁니다. |
| [isReadOnly()](#isReadOnly--) | 이 컬렉션이 읽기 전용인지 여부를 나타내는 값을 가져옵니다; 그렇지 않으면 false. |
| [remove(String name)](#remove-java.lang.String-) | 지정된 이름을 가진 속성을 컬렉션에서 제거합니다. |
### CustomProjectPropertyCollection() {#CustomProjectPropertyCollection--}
```
public CustomProjectPropertyCollection()
```


새 인스턴스를 초기화합니다 [CustomProjectPropertyCollection](../../com.aspose.tasks/customprojectpropertycollection) 클래스.

### add(String name, boolean value) {#add-java.lang.String-boolean-}
```
public final CustomProjectProperty add(String name, boolean value)
```


새 사용자 정의 속성을 생성합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| name | java.lang.String | 속성의 이름입니다. |
| 값 | boolean | 새로 생성된 속성 객체의 값입니다. |

**Returns:**
[CustomProjectProperty](../../com.aspose.tasks/customprojectproperty) - The newly created property object.
### add(String name, double value) {#add-java.lang.String-double-}
```
public final CustomProjectProperty add(String name, double value)
```


새 사용자 정의 속성을 생성합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| name | java.lang.String | 속성의 이름입니다. |
| 값 | double | 새로 생성된 속성 객체의 값입니다. |

**Returns:**
[CustomProjectProperty](../../com.aspose.tasks/customprojectproperty) - The newly created property object.
### add(String name, String value) {#add-java.lang.String-java.lang.String-}
```
public final CustomProjectProperty add(String name, String value)
```


새 사용자 정의 속성을 생성합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| name | java.lang.String | 속성의 이름입니다. |
| 값 | java.lang.String | 새로 생성된 속성 객체의 값입니다. |

**Returns:**
[CustomProjectProperty](../../com.aspose.tasks/customprojectproperty) - The newly created property object.
### add(String name, Date value) {#add-java.lang.String-java.util.Date-}
```
public final CustomProjectProperty add(String name, Date value)
```


새 사용자 정의 속성을 생성합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| name | java.lang.String | 속성의 이름입니다. |
| 값 | java.util.Date | 새로 생성된 속성 객체의 값입니다. |

**Returns:**
[CustomProjectProperty](../../com.aspose.tasks/customprojectproperty) - The newly created property object.
### clear() {#clear--}
```
public final void clear()
```


PropertyCollection를 비웁니다.

### isReadOnly() {#isReadOnly--}
```
public boolean isReadOnly()
```


이 컬렉션이 읽기 전용인지 여부를 나타내는 값을 가져옵니다; 그렇지 않으면 false.

**Returns:**
boolean - 이 컬렉션이 읽기 전용인지 여부를 나타내는 값; 그렇지 않으면 false.
### remove(String name) {#remove-java.lang.String-}
```
public final boolean remove(String name)
```


지정된 이름을 가진 속성을 컬렉션에서 제거합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| name | java.lang.String | 속성의 대소문자를 구분하지 않는 이름입니다. |

**Returns:**
boolean - 요소가 성공적으로 찾아져 제거되면 true; 그렇지 않으면 false.
