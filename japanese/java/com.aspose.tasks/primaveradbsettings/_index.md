---
title: "PrimaveraDbSettings"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "Primavera データベースからプロジェクトデータを読み取るために必要なオプションを設定できます。"
type: docs
weight: 201
url: /ja/java/com.aspose.tasks/primaveradbsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.DbSettings](../../com.aspose.tasks/dbsettings)
```
public class PrimaveraDbSettings extends DbSettings
```

Primavera データベースからプロジェクトデータを読み取るために必要なオプションを設定できます。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [PrimaveraDbSettings(String connectionString, int projectId)](#PrimaveraDbSettings-java.lang.String-int-) | 新しい [PrimaveraDbSettings](../../com.aspose.tasks/primaveradbsettings) クラスのインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getProjectId()](#getProjectId--) | 読み取るプロジェクトの ID を取得します。 |
### PrimaveraDbSettings(String connectionString, int projectId) {#PrimaveraDbSettings-java.lang.String-int-}
```
public PrimaveraDbSettings(String connectionString, int projectId)
```


新しい [PrimaveraDbSettings](../../com.aspose.tasks/primaveradbsettings) クラスのインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| connectionString | java.lang.String | 指定された接続文字列です。 |
| projectId | int | 読み取るプロジェクトの指定された ID です。 |

### getProjectId() {#getProjectId--}
```
public final int getProjectId()
```


読み取るプロジェクトの ID を取得します。

**Returns:**
int - 読み取るプロジェクトの ID です。
