---
title: "クラス PrimaveraDbReader"
second_title: "Aspose.Tasks for .NET API リファレンス"
description: "Aspose.Tasks.PrimaveraDbReader クラス。Primavera DB からプロジェクト情報を読み取るリーダーを表します。"
type: docs
weight: 1350
url: /ja/net/aspose.tasks/primaveradbreader/
---
## PrimaveraDbReader class

Primavera DB からプロジェクト情報を読み取るリーダーを表します。

```csharp
public sealed class PrimaveraDbReader : PrimaveraBaseReader
```

## コンストラクタ

| 名前 | 説明 |
| --- | --- |
| [PrimaveraDbReader](primaveradbreader/)(PrimaveraDbSettings) | 新しい [`PrimaveraXerReader`](../primaveraxerreader/) クラスのインスタンスを初期化します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [GetProjectInfos](../../aspose.tasks/primaverabasereader/getprojectinfos/)() | プロジェクトの簡易情報オブジェクトのリストを返します。 |
| [GetProjectUids](../../aspose.tasks/primaverabasereader/getprojectuids/)() | プロジェクトの一意の識別子のリストを返します。 |
| override [LoadProject](../../aspose.tasks/primaveradbreader/loadproject/)(int) | 指定された一意の識別子でプロジェクトをロードします。 |

## 例

Primavera データベースからプロジェクトの簡易情報を取得する方法を示します。

```csharp
var settings = new PrimaveraDbSettings(GetConnectionString(), 0);

var reader = new PrimaveraDbReader(settings);
var projectInfos = reader.GetProjectInfos();

foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - '{2}'", info.Uid, info.ShortName, info.Name);
}

var firstProject = reader.LoadProject(projectInfos[0].Uid);
Console.WriteLine(firstProject.Uid);
Console.WriteLine(firstProject.Name);
Console.WriteLine(firstProject.PrimaveraProperties.ShortName);
```

### 関連項目

* class [PrimaveraBaseReader](../primaverabasereader/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


