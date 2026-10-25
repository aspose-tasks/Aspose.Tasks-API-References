---
title: "OleObject"
second_title: "Aspose.Tasks for Java API Reference"
description: "MPP 파일의 간트 차트 보기로 삽입할 수 있는 OLE 객체를 나타냅니다."
type: docs
weight: 164
url: /ko/java/com.aspose.tasks/oleobject/
---

**Inheritance:**
java.lang.Object
```
public class OleObject
```

MPP 파일의 간트 차트 보기로 삽입할 수 있는 OLE 객체를 나타냅니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [OleObject()](#OleObject--) | [OleObject](../../com.aspose.tasks/oleobject) 클래스의 새 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getApplicationName()](#getApplicationName--) | 임베드된 객체를 열 때 사용할 애플리케이션 이름을 가져옵니다. |
| [getContent()](#getContent--) | 임베드된 파일 데이터를 가져옵니다; 데이터가 임베드되지 않은 경우 null입니다. |
| [getDisplayAsIcon()](#getDisplayAsIcon--) | OLE object를 아이콘으로 표시하거나 일반 그림으로 표시해야 함을 나타내는 플래그를 가져옵니다. |
| [getFileFormat()](#getFileFormat--) | 임베드된 객체의 파일 형식을 가져옵니다. |
| [getFullPath()](#getFullPath--) | 삽입된 객체의 전체 경로를 가져옵니다. |
| [getId()](#getId--) | 객체 ID를 가져옵니다. |
| [getLabel()](#getLabel--) | 삽입된 객체의 레이블을 가져옵니다. |
| [getLinked()](#getLinked--) | 프로젝트 파일이 실제 데이터가 저장된 링크 소스에 대한 링크만 포함하는지 여부를 나타내는 값을 가져옵니다. |
| [getName()](#getName--) | OLE object 인스턴스의 이름을 가져옵니다. |
| [getTemporaryFile()](#getTemporaryFile--) | 삽입된 객체의 임시 파일 경로를 가져옵니다. |
| [getView()](#getView--) | 삽입된 객체가 속한 `View`([getView()](../../com.aspose.tasks/oleobject\#getView--)/[setView(View)](../../com.aspose.tasks/oleobject\#setView-View-)) 클래스의 인스턴스를 가져옵니다. |
| [setApplicationName(String value)](#setApplicationName-java.lang.String-) | 임베드된 객체를 열 때 사용할 애플리케이션 이름을 설정합니다. |
| [setContent(byte[] value)](#setContent-byte---) | 임베드된 파일 데이터를 설정합니다; 데이터가 임베드되지 않은 경우 null입니다. |
| [setDisplayAsIcon(boolean value)](#setDisplayAsIcon-boolean-) | OLE object를 아이콘으로 표시하거나 일반 그림으로 표시해야 함을 나타내는 플래그를 설정합니다. |
| [setFileFormat(String value)](#setFileFormat-java.lang.String-) | 임베드된 객체의 파일 형식을 설정합니다. |
| [setFullPath(String value)](#setFullPath-java.lang.String-) | 삽입된 객체의 전체 경로를 설정합니다. |
| [setId(int value)](#setId-int-) | 객체 ID를 설정합니다. |
| [setLabel(String value)](#setLabel-java.lang.String-) | 삽입된 객체의 레이블을 설정합니다. |
| [setName(String value)](#setName-java.lang.String-) | OLE object 인스턴스의 이름을 설정합니다. |
| [setTemporaryFile(String value)](#setTemporaryFile-java.lang.String-) | 삽입된 객체의 임시 파일 경로를 설정합니다. |
| [setView(View value)](#setView-com.aspose.tasks.View-) | 삽입된 객체가 속한 `View`([getView()](../../com.aspose.tasks/oleobject\#getView--)/[setView(View)](../../com.aspose.tasks/oleobject\#setView-View-)) 클래스의 인스턴스를 설정합니다. |
### OleObject() {#OleObject--}
```
public OleObject()
```


[OleObject](../../com.aspose.tasks/oleobject) 클래스의 새 인스턴스를 초기화합니다.

### getApplicationName() {#getApplicationName--}
```
public final String getApplicationName()
```


임베드된 객체를 열 때 사용할 애플리케이션 이름을 가져옵니다.

**Returns:**
java.lang.String - 임베드된 객체를 열 때 사용할 애플리케이션 이름.
### getContent() {#getContent--}
```
public final byte[] getContent()
```


임베드된 파일 데이터를 가져옵니다; 데이터가 임베드되지 않은 경우 null입니다.

**Returns:**
byte[] - 임베드된 파일 데이터; 데이터가 임베드되지 않은 경우 null.
### getDisplayAsIcon() {#getDisplayAsIcon--}
```
public final boolean getDisplayAsIcon()
```


OLE object를 아이콘으로 표시하거나 일반 그림으로 표시해야 함을 나타내는 플래그를 가져옵니다.

**Returns:**
boolean - OLE object를 아이콘으로 표시하거나 일반 그림으로 표시해야 함을 나타내는 플래그.
### getFileFormat() {#getFileFormat--}
```
public final String getFileFormat()
```


임베드된 객체의 파일 형식을 가져옵니다.

**Returns:**
java.lang.String - 임베드된 객체의 파일 형식.
### getFullPath() {#getFullPath--}
```
public final String getFullPath()
```


삽입된 객체의 전체 경로를 가져옵니다.

**Returns:**
java.lang.String - 삽입된 객체의 전체 경로.
### getId() {#getId--}
```
public final int getId()
```


객체 ID를 가져옵니다.

**Returns:**
int - 객체 ID.
### getLabel() {#getLabel--}
```
public final String getLabel()
```


삽입된 객체의 레이블을 가져옵니다.

**Returns:**
java.lang.String - 삽입된 객체의 레이블.
### getLinked() {#getLinked--}
```
public final boolean getLinked()
```


프로젝트 파일이 실제 데이터가 저장된 링크 소스에 대한 링크만 포함하는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - 프로젝트 파일이 실제 데이터가 저장된 링크 소스에 대한 링크만 포함하는지 여부를 나타내는 값.
### getName() {#getName--}
```
public final String getName()
```


OLE object 인스턴스의 이름을 가져옵니다.

**Returns:**
java.lang.String - OLE 객체 인스턴스의 이름.
### getTemporaryFile() {#getTemporaryFile--}
```
public final String getTemporaryFile()
```


삽입된 객체의 임시 파일 경로를 가져옵니다.

**Returns:**
java.lang.String - 삽입된 객체의 임시 파일 경로.
### getView() {#getView--}
```
public final View getView()
```


삽입된 객체가 속한 `View`([getView()](../../com.aspose.tasks/oleobject\#getView--)/[setView(View)](../../com.aspose.tasks/oleobject\#setView-View-)) 클래스의 인스턴스를 가져옵니다.

**Returns:**
[View](../../com.aspose.tasks/view) - the instance of the `View`([getView()](../../com.aspose.tasks/oleobject\#getView--)/[setView(View)](../../com.aspose.tasks/oleobject\#setView-View-)) class the inserted object belongs to.
### setApplicationName(String value) {#setApplicationName-java.lang.String-}
```
public final void setApplicationName(String value)
```


임베드된 객체를 열 때 사용할 애플리케이션 이름을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | 임베디드 객체를 열 때 사용할 애플리케이션 이름. |

### setContent(byte[] value) {#setContent-byte---}
```
public final void setContent(byte[] value)
```


임베드된 파일 데이터를 설정합니다; 데이터가 임베드되지 않은 경우 null입니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | byte[] | 임베디드 파일 데이터; 데이터가 임베드되지 않은 경우 null. |

### setDisplayAsIcon(boolean value) {#setDisplayAsIcon-boolean-}
```
public final void setDisplayAsIcon(boolean value)
```


OLE object를 아이콘으로 표시하거나 일반 그림으로 표시해야 함을 나타내는 플래그를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | OLE 객체를 아이콘으로 표시할지 일반 그림으로 표시할지 나타내는 플래그. |

### setFileFormat(String value) {#setFileFormat-java.lang.String-}
```
public final void setFileFormat(String value)
```


임베드된 객체의 파일 형식을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | 임베디드 객체의 파일 형식. |

### setFullPath(String value) {#setFullPath-java.lang.String-}
```
public final void setFullPath(String value)
```


삽입된 객체의 전체 경로를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | 삽입된 객체의 전체 경로. |

### setId(int value) {#setId-int-}
```
public final void setId(int value)
```


객체 ID를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 객체 ID. |

### setLabel(String value) {#setLabel-java.lang.String-}
```
public final void setLabel(String value)
```


삽입된 객체의 레이블을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | 삽입된 객체의 레이블. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


OLE object 인스턴스의 이름을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | OLE 객체 인스턴스의 이름. |

### setTemporaryFile(String value) {#setTemporaryFile-java.lang.String-}
```
public final void setTemporaryFile(String value)
```


삽입된 객체의 임시 파일 경로를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | 삽입된 객체의 임시 파일 경로. |

### setView(View value) {#setView-com.aspose.tasks.View-}
```
public final void setView(View value)
```


삽입된 객체가 속한 `View`([getView()](../../com.aspose.tasks/oleobject\#getView--)/[setView(View)](../../com.aspose.tasks/oleobject\#setView-View-)) 클래스의 인스턴스를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [View](../../com.aspose.tasks/view) | 삽입된 객체가 속한 `View`([getView()](../../com.aspose.tasks/oleobject\#getView--)/[setView(View)](../../com.aspose.tasks/oleobject\#setView-View-)) 클래스의 인스턴스. |

