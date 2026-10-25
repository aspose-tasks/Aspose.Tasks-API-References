---
title: "FontSettings.SetFontFolders"
second_title: "Aspose.Tasks for .NET API リファレンス"
description: "FontSettings メソッド。プロジェクトビューをレンダリングする際に Aspose.Tasks が TrueType フォントを検索するフォルダーを設定します"
type: docs
weight: 50
url: /ja/net/aspose.tasks/fontsettings/setfontfolders/
---
## FontSettings.SetFontFolders method

プロジェクトビューのレンダリング時に Aspose.Tasks が TrueType フォントを検索するフォルダーを設定します。

```csharp
public void SetFontFolders(string[] fontFolders, bool recursive)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| fontFolders | String[] | TrueType フォントを含むフォルダーの配列です。 |
| recursive | Boolean | true の場合、指定されたフォルダーは再帰的にスキャンされます。 |

## 例

カスタムフォントフォルダーの設定方法を示します。

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.GanttChart,
};

// 開いたプロジェクトで使用されるすべてのフォントの TrueType フォントファイルは MyFonts フォルダーに配置する必要があります。
options.FontSettings.SetFontFolders(new string[] { "c:\\MyFonts"}, true);

project.Save(OutDir + "EstimatedMilestoneTasks_out4.pdf", options);
```

### 関連項目

* class [FontSettings](../)
* namespace [Aspose.Tasks](../../fontsettings/)
* assembly [Aspose.Tasks](../../../)


