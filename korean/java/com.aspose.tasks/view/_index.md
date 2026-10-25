---
title: "View"
second_title: "Aspose.Tasks for Java API Reference"
description: "Project에서 보기를 나타냅니다."
type: docs
weight: 342
url: /ko/java/com.aspose.tasks/view/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Comparable
```
public class View implements Comparable<View>
```

Project에서 보기를 나타냅니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [View()](#View--) | 새 인스턴스를 초기화합니다 [View](../../com.aspose/tasks/view) 클래스. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [compareTo(View other)](#compareTo-com.aspose.tasks.View-) | 현재 인스턴스를 동일한 유형의 다른 객체와 비교하고 정렬 순서에서 현재 인스턴스가 앞선, 뒤따른 또는 같은 위치에 있는지를 나타내는 정수를 반환합니다. |
| [equals(Object obj)](#equals-java.lang.Object-) | 이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다. |
| [forViewScreen(int viewScreen)](#forViewScreen-int-) | 새 인스턴스를 생성합니다 [View](../../com.aspose/tasks/view) 클래스. |
| [getFilter()](#getFilter--) | 단일 보기에서 사용되는 필터를 가져옵니다. |
| [getGroup()](#getGroup--) | 단일 보기의 그룹을 가져옵니다. |
| [getHighlightFilter()](#getHighlightFilter--) | Microsoft Project가 단일 보기의 필터를 강조 표시하는지 여부를 나타내는 값을 가져옵니다. |
| [getName()](#getName--) | View 객체의 이름을 가져옵니다. |
| [getPageInfo()](#getPageInfo--) | `PageInfo`([getPageInfo()](../../com.aspose.tasks/view\#getPageInfo--)) 클래스의 인스턴스를 가져옵니다. |
| [getParentProject()](#getParentProject--) | View 객체의 부모를 가져옵니다. |
| [getScreen()](#getScreen--) | 단일 보기의 화면 유형을 가져옵니다. |
| [getShowInMenu()](#getShowInMenu--) | Microsoft Project가 리본의 View 또는 Other Views 드롭다운 목록에 단일 보기 이름을 표시하는지 여부를 나타내는 값을 가져옵니다. |
| [getTable()](#getTable--) | 단일 보기의 테이블을 가져옵니다. |
| [getType()](#getType--) | 작업 또는 리소스와 같은 단일 보기의 항목 유형을 가져옵니다. |
| [getUid()](#getUid--) | 보기의 고유 식별자를 가져옵니다. |
| [getVisualObjectsPlacements()](#getVisualObjectsPlacements--) | 보기에서 [OleObject](../../com.aspose.tasks/oleobject)의 배치 및 모양을 나타내는 객체 컬렉션을 가져옵니다. |
| [hashCode()](#hashCode--) | [Resource](../../com.aspose.tasks/resource) 클래스 인스턴스에 대한 해시 코드 값을 반환합니다. |
| [op_Equality(View a, View b)](#op-Equality-com.aspose.tasks.View-com.aspose.tasks.View-) | 이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다. |
| [op_GreaterThan(View a, View b)](#op-GreaterThan-com.aspose.tasks.View-com.aspose.tasks.View-) | 이 인스턴스가 지정된 객체보다 큰지 여부를 나타내는 값을 반환합니다. |
| [op_GreaterThanOrEqual(View a, View b)](#op-GreaterThanOrEqual-com.aspose.tasks.View-com.aspose.tasks.View-) | 이 인스턴스가 지정된 객체보다 크거나 같은지 여부를 나타내는 값을 반환합니다. |
| [op_Inequality(View a, View b)](#op-Inequality-com.aspose.tasks.View-com.aspose.tasks.View-) | 이 인스턴스가 지정된 객체와 같지 않은지 여부를 나타내는 값을 반환합니다. |
| [op_LessThan(View a, View b)](#op-LessThan-com.aspose.tasks.View-com.aspose.tasks.View-) | 이 인스턴스가 지정된 객체보다 작은지 여부를 나타내는 값을 반환합니다. |
| [op_LessThanOrEqual(View a, View b)](#op-LessThanOrEqual-com.aspose.tasks.View-com.aspose.tasks.View-) | 이 인스턴스가 지정된 객체보다 작거나 같은지 여부를 나타내는 값을 반환합니다. |
| [setFilter(Filter value)](#setFilter-com.aspose.tasks.Filter-) | 단일 보기에서 사용되는 필터를 설정합니다. |
| [setGroup(Group value)](#setGroup-com.aspose.tasks.Group-) | 단일 보기의 그룹을 설정합니다. |
| [setHighlightFilter(boolean value)](#setHighlightFilter-boolean-) | Microsoft Project가 단일 보기의 필터를 강조 표시하는지 여부를 나타내는 값을 설정합니다. |
| [setName(String value)](#setName-java.lang.String-) | View 객체의 이름을 설정합니다. |
| [setShowInMenu(boolean value)](#setShowInMenu-boolean-) | Microsoft Project가 리본의 View 또는 Other Views 드롭다운 목록에 단일 보기 이름을 표시하는지 여부를 나타내는 값을 설정합니다. |
| [setTable(Table value)](#setTable-com.aspose.tasks.Table-) | 단일 보기의 테이블을 설정합니다. |
### View() {#View--}
```
public View()
```


새 인스턴스를 초기화합니다 [View](../../com.aspose/tasks/view) 클래스.

### compareTo(View other) {#compareTo-com.aspose.tasks.View-}
```
public final int compareTo(View other)
```


현재 인스턴스를 동일한 유형의 다른 객체와 비교하고 정렬 순서에서 현재 인스턴스가 앞선, 뒤따른 또는 같은 위치에 있는지를 나타내는 정수를 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| other | [View](../../com.aspose.tasks/view) | 이 인스턴스를 비교할 지정된 View 객체. |

**Returns:**
int - 비교되는 객체들의 상대 순서를 나타내는 32비트 부호 있는 정수입니다. 반환 값은 다음과 같은 의미를 가집니다: 값 의미 0보다 작음 이 인스턴스는 정렬 순서에서 `other`보다 앞에 있습니다. 0 이 인스턴스는 `other`와 동일한 위치에 있습니다. 0보다 큼 이 인스턴스는 정렬 순서에서 `other`보다 뒤에 있습니다.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| obj | java.lang.Object | 이 인스턴스와 비교할 객체입니다. |

**Returns:**
boolean - 지정된 객체가 이 인스턴스와 동일한 Uid 값을 가진 View인 경우 **True**, 그렇지 않으면 **false**.
### forViewScreen(int viewScreen) {#forViewScreen-int-}
```
public static View forViewScreen(int viewScreen)
```


새 인스턴스를 생성합니다 [View](../../com.aspose/tasks/view) 클래스.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| viewScreen | int | 뷰를 표시할 수 있는 화면 유형. |

**Returns:**
[View](../../com.aspose.tasks/view) - Constructed view.
### getFilter() {#getFilter--}
```
public final Filter getFilter()
```


단일 보기에서 사용되는 필터를 가져옵니다.

**Returns:**
[Filter](../../com.aspose.tasks/filter) - a filter used in a single view.
### getGroup() {#getGroup--}
```
public final Group getGroup()
```


단일 보기의 그룹을 가져옵니다.

**Returns:**
[Group](../../com.aspose.tasks/group) - a group of the single view.
### getHighlightFilter() {#getHighlightFilter--}
```
public final boolean getHighlightFilter()
```


Microsoft Project가 단일 보기의 필터를 강조 표시하는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - 단일 뷰에 대한 필터를 Microsoft Project가 강조 표시하는지 여부를 나타내는 값.
### getName() {#getName--}
```
public final String getName()
```


View 객체의 이름을 가져옵니다.

**Returns:**
java.lang.String - View 객체의 이름.
### getPageInfo() {#getPageInfo--}
```
public final PageInfo getPageInfo()
```


`PageInfo`([getPageInfo()](../../com.aspose.tasks/view\#getPageInfo--)) 클래스의 인스턴스를 가져옵니다. mpp 파일 형식에 존재하는 페이지 설정 데이터를 나타냅니다.

**Returns:**
[PageInfo](../../com.aspose.tasks/pageinfo) - an instance of the `PageInfo`([getPageInfo()](../../com.aspose.tasks/view\#getPageInfo--)) class.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


View 객체의 상위 항목을 가져옵니다. 읽기 전용 [Project](../../com.aspose.tasks/project).

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent of the View object.
### getScreen() {#getScreen--}
```
public final int getScreen()
```


단일 뷰의 화면 유형을 가져옵니다. 읽기 전용 [ViewScreen](../../com.aspose.tasks/viewscreen).

**Returns:**
int - 단일 뷰의 화면 유형.
### getShowInMenu() {#getShowInMenu--}
```
public final boolean getShowInMenu()
```


Microsoft Project가 리본의 View 또는 Other Views 드롭다운 목록에 단일 보기 이름을 표시하는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - Microsoft Project가 리본의 View 또는 Other Views 드롭다운 목록에 단일 뷰 이름을 표시하는지 여부를 나타내는 값.
### getTable() {#getTable--}
```
public final Table getTable()
```


단일 보기의 테이블을 가져옵니다.

**Returns:**
[Table](../../com.aspose.tasks/table) - a table of the single view.
### getType() {#getType--}
```
public final int getType()
```


단일 뷰의 항목 유형(예: 작업 또는 리소스)을 가져옵니다. 읽기 전용 [ItemType](../../com.aspose.tasks/itemtype).

**Returns:**
int - 단일 뷰의 항목 유형(예: 작업 또는 리소스).
### getUid() {#getUid--}
```
public final int getUid()
```


보기의 고유 식별자를 가져옵니다.

**Returns:**
int - 뷰의 고유 식별자.
### getVisualObjectsPlacements() {#getVisualObjectsPlacements--}
```
public final List<VisualObjectPlacement> getVisualObjectsPlacements()
```


보기에서 [OleObject](../../com.aspose.tasks/oleobject)의 배치 및 모양을 나타내는 객체 컬렉션을 가져옵니다.

**Returns:**
java.util.List&lt;com.aspose.tasks.VisualObjectPlacement&gt; - 뷰 내에서 [OleObject](../../com.aspose.tasks/oleobject)의 배치 및 모양을 나타내는 객체 컬렉션.
### hashCode() {#hashCode--}
```
public int hashCode()
```


[Resource](../../com.aspose.tasks/resource) 클래스 인스턴스에 대한 해시 코드 값을 반환합니다.

**Returns:**
int - 이 객체에 대한 해시 코드 값을 반환합니다.
### op_Equality(View a, View b) {#op-Equality-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_Equality(View a, View b)
```


이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | 첫 번째 뷰. |
| b | [View](../../com.aspose.tasks/view) | 두 번째 뷰. |

**Returns:**
boolean - 이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값
### op_GreaterThan(View a, View b) {#op-GreaterThan-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_GreaterThan(View a, View b)
```


이 인스턴스가 지정된 객체보다 큰지 여부를 나타내는 값을 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | 첫 번째 뷰. |
| b | [View](../../com.aspose.tasks/view) | 두 번째 뷰. |

**Returns:**
boolean - 이 인스턴스가 지정된 객체보다 큰지 여부를 나타내는 값
### op_GreaterThanOrEqual(View a, View b) {#op-GreaterThanOrEqual-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_GreaterThanOrEqual(View a, View b)
```


이 인스턴스가 지정된 객체보다 크거나 같은지 여부를 나타내는 값을 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | 첫 번째 뷰. |
| b | [View](../../com.aspose.tasks/view) | 두 번째 뷰. |

**Returns:**
boolean - 이 인스턴스가 지정된 객체보다 크거나 같은지 여부를 나타내는 값
### op_Inequality(View a, View b) {#op-Inequality-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_Inequality(View a, View b)
```


이 인스턴스가 지정된 객체와 같지 않은지 여부를 나타내는 값을 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | 첫 번째 뷰. |
| b | [View](../../com.aspose.tasks/view) | 두 번째 뷰. |

**Returns:**
boolean - 이 인스턴스가 지정된 객체와 같지 않은지 여부를 나타내는 값
### op_LessThan(View a, View b) {#op-LessThan-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_LessThan(View a, View b)
```


이 인스턴스가 지정된 객체보다 작은지 여부를 나타내는 값을 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | 첫 번째 필터. |
| b | [View](../../com.aspose.tasks/view) | 두 번째 필터. |

**Returns:**
boolean - 이 인스턴스가 지정된 객체보다 작은지 여부를 나타내는 값
### op_LessThanOrEqual(View a, View b) {#op-LessThanOrEqual-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_LessThanOrEqual(View a, View b)
```


이 인스턴스가 지정된 객체보다 작거나 같은지 여부를 나타내는 값을 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | 첫 번째 뷰. |
| b | [View](../../com.aspose.tasks/view) | 두 번째 뷰. |

**Returns:**
boolean - 이 인스턴스가 지정된 객체보다 작거나 같은지 여부를 나타내는 값
### setFilter(Filter value) {#setFilter-com.aspose.tasks.Filter-}
```
public final void setFilter(Filter value)
```


단일 보기에서 사용되는 필터를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [Filter](../../com.aspose.tasks/filter) | 단일 뷰에서 사용되는 필터. |

### setGroup(Group value) {#setGroup-com.aspose.tasks.Group-}
```
public final void setGroup(Group value)
```


단일 보기의 그룹을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [Group](../../com.aspose.tasks/group) | 단일 뷰의 그룹. |

### setHighlightFilter(boolean value) {#setHighlightFilter-boolean-}
```
public final void setHighlightFilter(boolean value)
```


Microsoft Project가 단일 보기의 필터를 강조 표시하는지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | Microsoft Project가 단일 뷰에 대한 필터를 강조 표시하는지 여부를 나타내는 값. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


View 객체의 이름을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | View 객체의 이름. |

### setShowInMenu(boolean value) {#setShowInMenu-boolean-}
```
public final void setShowInMenu(boolean value)
```


Microsoft Project가 리본의 View 또는 Other Views 드롭다운 목록에 단일 보기 이름을 표시하는지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | Microsoft Project가 리본의 View 또는 Other Views 드롭다운 목록에 단일 뷰 이름을 표시하는지 여부를 나타내는 값. |

### setTable(Table value) {#setTable-com.aspose.tasks.Table-}
```
public final void setTable(Table value)
```


단일 보기의 테이블을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [Table](../../com.aspose.tasks/table) | 단일 뷰의 테이블. |

