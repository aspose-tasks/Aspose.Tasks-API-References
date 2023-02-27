---
title: HtmlSaveOptions
second_title: Aspose.Tasks for .NET API リファレンス
description: プロジェクト ページを HTML にレンダリングするときに追加のオプションを指定できます
type: docs
weight: 1750
url: /ja/net/aspose.tasks.saving/htmlsaveoptions/
---
## HtmlSaveOptions class

プロジェクト ページを HTML にレンダリングするときに、追加のオプションを指定できます。

```csharp
public class HtmlSaveOptions : SaveOptions
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [HtmlSaveOptions](htmlsaveoptions/)() | の新しいインスタンスを初期化します`HtmlSaveOptions`class. |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [BarStyles](../../aspose.tasks.saving/saveoptions/barstyles/) { get; set; } | のインスタンスのリストを取得または設定します[`BarStyle`](../../aspose.tasks.visualization/barstyle/)プロジェクト ビューに表示されるクラス. |
| [CssSavingCallback](../../aspose.tasks.saving/htmlsaveoptions/csssavingcallback/) { get; set; } | CSS を格納するリソースを作成するために呼び出されるコールバックを取得または設定します。 |
| [CssStylePrefix](../../aspose.tasks.saving/htmlsaveoptions/cssstyleprefix/) { get; set; } | CSS スタイル プレフィックスを取得または設定します。 |
| [CustomPageSize](../../aspose.tasks.saving/saveoptions/custompagesize/) { get; set; } | カスタム ページ サイズをポイント単位で取得または設定します (1 ポイント = 1/72 インチ). |
| [DefaultFontName](../../aspose.tasks.saving/htmlsaveoptions/defaultfontname/) { get; set; } | レンダリング用のデフォルト フォントを取得または設定します。 |
| [DrawNonWorkingTime](../../aspose.tasks.saving/saveoptions/drawnonworkingtime/) { get; set; } | 非稼働時間を描画するかどうかを示す値を取得または設定します (デフォルト値は TRUE です). |
| [EndDate](../../aspose.tasks.saving/saveoptions/enddate/) { get; set; } | レンダリングを終了する日付を取得または設定します。 |
| [ExportCss](../../aspose.tasks.saving/htmlsaveoptions/exportcss/) { get; set; } | CSS のエクスポート方法を取得または設定します。 |
| [ExportFonts](../../aspose.tasks.saving/htmlsaveoptions/exportfonts/) { get; set; } | フォントのエクスポート方法を取得または設定します。 |
| [ExportImages](../../aspose.tasks.saving/htmlsaveoptions/exportimages/) { get; set; } | 画像のエクスポート方法を取得または設定します。 |
| [FitContent](../../aspose.tasks.saving/saveoptions/fitcontent/) { get; set; } | コンテンツに合わせて行の高さを増やす必要があるかどうかを示す値を取得または設定します. |
| [FitTimescaleToEndOfPage](../../aspose.tasks.saving/saveoptions/fittimescaletoendofpage/) { get; set; } | ビューのカレンダー セクションを最後のページの最後 (右側) にレンダリングするかどうかを取得または設定します。 値が false の場合、ページに空白があっても、カレンダー セクションは正確に EndDate にレンダリングされます。 |
| [FontFaceTypes](../../aspose.tasks.saving/htmlsaveoptions/fontfacetypes/) { get; set; } | フォント フェイス タイプを取得または設定します。 |
| [FontResolveCallback](../../aspose.tasks.saving/htmlsaveoptions/fontresolvecallback/) { get; set; } | 解決されたフォントのカスタマイズに使用できるコールバックを取得または設定します。 |
| [FontSavingCallback](../../aspose.tasks.saving/htmlsaveoptions/fontsavingcallback/) { get; set; } | フォントを格納するリソースを作成するために呼び出されるコールバックを取得または設定します。 |
| [Gridlines](../../aspose.tasks.saving/saveoptions/gridlines/) { get; set; } | のリストを取得または設定します[`Gridline`](../../aspose.tasks.visualization/gridline/)プロジェクトビューに表示される. |
| [ImageSavingCallback](../../aspose.tasks.saving/htmlsaveoptions/imagesavingcallback/) { get; set; } | フォントを格納するリソースを作成するために呼び出されるコールバックを取得または設定します。 |
| [IncludeProjectNameInPageHeader](../../aspose.tasks.saving/htmlsaveoptions/includeprojectnameinpageheader/) { get; set; } | HTML ページ ヘッダーにプロジェクト名を含めるかどうかを示す値を取得または設定します。 |
| [IncludeProjectNameInTitle](../../aspose.tasks.saving/htmlsaveoptions/includeprojectnameintitle/) { get; set; } | HTML タイトルにプロジェクト名を含めるかどうかを示す値を取得または設定します。 |
| [LegendOnEachPage](../../aspose.tasks.saving/saveoptions/legendoneachpage/) { get; set; } | 各ページに凡例を表示するかどうかを示す値を取得または設定します (デフォルト値は TRUE です)。 |
| [MarkCriticalTasks](../../aspose.tasks.saving/saveoptions/markcriticaltasks/) { get; set; } | 重要なタスクを赤色で表示するかどうかを示す値を取得または設定します (デフォルト値は FALSE です)。 |
| [NonWorkingTimeColor](../../aspose.tasks.saving/saveoptions/nonworkingtimecolor/) { get; set; } | 非稼働時間の色を取得または設定します。 |
| [PageCount](../../aspose.tasks.saving/saveoptions/pagecount/) { get; } | プロジェクトのページ数を取得または設定します。 |
| [Pages](../../aspose.tasks.saving/htmlsaveoptions/pages/) { get; set; } | プロジェクト レイアウトをレンダリングするときに保存するページ番号のリストを取得または設定します。このリストが空の場合、すべてのプロジェクト ページが保存されます。 |
| [PageSavingCallback](../../aspose.tasks.saving/htmlsaveoptions/pagesavingcallback/) { get; set; } | レンダリングされた各ページの出力ストリームを取得するために使用されるユーザー定義のコールバックを取得または設定します。 |
| [PageSize](../../aspose.tasks.saving/saveoptions/pagesize/) { get; set; } | レンダリングするページのサイズを取得または設定します (デフォルト値は PageSize.A4 です). |
| [PresentationFormat](../../aspose.tasks.saving/saveoptions/presentationformat/) { get; set; } | を取得または設定します[`PresentationFormat`](../saveoptions/presentationformat/)ドキュメントが保存される場所. |
| [ReduceFooterGap](../../aspose.tasks.saving/htmlsaveoptions/reducefootergap/) { get; set; } | 最後のタスクとフッターの間のギャップを縮小する必要があるかどうかを示す値を取得または設定します. |
| [RenderToSinglePage](../../aspose.tasks.saving/saveoptions/rendertosinglepage/) { get; set; } | プロジェクトをグラフィック形式で保存するときに、プロジェクトを 1 つのページにレンダリングする必要があるかどうかを示す値を取得または設定します . レンダリングされたプロジェクトが 1 ページに収まるようにページ サイズが変更されます. |
| [RollUpGanttBars](../../aspose.tasks.saving/saveoptions/rollupganttbars/) { get; set; } | サマリー タスク バーのサブタスクをマークするかどうかを示す値を取得または設定します。フィールドは、サマリー タスク バーにロールアップ バーを表示するかどうかを示します。 サブタスクをロールアップするには、サマリー タスクのロールアップ フィールドをはいに設定する必要があります。 |
| [SaveFormat](../../aspose.tasks.saving/saveoptions/saveformat/) { get; } | この保存オプション オブジェクトが使用される場合にドキュメントが保存される形式を取得または設定します。 |
| [StartDate](../../aspose.tasks.saving/saveoptions/startdate/) { get; set; } | レンダリングを開始する日付を取得または設定します。 |
| [TasksComparer](../../aspose.tasks.saving/saveoptions/taskscomparer/) { get; set; } | ガント チャートおよびタスク シート チャートでタスクを並べ替える比較演算子を取得または設定します。 |
| [TasksFilter](../../aspose.tasks.saving/saveoptions/tasksfilter/) { get; set; } | ガント チャート、タスク シート、およびタスク配分状況チャートに表示されるタスクをフィルター処理するために使用される条件を取得または設定します。 |
| [TextStyles](../../aspose.tasks.saving/saveoptions/textstyles/) { get; set; } | のインスタンスのリストを取得または設定します[`TextStyle`](../../aspose.tasks.visualization/textstyle/)プロジェクト ビューに表示されるクラス. |
| [Timescale](../../aspose.tasks.saving/saveoptions/timescale/) { get; set; } | を取得または設定します[`Timescale`](../saveoptions/timescale/)プロジェクトがグラフィック形式で保存されるときに、タイムスケール (存在する場合) のレンダリング方法を制御するために使用される値. |
| override [UseGradientBrush](../../aspose.tasks.saving/htmlsaveoptions/usegradientbrush/) { get; set; } | プロジェクト レイアウトのレンダリング時にグラデーション ブラシを使用するかどうかを示す値を取得または設定します。現在、HTML にレンダリングする場合、グラデーション ブラシの使用はサポートされていません。 |
| [UseProjectDefaultFont](../../aspose.tasks.saving/htmlsaveoptions/useprojectdefaultfont/) { get; set; } | レンダリングに既定のフォントを使用する必要があるかどうかを示す値を取得または設定します。 |
| [View](../../aspose.tasks.saving/saveoptions/view/) { get; set; } | レンダリングするビュー列のリストを取得または設定します ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/) ). 設定されていない場合、タスク ID、タスク名、開始と終了のみがレンダリングされます。[`ViewSettings`](../saveoptions/viewsettings/)プロパティが設定され、View の列が ViewSettings. の列をオーバーライドします。 |
| [ViewSettings](../../aspose.tasks.saving/saveoptions/viewsettings/) { get; set; } | ビューを取得または設定します ([`View`](../saveoptions/view/) ) レンダリングします。このオプションを使用して、どのビューを PDF、HTML、または画像形式で保存するかを明示的に指定できます。 このプロパティが設定されている場合、[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/)プロパティは、プロジェクトが保存されるときに無視されます。 ビューは、次のいずれかの画面 (([`Screen`](../../aspose.tasks/view/screen/) )): (ガント、TaskSheet、TaskUsage、ResourceSheet、ResourceUsage) |

### 関連項目

* class [SaveOptions](../saveoptions/)
* 名前空間 [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* 組み立て [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
