---
title: "PrimaveraProjectProperties.CurrentBaselineProjectId"
second_title: "Aspose.Tasks for .NET API リファレンス"
description: "PrimaveraProjectProperties プロパティ。現在のベースラインプロジェクトの ID を取得します。エクスポートされたベースラインを含む Primavera XML ファイルから読み込んだプロジェクトに適用可能です"
type: docs
weight: 40
url: /ja/net/aspose.tasks/primaveraprojectproperties/currentbaselineprojectid/
---
## PrimaveraProjectProperties.CurrentBaselineProjectId property

現在のベースラインプロジェクトの ID を取得します。エクスポートされたベースラインを含む Primavera XML ファイルから読み込まれたプロジェクトに適用できます。

```csharp
public int CurrentBaselineProjectId { get; }
```

## 例

Primavera XML ファイルからプロジェクトを読み取り、ベースラインプロジェクトデータを調べる方法を示します。

```csharp
Project project = new Project(DataDir + "BaselineProjects.xml");

Console.WriteLine("Current baseline project uid: " + project.PrimaveraProperties.CurrentBaselineProjectId);

foreach (var baselineProject in project.PrimaveraProperties.BaselineProjects)
{
    Console.WriteLine("Baseline project: uid: {0}, name: '{1}'", baselineProject.Uid, baselineProject.Name);
}

var baseline1 = project.PrimaveraProperties.BaselineProjects[1];

var task = GetTaskByActivityId(project, "A1000");
var baselineTask = GetTaskByActivityId(baseline1, "A1000");

Console.WriteLine("Task budgeted total cost: " + task.PrimaveraProperties.BudgetedTotalCost);
Console.WriteLine("Task baseline budgeted total cost: " + baselineTask.PrimaveraProperties.BudgetedTotalCost);
```

### 関連項目

* class [PrimaveraProjectProperties](../)
* namespace [Aspose.Tasks](../../primaveraprojectproperties/)
* assembly [Aspose.Tasks](../../../)


