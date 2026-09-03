---
title: "Aspose::Tasks::Saving::SaveOptions クラス"
linktitle: "SaveOptions"
articleTitle: "SaveOptions"
second_title: "Aspose.Tasks for C++"
description: "これは、プロジェクトを特定の形式で保存する際に、ユーザーが追加オプションを指定できるようにするクラスの抽象基底クラスです。"
type: docs
weight: 10
url: /ja/cpp/aspose.tasks.saving/saveoptions/
---

## SaveOptions class

**Inherits:** Aspose::Tasks::Saving::SimpleSaveOptions

これは、プロジェクトを特定の形式で保存する際に、ユーザーが追加オプションを指定できるようにするクラスの抽象基底クラスです。

SaveOptions クラスから派生した任意のクラスのインスタンスは、ドキュメントを保存する際にユーザーがカスタムオプションを定義できるよう、ストリーム Save または文字列 Save のオーバーロードに渡されます。

## メソッド

| 名前 | 説明 |
| --- | --- |
| [get_BarStyles](./get_barstyles/) | プロジェクトビューに表示される BarStyle クラスのインスタンスの一覧を取得します。 |
| [get_CustomPageSize](./get_custompagesize/) | ポイント単位（1 ポイント = 1/72 インチ）のカスタムページサイズを取得します。 |
| [get_DrawNonWorkingTime](./get_drawnonworkingtime/) | 非稼働時間を描画するかどうかを示す値を取得します（既定値は TRUE）。 |
| [get_EndDate](./get_enddate/) | レンダリングを終了する日付を取得します。 |
| [get_FitContent](./get_fitcontent/) | 行の高さを内容に合わせて拡大するかどうかを示す値を取得します。 |
| [get_FitTimescaleToEndOfPage](./get_fittimescaletoendofpage/) | ビューのカレンダーセクションを最終ページの末端（右側）まで描画するかどうかを取得します。値が false の場合、ページに空白があってもカレンダーセクションは EndDate まで正確に描画されます。 |
| [get_Gridlines](./get_gridlines/) | プロジェクトビューに表示される Gridline の一覧を取得します。 |
| [get_IsPortrait](./get_isportrait/) | ページの向きが縦向きかどうかを示す値を取得します。横向きの場合は false を返します。 |
| [get_LegendDrawingOptions](./get_legenddrawingoptions/) | 凡例の描画方法を定義する値を取得します。既定値は LegendDrawingOptions.OnEveryPage です。 |
| [get_LegendItems](./get_legenditems/) | ページ凡例に描画すべきバーを定義する PageLegendItem の配列を取得します。null の場合、既定の項目が描画されます。 |
| [get_MarkCriticalTasks](./get_markcriticaltasks/) | 重要タスクを赤色で表示するかどうかを示す値を取得します（既定値は FALSE）。 |
| [get_NonWorkingTimeColor](./get_nonworkingtimecolor/) | 非稼働時間の色を取得します。 |
| [get_PageCount](./get_pagecount/) | プロジェクトのページ数を取得します。 |
| [get_PageSize](./get_pagesize/) | レンダリングされるページサイズを取得します（既定値は PageSize.A4）。 |
| [get_PresentationFormat](./get_presentationformat/) | ドキュメントが保存される PresentationFormat を取得します。 |
| [get_RenderToSinglePage](./get_rendertosinglepage/) | プロジェクトがグラフィカル形式で保存される際に、単一ページにレンダリングするかどうかを示す値を取得します。ページサイズは、レンダリングされたプロジェクトが1ページに収まるように変更されます。 |
| [get_RollUpGanttBars](./get_rollupganttbars/) | サマリタスクバー上のサブタスクにマークを付けるかどうかを示す値を取得します。サブタスクの場合、Rollup フィールドはサブタスクのガントバー情報がサマリタスクバーに集約されるかどうかを示します。サマリタスクの場合、Rollup フィールドはサマリタスクバーが集約されたバーを表示するかどうかを示します。サブタスクを集約させるには、サマリタスクの Rollup フィールドを Yes に設定する必要があります。 |
| [get_StartDate](./get_startdate/) | レンダリングを開始する日付を取得します。 |
| [get_TextStyles](./get_textstyles/) | プロジェクトビューのレンダリング中に適用されるテキストスタイルの一覧を取得します。 |
| [get_Timescale](./get_timescale/) | プロジェクトがグラフィカル形式で保存される際に、タイムスケール（存在する場合）の描画方法を制御するために使用される Timescale 値を取得します。 |
| [get_TimescaleFitBehavior](./get_timescalefitbehavior/) | タイムスケールの右端をページの末端に合わせる方法を定義する動作を取得します。 |
| [get_UseGradientBrush](./get_usegradientbrush/) | ガントチャートのレンダリング時にグラデーションブラシを使用するかどうかを示す値を取得します。 |
| [get_View](./get_view/) | レンダリングするビュー列のリストを取得します（ GanttChartColumn ）。設定されていない場合は、タスクID、タスク名、開始日と終了日だけがレンダリングされます。View と ViewSettings の両方のプロパティが設定されている場合、View の列が ViewSettings の列を上書きします。 |
| [get_ViewSettings](./get_viewsettings/) | レンダリングするビュー（ View ）を取得します。このオプションを使用して、PDF、HTML、または画像形式で保存すべきビューを明示的に指定できます。このプロパティが設定されている場合、プロジェクトを保存するときに Visualization::PresentationFormat プロパティは無視されます。ビューは次のいずれかの画面（ (( Aspose::Tasks::View::Screen ))）から選択する必要があります：（Gantt、TaskSheet、TaskUsage、ResourceSheet、ResourceUsage）。 |
| [set_BarStyles](./set_barstyles/) | プロジェクトビューに表示される BarStyle クラスのインスタンスのリストを設定します。 |
| [set_CustomPageSize](./set_custompagesize/) | カスタムページサイズをポイント単位で設定します（1ポイント = 1/72 インチ）。 |
| [set_DrawNonWorkingTime](./set_drawnonworkingtime/) | 非稼働時間を描画するかどうかを示す値を設定します（デフォルト値は TRUE）。 |
| [set_EndDate](./set_enddate/) | レンダリングの終了日を設定します。 |
| [set_FitContent](./set_fitcontent/) | 行の高さを内容に合わせて拡大するかどうかを示す値を設定します。 |
| [set_FitTimescaleToEndOfPage](./set_fittimescaletoendofpage/) | ビューのカレンダーセクションを最終ページの末尾（右側）までレンダリングするかどうかを設定します。値が false の場合、ページに空白が残っていてもカレンダーセクションは EndDate まで正確にレンダリングされます。 |
| [set_Gridlines](./set_gridlines/) | プロジェクトビューに表示される Gridline のリストを設定します。 |
| [set_IsPortrait](./set_isportrait/) | ページの向きが縦向きかどうかを示す値を設定します。ページの向きが横向きの場合は false を返します。 |
| [set_LegendDrawingOptions](./set_legenddrawingoptions/) | 凡例の描画方法を定義する値を設定します。デフォルト値は LegendDrawingOptions.OnEveryPage です。 |
| [set_LegendItems](./set_legenditems/) | ページ凡例にレンダリングすべきバーを定義する PageLegendItem の配列を設定します。null の場合、デフォルト項目がレンダリングされます。 |
| [set_MarkCriticalTasks](./set_markcriticaltasks/) | 重要タスクを赤色で表示するかどうかを示す値を設定します（デフォルト値は FALSE）。 |
| [set_NonWorkingTimeColor](./set_nonworkingtimecolor/) | 非稼働時間の色を設定します。 |
| [set_PageSize](./set_pagesize/) | レンダリングするページサイズを設定します（デフォルト値は PageSize.A4）。 |
| [set_PresentationFormat](./set_presentationformat/) | ドキュメントが保存される PresentationFormat を設定します。 |
| [set_RenderToSinglePage](./set_rendertosinglepage/) | プロジェクトがグラフィカル形式で保存される際に、単一ページにレンダリングするかどうかを示す値を設定します。ページサイズは、レンダリングされたプロジェクトが1ページに収まるように変更されます。 |
| [set_RollUpGanttBars](./set_rollupganttbars/) | サマリタスクバー上のサブタスクにマークを付けるかどうかを示す値を設定します。サブタスクの場合、Rollup フィールドはサブタスクのガントバーの情報がサマリタスクバーにロールアップされるかどうかを示します。サマリタスクの場合、Rollup フィールドはサマリタスクバーがロールアップされたバーを表示するかどうかを示します。サブタスクをロールアップさせるには、サマリタスクの Rollup フィールドを Yes に設定しておく必要があります。 |
| [set_StartDate](./set_startdate/) | レンダリング開始日を設定します。 |
| [set_TextStyles](./set_textstyles/) | プロジェクトビューのレンダリング時に適用されるテキストスタイルのリストを設定します。 |
| [set_Timescale](./set_timescale/) | プロジェクトがグラフィカル形式で保存される際に、タイムスケール（存在する場合）の描画方法を制御するために使用される Timescale の値を設定します。 |
| [set_TimescaleFitBehavior](./set_timescalefitbehavior/) | タイムスケールの右端をページの端に合わせる方法を定義する動作を設定します。 |
| [set_UseGradientBrush](./set_usegradientbrush/) | ガントチャートのレンダリング時にグラデーションブラシを使用するかどうかを示す値を設定します。 |
| [set_View](./set_view/) | レンダリングするビュー列のリストを設定します（ GanttChartColumn ）。設定されていない場合は、タスクID、タスク名、開始日と終了日だけがレンダリングされます。View と ViewSettings の両方のプロパティが設定されている場合、View の列が ViewSettings の列を上書きします。 |
| [set_ViewSettings](./set_viewsettings/) | レンダリングするビュー（ View ）を設定します。このオプションを使用して、PDF、HTML、または画像形式で保存すべきビューを明示的に指定できます。このプロパティが設定されている場合、プロジェクトを保存するときに Visualization::PresentationFormat プロパティは無視されます。ビューは次のいずれかの画面（ (( Aspose::Tasks::View::Screen ))）から選択する必要があります：（Gantt、TaskSheet、TaskUsage、ResourceSheet、ResourceUsage）。 |

