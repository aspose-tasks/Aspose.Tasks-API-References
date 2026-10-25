---
title: "FieldHelper"
second_title: "Aspose.Tasks for Java API Reference"
description: "필드와 관련된 유용한 작업을 제공하는 도우미 클래스입니다."
type: docs
weight: 88
url: /ko/java/com.aspose.tasks/fieldhelper/
---

**Inheritance:**
java.lang.Object
```
public class FieldHelper
```

필드와 관련된 유용한 작업을 제공하는 도우미 클래스입니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [FieldHelper()](#FieldHelper--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getDefaultFieldTitle(int field)](#getDefaultFieldTitle-int-) | 특정 필드의 기본 제목을 반환합니다. |
| [getDefaultTaskFieldTitle(byte taskKey)](#getDefaultTaskFieldTitle-byte-) | 특정 작업 필드의 기본 제목을 반환합니다. |
### FieldHelper() {#FieldHelper--}
```
public FieldHelper()
```


### getDefaultFieldTitle(int field) {#getDefaultFieldTitle-int-}
```
public static String getDefaultFieldTitle(int field)
```


특정 필드의 기본 제목을 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 필드 | int | 기본 제목을 가져올 필드. |

**Returns:**
java.lang.String - 필드가 MS Project 보기에서 표시될 수 있는 경우 특정 필드의 기본 제목, 그렇지 않으면 null.
### getDefaultTaskFieldTitle(byte taskKey) {#getDefaultTaskFieldTitle-byte-}
```
public static String getDefaultTaskFieldTitle(byte taskKey)
```


특정 작업 필드의 기본 제목을 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| taskKey | 바이트 | 기본 제목을 가져올 작업 필드. |

**Returns:**
java.lang.String - 필드가 MS Project 보기에서 표시될 수 있는 경우 특정 작업 필드의 기본 제목, 그렇지 않으면 null.
