---
title: "FontSettings.UseProjectDefaultFont"
second_title: "Aspose.Tasks for .NET API リファレンス"
description: "FontSettings プロパティ。レンダリングにデフォルトフォントを使用すべきかを示す値を取得または設定します"
type: docs
weight: 40
url: /ja/net/aspose.tasks/fontsettings/useprojectdefaultfont/
---
## FontSettings.UseProjectDefaultFont property

レンダリングにデフォルトフォントを使用しなければならないかどうかを示す値を取得または設定します。

```csharp
public bool UseProjectDefaultFont { get; set; }
```

## 備考

値が False で DefaultFontName が指定されている場合、レンダリングエンジンは DefaultFontName で指定されたフォントをフォールバックフォントとして使用します。そうでない場合は、'Arial'（インストールされている場合）または 'Generic Sans Serif' フォントがフォールバックフォントとして使用されます。フォールバックフォントは、テキストスタイルが現在のオペレーティングシステムにインストールされていないフォントを参照している場合のプロジェクトビューのレンダリング時に使用されます。フォント解決をより細かく制御したい場合は、[`FontResolveCallback`](../fontresolvecallback/) コールバックを使用できます。

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


