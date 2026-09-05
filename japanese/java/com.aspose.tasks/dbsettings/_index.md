---
title: "DbSettings"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "プロジェクト データベースから読み取る設定を指定できるようにします。"
type: docs
weight: 75
url: /ja/java/com.aspose.tasks/dbsettings/
---

**Inheritance:**
java.lang.Object
```
public abstract class DbSettings
```

プロジェクト データベースから読み取る設定を指定できるようにします。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getConnectionString()](#getConnectionString--) | 接続文字列を取得します。 |
| [getDriverClassName()](#getDriverClassName--) | JDBC ドライバークラスの名前を返します。 |
| [setConnectionString(String value)](#setConnectionString-java.lang.String-) | 接続文字列を設定します。 |
| [setDriverClassName(String value)](#setDriverClassName-java.lang.String-) | JDBC ドライバークラスの名前を設定します。 |
### getConnectionString() {#getConnectionString--}
```
public final String getConnectionString()
```


接続文字列を取得します。

**Returns:**
java.lang.String - 接続文字列。
### getDriverClassName() {#getDriverClassName--}
```
public final String getDriverClassName()
```


JDBC ドライバークラスの名前を返します。デフォルトのドライバークラス名は "com.microsoft.jdbc.sqlserver.SQLServerDriver" です。

**Returns:**
java.lang.String - ドライバークラス文字列。
### setConnectionString(String value) {#setConnectionString-java.lang.String-}
```
public final void setConnectionString(String value)
```


接続文字列を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | 接続文字列。 |

### setDriverClassName(String value) {#setDriverClassName-java.lang.String-}
```
public final void setDriverClassName(String value)
```


JDBC ドライバークラスの名前を設定します。デフォルトのドライバークラス名は "com.microsoft.jdbc.sqlserver.SQLServerDriver" です。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | JDBC ドライバークラスの名前。 |

