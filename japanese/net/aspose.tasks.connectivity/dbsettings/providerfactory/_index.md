---
title: "DbSettings.ProviderFactory"
second_title: "Aspose.Tasks for .NET API リファレンス"
description: "DbSettings プロパティ。データベース接続に使用される DbProviderFactory のインスタンスを取得または設定します。ProviderFactory と ProviderInvariantName の両方が設定されている場合、ProviderFactory が優先されます。デフォルト値は null です。"
type: docs
weight: 30
url: /ja/net/aspose.tasks.connectivity/dbsettings/providerfactory/
---
## DbSettings.ProviderFactory property

データベース接続に使用される DbProviderFactory のインスタンスを取得または設定します。ProviderFactory と ProviderInvariantName の両方が設定されている場合、ProviderFactory が優先されます。デフォルト値は null です。

```csharp
public DbProviderFactory ProviderFactory { get; set; }
```

## 例

Primavera データベースからプロジェクトをインポートする方法を示します。

```csharp
// 接続文字列とプロジェクト ID を使用して PrimaveraDbSettings クラスの新しいインスタンスを初期化します
var settings = new PrimaveraDbSettings(GetConnectionString(), 4502);
settings.ProviderFactory = SqliteFactory.Instance;

Console.WriteLine("Project UID to read: " + settings.ProjectId);

// UID = 4502 のプロジェクトを読み取ります
var project = new Project(settings);
Console.WriteLine(project.Uid);
Console.WriteLine(project.Name);
Console.WriteLine(project.PrimaveraProperties.ShortName);
```

### 関連項目

* class [DbSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../dbsettings/)
* assembly [Aspose.Tasks](../../../)


