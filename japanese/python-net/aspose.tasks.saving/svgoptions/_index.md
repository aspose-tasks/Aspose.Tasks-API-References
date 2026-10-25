---
title: "SvgOptions"
second_title: "Aspose.Tasks for Python via .NET API リファレンス"
description: 
type: docs
weight: 170
url: /ja/python-net/aspose.tasks.saving/svgoptions/
---

## SvgOptions class

プロジェクトページを SVG にレンダリングする際に、追加オプションを指定できます。

SvgOptions 型は次のメンバーを公開します:
## コンストラクタ
| 名前 | 説明 |
| :- | :- |
| SvgOptions() | [SvgOptions](/tasks/python-net/aspose.tasks.saving/svgoptions/) クラスの新しいインスタンスを初期化します。このインスタンスはプロジェクトを SVG 形式で保存するために使用できます。 |
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
| use_gradient_brush | プロジェクトレイアウトをレンダリングする際にグラデーションブラシを使用するかどうかを決定します。 |
| view | 描画するビュー列のリストを取得または設定します（[GanttChartColumn](/tasks/python-net/aspose.tasks.visualization/ganttchartcolumn/)）。<br/>            設定されていない場合、タスク ID、タスク名、開始日と終了日だけが描画されます。<br/>            View と [view_settings](/tasks/python-net/aspose.tasks.saving/saveoptions/) の両方のプロパティが設定されている場合、View の列が ViewSettings の列を上書きします。 |
| view_settings | 描画するビュー ([view](/tasks/python-net/aspose.tasks.saving/saveoptions/)) を取得または設定します。このオプションを使用して、PDF、HTML、または画像形式で保存すべきビューを明示的に指定できます。<br/>            このプロパティが設定されている場合、プロジェクトが保存される際に [PresentationFormat](/tasks/python-net/aspose.tasks.visualization/presentationformat/) プロパティは無視されます。<br/>            ビューは次のいずれかの画面から選択する必要があります (([screen](/tasks/python-net/aspose.tasks/view/))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage) |
| custom_page_size | ポイント単位でカスタムページサイズを取得または設定します（1ポイント = 1/72インチ）。 |
| render_to_single_page | プロジェクトを単一ページにレンダリングすべきかどうかを示す値を取得または設定します<br/>            プロジェクトがグラフィック形式で保存されるとき。<br/>            ページサイズが変更され、レンダリングされたプロジェクトが1ページに収まるようになります。 |
| page_saving_callback | 各レンダリングページの出力ストリームを取得するために使用される、ユーザー定義の実装コールバックを取得または設定します。 |

### 関連項目

* namespace [aspose.tasks.saving](/tasks/python-net/aspose.tasks.saving/)
* assembly [Aspose.Tasks](/tasks/python-net/)

