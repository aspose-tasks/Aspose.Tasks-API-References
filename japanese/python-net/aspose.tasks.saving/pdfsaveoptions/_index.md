---
title: "PdfSaveOptions"
second_title: "Aspose.Tasks for Python via .NET API リファレンス"
description: 
type: docs
weight: 90
url: /ja/python-net/aspose.tasks.saving/pdfsaveoptions/
---

## PdfSaveOptions class

プロジェクトページを PDF にレンダリングする際に、追加オプションを指定できます。

PdfSaveOptions 型は次のメンバーを公開します：
## コンストラクタ
| 名前 | 説明 |
| :- | :- |
| PdfSaveOptions() | PDF ドキュメントを保存するために使用できる [PdfSaveOptions](/tasks/python-net/aspose.tasks.saving/pdfsaveoptions/) クラスの新しいインスタンスを初期化します |
## プロパティ
| 名前 | 説明 |
| :- | :- |
| save_format |  |
| bar_styles | プロジェクトビューに表示される [BarStyle](/tasks/python-net/aspose.tasks.visualization/barstyle/) クラスのインスタンスのリストを取得または設定します。 |
| draw_non_working_time | 非稼働時間を描画するかどうかを示す値を取得または設定します（デフォルト値は TRUE です）。 |
| end_date | レンダリングを終了する日付を取得または設定します。 |
| timescale_fit_behavior | タイムスケールの右端をページの終端に合わせる方法を定義する動作を取得または設定します。 |
| fit_content | 行の高さを内容に合わせて増やすかどうかを示す値を取得または設定します。 |
| gridlines | プロジェクトビューに表示される [Gridline](/tasks/python-net/aspose.tasks.visualization/gridline/) のリストを取得または設定します。 |
| legend_drawing_options | 凡例の描画方法を定義する値を取得または設定します。デフォルト値は LegendDrawingOptions.OnEveryPage です。 |
| legend_items | ページ凡例に描画すべきバーを定義する PageLegendItem の配列を取得または設定します。<br/>            null の場合、デフォルト項目が描画されます。 |
| mark_critical_tasks | 重要タスクを赤色で表示するかどうかを示す値を取得または設定します（デフォルト値は FALSE）。 |
| non_working_time_color | 非稼働時間の色を取得または設定します。 |
| page_count | プロジェクトのページ数を取得または設定します。 |
| page_size | 描画されるページのサイズを取得または設定します（デフォルト値は PageSize.A4）。 |
| is_portrait | ページの向きが縦向きかどうかを示す値を取得または設定します。横向きの場合は false が返されます。 |
| presentation_format | ドキュメントが保存される [presentation_format](/tasks/python-net/aspose.tasks.saving/saveoptions/) を取得または設定します。 |
| roll_up_gantt_bars | サマリタスクバー上のサブタスクをマークするかどうかを示す値を取得または設定します。<br/>            サブタスクの場合、Rollup フィールドはサブタスクのガントバーの情報がサマリタスクバーにロールアップされるかどうかを示します。<br/>            サマリタスクの場合、Rollup フィールドはサマリタスクバーがロールアップされたバーを表示するかどうかを示します。<br/>            サブタスクをロールアップさせるには、サマリタスクの Rollup フィールドを Yes に設定している必要があります。 |
| start_date | 描画を開始する日付を取得または設定します。 |
| text_styles | プロジェクトビューの描画中に適用されるテキストスタイルのリストを取得または設定します。 |
| timescale | プロジェクトがグラフィック形式で保存される際に、タイムスケール（存在する場合）の描画方法を制御するために使用される [timescale](/tasks/python-net/aspose.tasks.saving/saveoptions/) の値を取得または設定します。 |
| use_gradient_brush | ガントチャートをレンダリングする際にグラデーションブラシを使用するかどうかを示す値を取得または設定します。 |
| view | 描画するビュー列のリストを取得または設定します（[GanttChartColumn](/tasks/python-net/aspose.tasks.visualization/ganttchartcolumn/)）。<br/>            設定されていない場合、タスク ID、タスク名、開始日と終了日だけが描画されます。<br/>            View と [view_settings](/tasks/python-net/aspose.tasks.saving/saveoptions/) の両方のプロパティが設定されている場合、View の列が ViewSettings の列を上書きします。 |
| view_settings | 描画するビュー ([view](/tasks/python-net/aspose.tasks.saving/saveoptions/)) を取得または設定します。このオプションを使用して、PDF、HTML、または画像形式で保存すべきビューを明示的に指定できます。<br/>            このプロパティが設定されている場合、プロジェクトが保存される際に [PresentationFormat](/tasks/python-net/aspose.tasks.visualization/presentationformat/) プロパティは無視されます。<br/>            ビューは次のいずれかの画面から選択する必要があります (([screen](/tasks/python-net/aspose.tasks/view/))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage) |
| custom_page_size | ポイント単位でカスタムページサイズを取得または設定します（1ポイント = 1/72インチ）。 |
| render_to_single_page | プロジェクトを単一ページにレンダリングすべきかどうかを示す値を取得または設定します<br/>            プロジェクトがグラフィック形式で保存されるとき。<br/>            ページサイズが変更され、レンダリングされたプロジェクトが1ページに収まるようになります。 |
| reduce_footer_gap | 最後のタスクとフッター間のギャップを縮小すべきかどうかを示す値を取得または設定します。 |
| compliance | 生成された PDF ドキュメントの希望する準拠レベルを取得または設定します。<br/>            デフォルトは [PDF15](/tasks/python-net/aspose.tasks.saving/pdfcompliance/) です。 |
| encryption_details | 暗号化の詳細を取得または設定します。設定されていない場合、暗号化は行われません。 |
| text_compression | 画像を除くすべてのコンテンツ ストリームに使用される圧縮タイプを取得または設定します。<br/>            デフォルトは [FLATE](/tasks/python-net/aspose.tasks.saving/pdftextcompression/) です。 |
| digital_signature_details | デジタル署名の詳細を取得または設定します。設定されていない場合、署名は行われません。 |
| save_to_separate_files | プロジェクトページを別々のファイルに保存するかどうかを示す値を取得または設定します。 |
| page_saving_callback | 各レンダリングページの出力ストリームを取得するために使用されるユーザー定義コールバックを取得または設定します。<br/>            [save_to_separate_files](/tasks/python-net/aspose.tasks.saving/pdfsaveoptions/) オプションが使用されている場合に適用されます。 |
| pages | プロジェクトレイアウトを別々のファイルに保存する際に、保存するページ番号のリストを取得または設定します。 |
| font_settings | プロジェクトのビューをレンダリングする際に使用されるフォント設定を指定します。 |

### 関連項目

* namespace [aspose.tasks.saving](/tasks/python-net/aspose.tasks.saving/)
* assembly [Aspose.Tasks](/tasks/python-net/)

