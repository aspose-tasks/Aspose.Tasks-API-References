---
title: "FontSettings.DefaultFontName"
second_title: "Aspose.Tasks for .NET API リファレンス"
description: "FontSettings プロパティ。レンダリング用のデフォルトまたはフォールバックフォントを取得または設定します"
type: docs
weight: 20
url: /ja/net/aspose.tasks/fontsettings/defaultfontname/
---
## FontSettings.DefaultFontName property

レンダリング用のデフォルト（またはフォールバック）フォントを取得または設定します。

```csharp
public string DefaultFontName { get; set; }
```

## 例

出力 PDF の印刷に使用されるカスタムフォントの設定方法を示します。

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions
                  {
                      PresentationFormat = PresentationFormat.GanttChart, FitContent = true
                  };

options.FontSettings.UseProjectDefaultFont = false;
options.FontSettings.DefaultFontName = "Segoe UI Black";
project.Save(OutDir + "CreateProject2_out.pdf", options);
```

### 関連項目

* class [FontSettings](../)
* namespace [Aspose.Tasks](../../fontsettings/)
* assembly [Aspose.Tasks](../../../)


