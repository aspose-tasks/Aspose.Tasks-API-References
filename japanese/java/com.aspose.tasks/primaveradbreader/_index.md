---
title: "PrimaveraDbReader"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "Primavera DB からプロジェクト情報を読み取るリーダーを表します。"
type: docs
weight: 200
url: /ja/java/com.aspose.tasks/primaveradbreader/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.PrimaveraBaseReader](../../com.aspose.tasks/primaverabasereader)
```
public final class PrimaveraDbReader extends PrimaveraBaseReader
```

Primavera DB からプロジェクト情報を読み取るリーダーを表します。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [PrimaveraDbReader(PrimaveraDbSettings dbSettings)](#PrimaveraDbReader-com.aspose.tasks.PrimaveraDbSettings-) | 新しい [PrimaveraXerReader](../../com.aspose.tasks/primaveraxerreader) クラスのインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [loadProject(int projectUid)](#loadProject-int-) | 指定された一意の識別子でプロジェクトをロードします。 |
### PrimaveraDbReader(PrimaveraDbSettings dbSettings) {#PrimaveraDbReader-com.aspose.tasks.PrimaveraDbSettings-}
```
public PrimaveraDbReader(PrimaveraDbSettings dbSettings)
```


新しい [PrimaveraXerReader](../../com.aspose.tasks/primaveraxerreader) クラスのインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| dbSettings | [PrimaveraDbSettings](../../com.aspose.tasks/primaveradbsettings) | Primavera DB への接続方法を指定する設定。 |

### loadProject(int projectUid) {#loadProject-int-}
```
public Project loadProject(int projectUid)
```


指定された一意の識別子でプロジェクトをロードします。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| projectUid | int | ロードするプロジェクトの一意の識別子です。 |

**Returns:**
[Project](../../com.aspose.tasks/project) - Project with specified unique identifier read from Primavera DB. Null if project doesn't exist.
