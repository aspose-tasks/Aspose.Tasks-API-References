---
title: "SplitPartCollection"
second_title: "Aspose.Tasks for Java API Reference"
description: "작업의 부분을 나타내는 컬렉션입니다."
type: docs
weight: 279
url: /ko/java/com.aspose.tasks/splitpartcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class SplitPartCollection extends AbstractList<SplitPart>
```

작업의 부분을 나타내는 컬렉션입니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [get(int index)](#get-int-) | 주어진 인덱스에서 작업의 분할 부분을 검색합니다. |
| [set(int index, SplitPart value)](#set-int-com.aspose.tasks.SplitPart-) | 주어진 인덱스에서 작업의 분할 부분을 설정합니다. |
| [size()](#size--) | 컬렉션에 있는 부분의 수를 가져옵니다. |
| [toArray()](#toArray--) | 컬렉션의 모든 부분을 새 배열로 복사합니다. |
### get(int index) {#get-int-}
```
public final SplitPart get(int index)
```


주어진 인덱스에서 작업의 분할 부분을 검색합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | index | int | 부분 인덱스. |

--------------------

인덱스는 0부터 시작합니다. 인덱스가 배열 범위를 벗어나면 null을 반환합니다. |

**Returns:**
[SplitPart](../../com.aspose.tasks/splitpart) - a split part.
### set(int index, SplitPart value) {#set-int-com.aspose.tasks.SplitPart-}
```
public final SplitPart set(int index, SplitPart value)
```


주어진 인덱스에서 작업의 분할 부분을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | index | int | 부분 인덱스. |

--------------------

인덱스는 0부터 시작합니다. 인덱스가 배열 범위를 벗어나면 null을 반환합니다. |
| value | [SplitPart](../../com.aspose.tasks/splitpart) | 설정할 분할 부분. |

**Returns:**
[SplitPart](../../com.aspose.tasks/splitpart) - a split part.
### size() {#size--}
```
public final int size()
```


컬렉션에 있는 부분의 수를 가져옵니다.

**Returns:**
int - 컬렉션에 포함된 파트 수.
### toArray() {#toArray--}
```
public final SplitPart[] toArray()
```


컬렉션의 모든 부분을 새 배열로 복사합니다.

**Returns:**
com.aspose.tasks.SplitPart[] - [SplitPart](../../com.aspose.tasks/splitpart) 객체 배열.
