---
title: "베이스라인"
second_title: "Aspose.Tasks for Java API Reference"
description: "리소스의 기준값을 나타냅니다."
type: docs
weight: 26
url: /ko/java/com.aspose.tasks/baseline/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Comparable, com.aspose.ms.System.IEquatable
```
public class Baseline implements Comparable<Baseline>, System.IEquatable<Baseline>
```

리소스의 기준값을 나타냅니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [Baseline()](#Baseline--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [compareTo(Baseline other)](#compareTo-com.aspose.tasks.Baseline-) | IComparable 인터페이스 구현. |
| [equals(Baseline other)](#equals-com.aspose.tasks.Baseline-) | 이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다. |
| [equals(Object obj)](#equals-java.lang.Object-) | 이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다. |
| [getBaselineNumber()](#getBaselineNumber--) | 베이스라인 데이터 레코드의 고유 번호를 가져옵니다. |
| [getBcwp()](#getBcwp--) | 리소스가 프로젝트에서 수행한 작업의 현재까지 예산 비용을 가져옵니다. |
| [getBcws()](#getBcws--) | 리소스에 예정된 작업의 예산 비용을 가져옵니다. |
| [getCost()](#getCost--) | 베이스라인이 저장될 때 리소스의 예상 비용을 가져옵니다. |
| [getWork()](#getWork--) | 베이스라인이 저장될 때 리소스에 할당된 작업을 가져옵니다. |
| [hashCode()](#hashCode--) | 베이스라인에 대한 해시 코드 값을 반환합니다. |
| [op_Equality(Baseline a, Baseline b)](#op-Equality-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | 이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다. |
| [op_GreaterThan(Baseline a, Baseline b)](#op-GreaterThan-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | 이 인스턴스가 지정된 객체보다 큰지 여부를 나타내는 값을 반환합니다. |
| [op_GreaterThanOrEqual(Baseline a, Baseline b)](#op-GreaterThanOrEqual-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | 이 인스턴스가 지정된 객체보다 크거나 같은지 여부를 나타내는 값을 반환합니다. |
| [op_Inequality(Baseline a, Baseline b)](#op-Inequality-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | 이 인스턴스가 지정된 객체와 같지 않은지 여부를 나타내는 값을 반환합니다. |
| [op_LessThan(Baseline a, Baseline b)](#op-LessThan-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | 이 인스턴스가 지정된 객체보다 작은지 여부를 나타내는 값을 반환합니다. |
| [op_LessThanOrEqual(Baseline a, Baseline b)](#op-LessThanOrEqual-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | 이 인스턴스가 지정된 객체보다 작거나 같은지 여부를 나타내는 값을 반환합니다. |
| [setBaselineNumber(int value)](#setBaselineNumber-int-) | 베이스라인 데이터 레코드의 고유 번호를 설정합니다. |
| [setBcwp(double value)](#setBcwp-double-) | 리소스가 프로젝트에서 수행한 작업의 현재까지 예산 비용을 설정합니다. |
| [setBcws(double value)](#setBcws-double-) | 리소스에 예정된 작업의 예산 비용을 설정합니다. |
| [setCost(BigDecimal value)](#setCost-java.math.BigDecimal-) | 베이스라인이 저장될 때 리소스의 예상 비용을 설정합니다. |
| [setWork(Duration value)](#setWork-com.aspose.tasks.Duration-) | 베이스라인이 저장될 때 리소스에 할당된 작업을 설정합니다. |
### Baseline() {#Baseline--}
```
public Baseline()
```


### compareTo(Baseline other) {#compareTo-com.aspose.tasks.Baseline-}
```
public final int compareTo(Baseline other)
```


IComparable 인터페이스 구현. 이 인스턴스를 지정된 Baseline 객체와 비교합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| other | [Baseline](../../com.aspose.tasks/baseline) | 이 인스턴스를 비교할 지정된 Baseline 객체. |

**Returns:**
int - 이 인스턴스가 지정된 객체보다 작으면 -1을 반환하고, 크면 1을 반환합니다; 그 외의 경우 0을 반환합니다.
### equals(Baseline other) {#equals-com.aspose.tasks.Baseline-}
```
public final boolean equals(Baseline other)
```


이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| other | [Baseline](../../com.aspose.tasks/baseline) | 이 인스턴스와 비교할 지정된 객체. |

**Returns:**
boolean - 이 인스턴스가 지정된 객체와 같으면 true를 반환하고, 그렇지 않으면 false를 반환합니다.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| obj | java.lang.Object | 이 인스턴스와 비교할 지정된 객체. |

**Returns:**
boolean - 이 인스턴스가 지정된 객체와 같으면 true를 반환하고, 그렇지 않으면 false를 반환합니다.
### getBaselineNumber() {#getBaselineNumber--}
```
public final int getBaselineNumber()
```


베이스라인 데이터 레코드의 고유 번호를 가져옵니다.

**Returns:**
int - 베이스라인 데이터 레코드의 고유 번호입니다.
### getBcwp() {#getBcwp--}
```
public final double getBcwp()
```


리소스가 프로젝트에서 수행한 작업의 현재까지 예산 비용을 가져옵니다.

**Returns:**
double - 리소스가 프로젝트를 위해 수행한 작업의 현재까지 예산 비용입니다.
### getBcws() {#getBcws--}
```
public final double getBcws()
```


리소스에 예정된 작업의 예산 비용을 가져옵니다.

**Returns:**
double - 리소스에 예정된 작업의 예산 비용입니다.
### getCost() {#getCost--}
```
public final BigDecimal getCost()
```


베이스라인이 저장될 때 리소스의 예상 비용을 가져옵니다.

**Returns:**
java.math.BigDecimal - 베이스라인이 저장될 때 리소스의 예상 비용입니다.
### getWork() {#getWork--}
```
public final Duration getWork()
```


베이스라인이 저장될 때 리소스에 할당된 작업을 가져옵니다.

값: 베이스라인이 저장될 때 리소스에 할당된 작업량입니다.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the work assigned to a resource when the baseline is saved.
### hashCode() {#hashCode--}
```
public int hashCode()
```


베이스라인에 대한 해시 코드 값을 반환합니다.

**Returns:**
int - 이 객체에 대한 해시 코드 값을 반환합니다.
### op_Equality(Baseline a, Baseline b) {#op-Equality-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_Equality(Baseline a, Baseline b)
```


이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | 첫 번째 베이스라인입니다. |
| b | [Baseline](../../com.aspose.tasks/baseline) | 두 번째 베이스라인입니다. |

**Returns:**
boolean - 이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값
### op_GreaterThan(Baseline a, Baseline b) {#op-GreaterThan-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_GreaterThan(Baseline a, Baseline b)
```


이 인스턴스가 지정된 객체보다 큰지 여부를 나타내는 값을 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | 첫 번째 베이스라인입니다. |
| b | [Baseline](../../com.aspose.tasks/baseline) | 두 번째 베이스라인입니다. |

**Returns:**
boolean - 이 인스턴스가 지정된 객체보다 큰지 여부를 나타내는 값
### op_GreaterThanOrEqual(Baseline a, Baseline b) {#op-GreaterThanOrEqual-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_GreaterThanOrEqual(Baseline a, Baseline b)
```


이 인스턴스가 지정된 객체보다 크거나 같은지 여부를 나타내는 값을 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | 첫 번째 베이스라인입니다. |
| b | [Baseline](../../com.aspose.tasks/baseline) | 두 번째 베이스라인입니다. |

**Returns:**
boolean - 이 인스턴스가 지정된 객체보다 크거나 같은지 여부를 나타내는 값
### op_Inequality(Baseline a, Baseline b) {#op-Inequality-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_Inequality(Baseline a, Baseline b)
```


이 인스턴스가 지정된 객체와 같지 않은지 여부를 나타내는 값을 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | 첫 번째 베이스라인입니다. |
| b | [Baseline](../../com.aspose.tasks/baseline) | 두 번째 베이스라인입니다. |

**Returns:**
boolean - 이 인스턴스가 지정된 객체와 같지 않은지 여부를 나타내는 값
### op_LessThan(Baseline a, Baseline b) {#op-LessThan-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_LessThan(Baseline a, Baseline b)
```


이 인스턴스가 지정된 객체보다 작은지 여부를 나타내는 값을 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | 첫 번째 베이스라인입니다. |
| b | [Baseline](../../com.aspose.tasks/baseline) | 두 번째 베이스라인입니다. |

**Returns:**
boolean - 이 인스턴스가 지정된 객체보다 작은지 여부를 나타내는 값
### op_LessThanOrEqual(Baseline a, Baseline b) {#op-LessThanOrEqual-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_LessThanOrEqual(Baseline a, Baseline b)
```


이 인스턴스가 지정된 객체보다 작거나 같은지 여부를 나타내는 값을 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | 첫 번째 베이스라인입니다. |
| b | [Baseline](../../com.aspose.tasks/baseline) | 두 번째 베이스라인입니다. |

**Returns:**
boolean - 이 인스턴스가 지정된 객체보다 작거나 같은지 여부를 나타내는 값
### setBaselineNumber(int value) {#setBaselineNumber-int-}
```
public final void setBaselineNumber(int value)
```


베이스라인 데이터 레코드의 고유 번호를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 베이스라인 데이터 레코드의 고유 번호입니다. |

### setBcwp(double value) {#setBcwp-double-}
```
public final void setBcwp(double value)
```


리소스가 프로젝트에서 수행한 작업의 현재까지 예산 비용을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | double | 리소스가 프로젝트를 위해 수행한 작업의 현재까지 예산 비용입니다. |

### setBcws(double value) {#setBcws-double-}
```
public final void setBcws(double value)
```


리소스에 예정된 작업의 예산 비용을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | double | 리소스에 예정된 작업의 예산 비용입니다. |

### setCost(BigDecimal value) {#setCost-java.math.BigDecimal-}
```
public final void setCost(BigDecimal value)
```


베이스라인이 저장될 때 리소스의 예상 비용을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.math.BigDecimal | 베이스라인이 저장될 때 리소스의 예상 비용입니다. |

### setWork(Duration value) {#setWork-com.aspose.tasks.Duration-}
```
public final void setWork(Duration value)
```


베이스라인이 저장될 때 리소스에 할당된 작업을 설정합니다.

값: 베이스라인이 저장될 때 리소스에 할당된 작업량입니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | 베이스라인이 저장될 때 리소스에 할당된 작업입니다. |

