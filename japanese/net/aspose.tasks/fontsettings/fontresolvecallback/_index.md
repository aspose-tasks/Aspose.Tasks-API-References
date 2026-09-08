---
title: "FontSettings.FontResolveCallback"
second_title: "Aspose.Tasks for .NET API リファレンス"
description: "FontSettings プロパティ。解決されたフォントをカスタマイズするために使用できるコールバックを取得または設定します"
type: docs
weight: 30
url: /ja/net/aspose.tasks/fontsettings/fontresolvecallback/
---
## FontSettings.FontResolveCallback property

解決されたフォントをカスタマイズするために使用できるコールバックを取得または設定します。

```csharp
public FontResolveCallbackDelegate FontResolveCallback { get; set; }
```

## 例

フォールバックフォントを設定したり特定のフォントを置き換えたりするために、ユーザー定義コードを実行するカスタムフォント解決コールバックの設定方法を示します。

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.GanttChart,
};

options.FontSettings.FontResolveCallback = delegate(FontResolveEventArgs args)
{
    if (args.RequestedFontName != args.ResolvedFontName)
    {
        // 正確なフォントが見つからず、フォールバックフォントが設定されたようです。
        // フォールバックフォントを上書きできます。
        args.ResolvedFontName = "Arial";
    }

    // または、単に特定のフォントを置き換えるだけです:
    if (args.RequestedFontName == "Comic Sans MS")
    {
        args.ResolvedFontName = "Arial";
    }
};

project.Save(OutDir + "EstimatedMilestoneTasks_out3.pdf", options);
```

### 関連項目

* delegate [FontResolveCallbackDelegate](../../fontresolvecallbackdelegate/)
* class [FontSettings](../)
* namespace [Aspose.Tasks](../../fontsettings/)
* assembly [Aspose.Tasks](../../../)


