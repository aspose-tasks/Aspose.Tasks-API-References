---
title: "ResourceViewColumn"
second_title: "Aspose.Tasks for Java API Reference"
description: "ResourceUsage 보기와 ResourceSheet 보기에서 사용되는 Projects 보기 클래스."
type: docs
weight: 261
url: /ko/java/com.aspose.tasks/resourceviewcolumn/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.ViewColumn](../../com.aspose.tasks/viewcolumn)
```
public final class ResourceViewColumn extends ViewColumn
```

ResourceUsage 보기와 ResourceSheet 보기에서 사용되는 프로젝트 보기 클래스를 나타냅니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter, int field)](#ResourceViewColumn-java.lang.String-int-com.aspose.tasks.ResourceToColumnTextConverter-int-) | [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn) 클래스의 새 인스턴스를 초기화합니다. |
| [ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter)](#ResourceViewColumn-java.lang.String-int-com.aspose.tasks.ResourceToColumnTextConverter-) | [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn) 클래스의 새 인스턴스를 초기화합니다. |
| [ResourceViewColumn(int width, int field)](#ResourceViewColumn-int-int-) | [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn) 클래스의 새 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getColumnText(Resource resource)](#getColumnText-com.aspose.tasks.Resource-) | 현재 리소스를 열 텍스트로 변환합니다. |
| [getField()](#getField--) | 열 필드를 반환합니다. |
| [setField(int value)](#setField-int-) | 열 필드를 설정합니다. |
### ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter, int field) {#ResourceViewColumn-java.lang.String-int-com.aspose.tasks.ResourceToColumnTextConverter-int-}
```
public ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter, int field)
```


[ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn) 클래스의 새 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| name | java.lang.String | 열 이름입니다. |
| width | int | 열의 너비(픽셀 단위)입니다. |
| converter | [ResourceToColumnTextConverter](../../com.aspose.tasks/resourcetocolumntextconverter) | 리소스 데이터를 열 텍스트로 변환하는 변환기. |
| 필드 | int | 열 필드. |

### ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter) {#ResourceViewColumn-java.lang.String-int-com.aspose.tasks.ResourceToColumnTextConverter-}
```
public ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter)
```


[ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn) 클래스의 새 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| name | java.lang.String | 열 이름입니다. |
| width | int | 열의 너비(픽셀 단위)입니다. |
| converter | [ResourceToColumnTextConverter](../../com.aspose.tasks/resourcetocolumntextconverter) | 리소스 데이터를 열 텍스트로 변환하는 변환기. |

### ResourceViewColumn(int width, int field) {#ResourceViewColumn-int-int-}
```
public ResourceViewColumn(int width, int field)
```


[ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn) 클래스의 새 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| width | int | 픽셀 단위의 열 너비. |
| 필드 | int | 열 필드. |

### getColumnText(Resource resource) {#getColumnText-com.aspose.tasks.Resource-}
```
public final String getColumnText(Resource resource)
```


현재 리소스를 열 텍스트로 변환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| resource | [Resource](../../com.aspose.tasks/resource) | 현재 리소스. |

**Returns:**
java.lang.String - 열 텍스트.
### getField() {#getField--}
```
public int getField()
```


열 필드를 반환합니다. `Field`.

**Returns:**
int - 열 필드 값.
### setField(int value) {#setField-int-}
```
public void setField(int value)
```


열 필드를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 열 필드 값. |

