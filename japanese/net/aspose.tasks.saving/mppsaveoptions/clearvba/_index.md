---
title: "MPPSaveOptions.ClearVba"
second_title: "Aspose.Tasks for .NET API リファレンス"
description: "MPPSaveOptions プロパティ。プロジェクトを MPP 形式で保存する際に既存の VBA マクロ データを削除するかどうかを示す値を取得または設定します"
type: docs
weight: 20
url: /ja/net/aspose.tasks.saving/mppsaveoptions/clearvba/
---
## MPPSaveOptions.ClearVba property

プロジェクトを MPP 形式で保存する際に既存の VBA マクロ データを削除するかどうかを示す値を取得または設定します。

```csharp
public bool ClearVba { get; set; }
```

## 例

MPP ファイルから VBA マクロを削除する方法を示します。

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
project.Save(OutDir + "Vba.cleared.mpp", new MPPSaveOptions() { ClearVba = true });
```

### 関連項目

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


