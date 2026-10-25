---
title: "PrimaveraProjectProperties.BaselineProjects"
second_title: "Aspose.Tasks for .NET API リファレンス"
description: "PrimaveraProjectProperties プロパティ。現在のプロジェクトのベースラインプロジェクトの配列を取得します。エクスポートされたベースラインを含む Primavera XML ファイルから読み込まれたプロジェクトに適用されます"
type: docs
weight: 10
url: /ja/net/aspose.tasks/primaveraprojectproperties/baselineprojects/
---
## PrimaveraProjectProperties.BaselineProjects property

現在のプロジェクトのベースラインプロジェクトの配列を取得します。エクスポートされたベースラインを含む Primavera XML ファイルから読み込まれたプロジェクトに適用できます。

```csharp
public Project[] BaselineProjects { get; }
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

* class [Project](../../project/)
* class [PrimaveraProjectProperties](../)
* namespace [Aspose.Tasks](../../primaveraprojectproperties/)
* assembly [Aspose.Tasks](../../../)


