---
title: "AssignmentViewColumn"
second_title: "Aspose.Tasks for Java API Reference"
description: "프로젝트 보기 클래스입니다."
type: docs
weight: 19
url: /ko/java/com.aspose.tasks/assignmentviewcolumn/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.ViewColumn](../../com.aspose.tasks/viewcolumn)
```
public class AssignmentViewColumn extends ViewColumn
```

프로젝트의 뷰 클래스.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [AssignmentViewColumn(String name, int width, AssignmentToColumnTextConverter converter)](#AssignmentViewColumn-java.lang.String-int-com.aspose.tasks.AssignmentToColumnTextConverter-) | AssignmentViewColumn 클래스의 새 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getColumnText(ResourceAssignment assignment)](#getColumnText-com.aspose.tasks.ResourceAssignment-) | 현재 리소스 할당을 열 텍스트로 변환합니다. |
| [getField()](#getField--) | 열 필드를 반환합니다. |
| [setField(int value)](#setField-int-) | 열 필드를 설정합니다. |
### AssignmentViewColumn(String name, int width, AssignmentToColumnTextConverter converter) {#AssignmentViewColumn-java.lang.String-int-com.aspose.tasks.AssignmentToColumnTextConverter-}
```
public AssignmentViewColumn(String name, int width, AssignmentToColumnTextConverter converter)
```


AssignmentViewColumn 클래스의 새 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| name | java.lang.String | 열 이름입니다. |
| width | int | 열의 너비(픽셀 단위)입니다. |
| converter | [AssignmentToColumnTextConverter](../../com.aspose.tasks/assignmenttocolumntextconverter) | 할당 데이터를 열 텍스트로 변환하는 변환기. |

### getColumnText(ResourceAssignment assignment) {#getColumnText-com.aspose.tasks.ResourceAssignment-}
```
public String getColumnText(ResourceAssignment assignment)
```


현재 리소스 할당을 열 텍스트로 변환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| assignment | [ResourceAssignment](../../com.aspose.tasks/resourceassignment) | 현재 할당입니다. |

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

