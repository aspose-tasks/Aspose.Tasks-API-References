---
title: "GenericProperty"
second_title: "Aspose.Tasks for Java API Reference"
description: "컨테이너 속성을 나타냅니다."
type: docs
weight: 113
url: /ko/java/com.aspose.tasks/genericproperty/
---

**Inheritance:**
java.lang.Object
```
public class GenericProperty<TKey>
```

컨테이너 속성을 나타냅니다.

TKey : 속성 값의 유형.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [GenericProperty()](#GenericProperty--) | GenericProperty&lt;T&gt; 클래스의 새 인스턴스를 초기화합니다. |
| [GenericProperty(Class&lt;TKey&gt; typeOfTKey, String name)](#GenericProperty-java.lang.Class-TKey--java.lang.String-) | GenericProperty&lt;TKey&gt; 구조체의 새 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [&lt;TKey&gt;equals(GenericProperty&lt;TKey&gt; obj1, GenericProperty&lt;TKey&gt; obj2)](#-TKey-equals-com.aspose.tasks.GenericProperty-TKey--com.aspose.tasks.GenericProperty-TKey--) | 지정된 `obj1` 인스턴스가 지정된 `obj2` 인스턴스와 같은지 여부를 나타내는 값을 반환합니다. |
| [Clone()](#Clone--) | 이 인스턴스의 깊은 복사본을 생성하고 반환합니다. |
| [CloneTo(GenericProperty&lt;TKey&gt; that)](#CloneTo-com.aspose.tasks.GenericProperty-TKey--) | 인스턴스를 다른 인스턴스로 깊게 복사합니다. |
| [clone()](#clone--) | \{@inheritDoc\} |
| [equals(Object obj)](#equals-java.lang.Object-) | \{@inheritDoc\} |
| [getName()](#getName--) | 속성의 이름을 가져옵니다. |
| [getValue()](#getValue--) | 속성의 값을 가져옵니다. |
### GenericProperty() {#GenericProperty--}
```
public GenericProperty()
```


GenericProperty&lt;T&gt; 클래스의 새 인스턴스를 초기화합니다.

### GenericProperty(Class&lt;TKey&gt; typeOfTKey, String name) {#GenericProperty-java.lang.Class-TKey--java.lang.String-}
```
public GenericProperty(Class<TKey> typeOfTKey, String name)
```


GenericProperty&lt;TKey&gt; 구조체의 새 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| typeOfTKey | java.lang.Class&lt;TKey&gt; |  |
| name | java.lang.String | 속성의 이름입니다. |

### &lt;TKey&gt;equals(GenericProperty&lt;TKey&gt; obj1, GenericProperty&lt;TKey&gt; obj2) {#-TKey-equals-com.aspose.tasks.GenericProperty-TKey--com.aspose.tasks.GenericProperty-TKey--}
```
public static boolean <TKey>equals(GenericProperty<TKey> obj1, GenericProperty<TKey> obj2)
```


지정된 `obj1` 인스턴스가 지정된 `obj2` 인스턴스와 같은지 여부를 나타내는 값을 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| obj1 | [GenericProperty](../../com.aspose.tasks/genericproperty) | 비교할 첫 번째 객체. |
| obj2 | [GenericProperty](../../com.aspose.tasks/genericproperty) | 비교할 두 번째 객체. |

**Returns:**
boolean - 지정된 `obj1` 인스턴스가 지정된 `obj2` 인스턴스와 같으면 true를 반환하고, 그렇지 않으면 false를 반환합니다.
### Clone() {#Clone--}
```
public GenericProperty<TKey> Clone()
```


이 인스턴스의 깊은 복사본을 생성하고 반환합니다.

**Returns:**
[GenericProperty](../../com.aspose.tasks/genericproperty) - a deep copy of this object.
### CloneTo(GenericProperty&lt;TKey&gt; that) {#CloneTo-com.aspose.tasks.GenericProperty-TKey--}
```
public void CloneTo(GenericProperty<TKey> that)
```


인스턴스를 다른 인스턴스로 깊게 복사합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| that | [GenericProperty](../../com.aspose.tasks/genericproperty) | 다른 인스턴스. |

### clone() {#clone--}
```
public Object clone()
```




**Returns:**
java.lang.Object - \{@inheritDoc\}
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```




**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| obj | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### getName() {#getName--}
```
public final String getName()
```


속성의 이름을 가져옵니다.

**Returns:**
java.lang.String - 속성의 이름.
### getValue() {#getValue--}
```
public final Object getValue()
```


속성의 값을 가져옵니다.

**Returns:**
java.lang.Object - 속성의 값.
