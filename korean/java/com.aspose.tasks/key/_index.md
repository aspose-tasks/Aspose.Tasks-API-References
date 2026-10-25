---
title: "키"
second_title: "Aspose.Tasks for Java API Reference"
description: "지정된 유형의 클래스에 대한 속성 키를 나타냅니다."
type: docs
weight: 139
url: /ko/java/com.aspose.tasks/key/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.lang.Struct
```
public class Key<T,K> extends Struct<Key<T,K>>
```

지정된 유형의 클래스에 대한 속성 키를 나타냅니다. 이 클래스의 인스턴스는 컨테이너의 속성을 가져오거나 설정할 때 사용됩니다.

T : 속성 값의 유형.
K : 속성 키의 유형.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [Clone()](#Clone--) | 인스턴스의 깊은 복사본을 반환합니다. |
| [CloneTo(Key&lt;T,K&gt; that)](#CloneTo-com.aspose.tasks.Key-T-K--) | 인스턴스를 다른 인스턴스로 깊게 복사합니다. |
| [clone()](#clone--) | \{@inheritDoc\} |
| [equals(Key obj1, Key obj2)](#equals-com.aspose.tasks.Key-com.aspose.tasks.Key-) | 지정된 `obj1` 인스턴스가 지정된 `obj2` 인스턴스와 같은지 여부를 나타내는 값을 반환합니다. |
| [equals(Object obj)](#equals-java.lang.Object-) | \{@inheritDoc\} |
| [getKeyType()](#getKeyType--) | 속성의 키를 가져옵니다. |
| [hashCode()](#hashCode--) | Key 클래스 인스턴스에 대한 해시 코드를 반환합니다. |
### Clone() {#Clone--}
```
public Key<T,K> Clone()
```


인스턴스의 깊은 복사본을 반환합니다.

**Returns:**
[Key](../../com.aspose.tasks/key) - deep copy of the instance.
### CloneTo(Key&lt;T,K&gt; that) {#CloneTo-com.aspose.tasks.Key-T-K--}
```
public void CloneTo(Key<T,K> that)
```


인스턴스를 다른 인스턴스로 깊게 복사합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| that | [Key](../../com.aspose.tasks/key) | 다른 인스턴스. |

### clone() {#clone--}
```
public Object clone()
```




**Returns:**
java.lang.Object - \{@inheritDoc\}
### equals(Key obj1, Key obj2) {#equals-com.aspose.tasks.Key-com.aspose.tasks.Key-}
```
public static boolean equals(Key obj1, Key obj2)
```


지정된 `obj1` 인스턴스가 지정된 `obj2` 인스턴스와 같은지 여부를 나타내는 값을 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| obj1 | com.aspose.tasks.Key | 비교할 첫 번째 객체. |
| obj2 | com.aspose.tasks.Key | 비교할 두 번째 객체. |

**Returns:**
boolean - 지정된 `obj1` 인스턴스가 지정된 `obj2` 인스턴스와 같으면 true를 반환하고, 그렇지 않으면 false를 반환합니다.
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
### getKeyType() {#getKeyType--}
```
public final K getKeyType()
```


속성의 키를 가져옵니다.

**Returns:**
K - 속성의 키.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Key 클래스 인스턴스에 대한 해시 코드를 반환합니다.

**Returns:**
int - 이 객체에 대한 해시 코드를 반환합니다.
