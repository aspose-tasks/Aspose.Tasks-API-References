---
title: "MpdSettings"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "MPD 形式の MS Access データベース ファイルからプロジェクト データを読み取るために必要なオプションを設定できるようにします。"
type: docs
weight: 160
url: /ja/java/com.aspose.tasks/mpdsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.DbSettings](../../com.aspose.tasks/dbsettings)
```
public class MpdSettings extends DbSettings
```

MPD形式（MS Access データベースファイル形式）からプロジェクト データを読み取るために必要なオプションを設定できるようにします。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [MpdSettings(String connectionString, int projectId)](#MpdSettings-java.lang.String-int-) | `MpdSettings` クラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getProjectId()](#getProjectId--) | 読み取るプロジェクトの ID を返します。 |
### MpdSettings(String connectionString, int projectId) {#MpdSettings-java.lang.String-int-}
```
public MpdSettings(String connectionString, int projectId)
```


`MpdSettings` クラスの新しいインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| connectionString | java.lang.String | 指定された接続文字列です。 |
| projectId | int | 読み取るプロジェクトの指定された ID です。 |

### getProjectId() {#getProjectId--}
```
public int getProjectId()
```


読み取るプロジェクトの ID を返します。

**Returns:**
int - 読み取るプロジェクトの ID です。
