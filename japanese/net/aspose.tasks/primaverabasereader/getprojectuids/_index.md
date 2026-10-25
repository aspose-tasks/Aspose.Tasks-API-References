---
title: "PrimaveraBaseReader.GetProjectUids"
second_title: "Aspose.Tasks for .NET API リファレンス"
description: "PrimaveraBaseReader メソッド。プロジェクトのユニーク識別子のリストを返します"
type: docs
weight: 20
url: /ja/net/aspose.tasks/primaverabasereader/getprojectuids/
---
## PrimaveraBaseReader.GetProjectUids method

プロジェクトの一意の識別子のリストを返します。

```csharp
public List<int> GetProjectUids()
```

### 戻り値

プロジェクトのユニーク識別子のリスト。

## 例

Primavera XML ファイルからプロジェクトをインポートする方法を示します。

```csharp
var reader = new PrimaveraXmlReader(DataDir + "primavera.xml");
List<int> projectUids = reader.GetProjectUids();
foreach (var projectUid in projectUids)
{
    Console.WriteLine("Project UID: " + projectUid);
}
```

### 関連項目

* class [PrimaveraBaseReader](../)
* namespace [Aspose.Tasks](../../primaverabasereader/)
* assembly [Aspose.Tasks](../../../)


