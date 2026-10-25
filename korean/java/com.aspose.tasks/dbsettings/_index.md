---
title: "DbSettings"
second_title: "Aspose.Tasks for Java API Reference"
description: "프로젝트 데이터베이스에서 읽기 위한 설정을 지정할 수 있습니다."
type: docs
weight: 75
url: /ko/java/com.aspose.tasks/dbsettings/
---

**Inheritance:**
java.lang.Object
```
public abstract class DbSettings
```

프로젝트 데이터베이스에서 읽기 위한 설정을 지정할 수 있습니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getConnectionString()](#getConnectionString--) | 연결 문자열을 가져옵니다. |
| [getDriverClassName()](#getDriverClassName--) | JDBC 드라이버 클래스의 이름을 반환합니다. |
| [setConnectionString(String value)](#setConnectionString-java.lang.String-) | 연결 문자열을 설정합니다. |
| [setDriverClassName(String value)](#setDriverClassName-java.lang.String-) | JDBC 드라이버 클래스의 이름을 설정합니다. |
### getConnectionString() {#getConnectionString--}
```
public final String getConnectionString()
```


연결 문자열을 가져옵니다.

**Returns:**
java.lang.String - 연결 문자열.
### getDriverClassName() {#getDriverClassName--}
```
public final String getDriverClassName()
```


JDBC 드라이버 클래스의 이름을 반환합니다. 기본 드라이버 클래스 이름은 "com.microsoft.jdbc.sqlserver.SQLServerDriver"입니다.

**Returns:**
java.lang.String - 드라이버 클래스 문자열.
### setConnectionString(String value) {#setConnectionString-java.lang.String-}
```
public final void setConnectionString(String value)
```


연결 문자열을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | 연결 문자열. |

### setDriverClassName(String value) {#setDriverClassName-java.lang.String-}
```
public final void setDriverClassName(String value)
```


JDBC 드라이버 클래스의 이름을 설정합니다. 기본 드라이버 클래스 이름은 "com.microsoft.jdbc.sqlserver.SQLServerDriver"입니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | JDBC 드라이버 클래스의 이름. |

