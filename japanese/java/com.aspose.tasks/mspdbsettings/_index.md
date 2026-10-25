---
title: "MspDbSettings"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "MS Project Server データベースからプロジェクト データを読み取るために必要なオプションを設定できるようにします。"
type: docs
weight: 161
url: /ja/java/com.aspose.tasks/mspdbsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.DbSettings](../../com.aspose.tasks/dbsettings)
```
public class MspDbSettings extends DbSettings
```

MS Project Server データベースからプロジェクト データを読み取るために必要なオプションを設定できるようにします。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [MspDbSettings(String connectionString, UUID projectGuid)](#MspDbSettings-java.lang.String-java.util.UUID-) | 新しい [MspDbSettings](../../com.aspose.tasks/mspdbsettings) クラスのインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getProjectGuid()](#getProjectGuid--) | 読み取るプロジェクトの GUID を取得します。 |
| [getSchema()](#getSchema--) | MS Project Server のスキーマを取得します。 |
| [setSchema(String value)](#setSchema-java.lang.String-) | MS Project Server のスキーマを設定します。 |
### MspDbSettings(String connectionString, UUID projectGuid) {#MspDbSettings-java.lang.String-java.util.UUID-}
```
public MspDbSettings(String connectionString, UUID projectGuid)
```


新しい [MspDbSettings](../../com.aspose.tasks/mspdbsettings) クラスのインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| connectionString | java.lang.String | 指定された接続文字列です。 |
| projectGuid | java.util.UUID | 読み取るプロジェクトの指定された GUID です。 |

### getProjectGuid() {#getProjectGuid--}
```
public final UUID getProjectGuid()
```


読み取るプロジェクトの GUID を取得します。

**Returns:**
java.util.UUID - 読み取るプロジェクトの GUID です。
### getSchema() {#getSchema--}
```
public final String getSchema()
```


MS Project Server のスキーマを取得します。デフォルト値は "pub" です。

**Returns:**
java.lang.String - MS Project Server のスキーマです。
### setSchema(String value) {#setSchema-java.lang.String-}
```
public final void setSchema(String value)
```


MS Project Server のスキーマを設定します。デフォルト値は "pub" です。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | MS Project Server のスキーマです。 |

