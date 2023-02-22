---
title: PdfSaveOptions
second_title: Aspose.Tasks for .NET API リファレンス
description: プロジェクト ページを PDF にレンダリングするときに追加オプションを指定できます
type: docs
weight: 1860
url: /ja/net/aspose.tasks.saving/pdfsaveoptions/
---
## PdfSaveOptions class

プロジェクト ページを PDF にレンダリングするときに追加オプションを指定できます。

```csharp
public class PdfSaveOptions : SaveOptions
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [PdfSaveOptions](pdfsaveoptions/)() | の新しいインスタンスを初期化します`PdfSaveOptions`ドキュメントを保存するために使用できるクラス[`PDF`](../savefileformat/)フォーマット。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [BarStyles](../../aspose.tasks.saving/saveoptions/barstyles/) { get; set; } | のインスタンスのリストを取得または設定します[`BarStyle`](../../aspose.tasks.visualization/barstyle/)プロジェクト ビューに表示されるクラス. |
| [Compliance](../../aspose.tasks.saving/pdfsaveoptions/compliance/) { get; set; } | 生成された PDF ドキュメントに必要なコンプライアンス レベルを取得または設定します。 デフォルトはPdf15. |
| [CustomPageSize](../../aspose.tasks.saving/saveoptions/custompagesize/) { get; set; } | カスタム ページ サイズをポイント単位で取得または設定します (1 ポイント = 1/72 インチ). |
| [DefaultFontName](../../aspose.tasks.saving/pdfsaveoptions/defaultfontname/) { get; set; } | レンダリング用のデフォルト フォントを取得または設定します。 |
| [DigitalSignatureDetails](../../aspose.tasks.saving/pdfsaveoptions/digitalsignaturedetails/) { get; set; } | デジタル署名の詳細を取得または設定します。設定されていない場合、署名は実行されません. |
| [DrawNonWorkingTime](../../aspose.tasks.saving/saveoptions/drawnonworkingtime/) { get; set; } | 非稼働時間を描画するかどうかを示す値を取得または設定します (デフォルト値は TRUE です). |
| [EncryptionDetails](../../aspose.tasks.saving/pdfsaveoptions/encryptiondetails/) { get; set; } | 暗号化の詳細を取得または設定します。設定されていない場合、暗号化は実行されません. |
| [EndDate](../../aspose.tasks.saving/saveoptions/enddate/) { get; set; } | レンダリングを終了する日付を取得または設定します。 |
| [FitContent](../../aspose.tasks.saving/saveoptions/fitcontent/) { get; set; } | コンテンツに合わせて行の高さを増やす必要があるかどうかを示す値を取得または設定します. |
| [FitTimescaleToEndOfPage](../../aspose.tasks.saving/saveoptions/fittimescaletoendofpage/) { get; set; } | ビューのカレンダー セクションを最後のページの最後 (右側) にレンダリングするかどうかを取得または設定します。 値が false の場合、ページに空白があっても、カレンダー セクションは正確に EndDate にレンダリングされます。 |
| [FontResolveCallback](../../aspose.tasks.saving/pdfsaveoptions/fontresolvecallback/) { get; set; } | 解決されたフォントのカスタマイズに使用できるコールバックを取得または設定します。 |
| [Gridlines](../../aspose.tasks.saving/saveoptions/gridlines/) { get; set; } | のリストを取得または設定します[`Gridline`](../../aspose.tasks.visualization/gridline/)プロジェクトビューに表示される. |
| [LegendOnEachPage](../../aspose.tasks.saving/saveoptions/legendoneachpage/) { get; set; } | 各ページに凡例を表示するかどうかを示す値を取得または設定します (デフォルト値は TRUE です)。 |
| [MarkCriticalTasks](../../aspose.tasks.saving/saveoptions/markcriticaltasks/) { get; set; } | 重要なタスクを赤色で表示するかどうかを示す値を取得または設定します (デフォルト値は FALSE です)。 |
| [NonWorkingTimeColor](../../aspose.tasks.saving/saveoptions/nonworkingtimecolor/) { get; set; } | 非稼働時間の色を取得または設定します。 |
| [PageCount](../../aspose.tasks.saving/saveoptions/pagecount/) { get; } | プロジェクトのページ数を取得または設定します。 |
| [Pages](../../aspose.tasks.saving/pdfsaveoptions/pages/) { get; set; } | プロジェクト レイアウトを別のファイルに保存するときに保存するページ番号のリストを取得または設定します。このリストが空の場合、すべてのページが保存されます。 |
| [PageSavingCallback](../../aspose.tasks.saving/pdfsaveoptions/pagesavingcallback/) { get; set; } | レンダリングされた各ページの出力ストリームを取得するために使用されるユーザー定義のコールバックを取得または設定します。[`SaveToSeparateFiles`](./savetoseparatefiles/)オプションが使用されています. |
| [PageSize](../../aspose.tasks.saving/saveoptions/pagesize/) { get; set; } | レンダリングするページのサイズを取得または設定します (デフォルト値は PageSize.A4 です). |
| [PresentationFormat](../../aspose.tasks.saving/saveoptions/presentationformat/) { get; set; } | を取得または設定します[`PresentationFormat`](../saveoptions/presentationformat/)ドキュメントが保存される場所. |
| [ReduceFooterGap](../../aspose.tasks.saving/pdfsaveoptions/reducefootergap/) { get; set; } | 最後のタスクとフッターの間のギャップを縮小する必要があるかどうかを示す値を取得または設定します. |
| [RenderToSinglePage](../../aspose.tasks.saving/saveoptions/rendertosinglepage/) { get; set; } | プロジェクトをグラフィック形式で保存するときに、プロジェクトを 1 つのページにレンダリングする必要があるかどうかを示す値を取得または設定します . レンダリングされたプロジェクトが 1 ページに収まるようにページ サイズが変更されます. |
| [RollUpGanttBars](../../aspose.tasks.saving/saveoptions/rollupganttbars/) { get; set; } | サマリー タスク バーのサブタスクをマークするかどうかを示す値を取得または設定します。フィールドは、サマリー タスク バーにロールアップ バーを表示するかどうかを示します。 サブタスクをロールアップするには、サマリー タスクのロールアップ フィールドをはいに設定する必要があります。 |
| [SaveFormat](../../aspose.tasks.saving/saveoptions/saveformat/) { get; } | この保存オプション オブジェクトが使用される場合にドキュメントが保存される形式を取得または設定します。 |
| [SaveToSeparateFiles](../../aspose.tasks.saving/pdfsaveoptions/savetoseparatefiles/) { get; set; } | プロジェクト ページを別のファイルに保存するかどうかを示す値を取得または設定します。 |
| [StartDate](../../aspose.tasks.saving/saveoptions/startdate/) { get; set; } | レンダリングを開始する日付を取得または設定します。 |
| [TasksComparer](../../aspose.tasks.saving/saveoptions/taskscomparer/) { get; set; } | ガント チャートおよびタスク シート チャートでタスクを並べ替える比較演算子を取得または設定します。 |
| [TasksFilter](../../aspose.tasks.saving/saveoptions/tasksfilter/) { get; set; } | ガント チャート、タスク シート、およびタスク配分状況チャートに表示されるタスクをフィルター処理するために使用される条件を取得または設定します。 |
| [TextCompression](../../aspose.tasks.saving/pdfsaveoptions/textcompression/) { get; set; } | 画像を除くすべてのコンテンツ ストリームに使用される圧縮タイプを取得または設定します。 デフォルトはFlate. |
| [TextStyles](../../aspose.tasks.saving/saveoptions/textstyles/) { get; set; } | のインスタンスのリストを取得または設定します[`TextStyle`](../../aspose.tasks.visualization/textstyle/)プロジェクト ビューに表示されるクラス. |
| [Timescale](../../aspose.tasks.saving/saveoptions/timescale/) { get; set; } | を取得または設定します[`Timescale`](../saveoptions/timescale/)プロジェクトがグラフィック形式で保存されるときに、タイムスケール (存在する場合) のレンダリング方法を制御するために使用される値. |
| virtual [UseGradientBrush](../../aspose.tasks.saving/saveoptions/usegradientbrush/) { get; set; } | ガント チャートのレンダリング時にグラデーション ブラシを使用するかどうかを示す値を取得または設定します。 |
| [UseProjectDefaultFont](../../aspose.tasks.saving/pdfsaveoptions/useprojectdefaultfont/) { get; set; } | レンダリングに既定のフォントを使用する必要があるかどうかを示す値を取得または設定します。 |
| [View](../../aspose.tasks.saving/saveoptions/view/) { get; set; } | レンダリングするビュー列のリストを取得または設定します ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/) ). 設定されていない場合、タスク ID、タスク名、開始と終了のみがレンダリングされます。[`ViewSettings`](../saveoptions/viewsettings/)プロパティが設定され、View の列が ViewSettings. の列をオーバーライドします。 |
| [ViewSettings](../../aspose.tasks.saving/saveoptions/viewsettings/) { get; set; } | ビューを取得または設定します ([`View`](../saveoptions/view/) ) レンダリングします。このオプションを使用して、どのビューを PDF、HTML、または画像形式で保存するかを明示的に指定できます。 このプロパティが設定されている場合、[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/)プロパティは、プロジェクトが保存されるときに無視されます。 ビューは、次のいずれかの画面 (([`Screen`](../../aspose.tasks/view/screen/) )): (ガント、TaskSheet、TaskUsage、ResourceSheet、ResourceUsage) |

### 関連項目

* class [SaveOptions](../saveoptions/)
* 名前空間 [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* 組み立て [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
