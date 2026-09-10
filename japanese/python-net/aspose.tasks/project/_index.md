---
title: "プロジェクト"
second_title: "Aspose.Tasks for Python via .NET API リファレンス"
description: 
type: docs
weight: 810
url: /ja/python-net/aspose.tasks/project/
---

## Project class

プロジェクトを表します。

Project 型は次のメンバーを公開します：
## コンストラクタ
| 名前 | 説明 |
| :- | :- |
| Project() | 新しい [Project](/tasks/python-net/aspose.tasks/project/) クラスのインスタンスを初期化します。 |
| Project(project_template, protection_password) | パスワードで保護されたテンプレート（既存の mpp または mpt ファイル）から新しい [Project](/tasks/python-net/aspose.tasks/project/) クラスのインスタンスを初期化します。 |
| Project(project_template) | パスワードで保護されたテンプレート（既存の mpp または mpt ファイル）から新しい [Project](/tasks/python-net/aspose.tasks/project/) クラスのインスタンスを初期化します。 |
| Project(stream, options) | ストリームから新しい [Project](/tasks/python-net/aspose.tasks/project/) クラスのインスタンスを初期化します<br/>            指定された [PrimaveraReadOptions](/tasks/python-net/aspose.tasks/primaverareadoptions/) クラスのインスタンスと共に。 |
| Project(stream) | ストリームから新しい [Project](/tasks/python-net/aspose.tasks/project/) クラスのインスタンスを初期化します<br/>            指定された [PrimaveraReadOptions](/tasks/python-net/aspose.tasks/primaverareadoptions/) クラスのインスタンスと共に。 |
| Project(project_template, options) | テンプレート（既存の MPP または MPT ファイル）から新しい [Project](/tasks/python-net/aspose.tasks/project/) クラスのインスタンスを初期化します <br/>            指定された [PrimaveraReadOptions](/tasks/python-net/aspose.tasks/primaverareadoptions/) クラスのインスタンスと共に。 |
| Project(settings) | データベースからデータを読み取るために、新しい [Project](/tasks/python-net/aspose.tasks/project/) クラスのインスタンスを初期化します。データベースは [DbSettings](/tasks/python-net/aspose.tasks.connectivity/dbsettings/) クラスのインスタンスで指定されます。 |
| Project(stream, protection_password) | テンプレート（既存の mpp または mpt ファイル）から新しい [Project](/tasks/python-net/aspose.tasks/project/) クラスのインスタンスを初期化します。 |
| Project(project_template, options) | テンプレート（既存の mpp または mpt ファイル）から新しい [Project](/tasks/python-net/aspose.tasks/project/) クラスのインスタンスを初期化します<br/>            指定された [LoadOptions](/tasks/python-net/aspose.tasks/loadoptions/) クラスのインスタンスと共に。 |
| Project(stream, options) | ストリームから新しい [Project](/tasks/python-net/aspose.tasks/project/) クラスのインスタンスを初期化します<br/>            指定された [LoadOptions](/tasks/python-net/aspose.tasks/loadoptions/) クラスのインスタンスと共に。 |
## プロパティ
| 名前 | 説明 |
| :- | :- |
| actuals_in_sync | ActualsInSync が設定されているかどうかを示す値を取得または設定します。 |
| admin_project | AdminProject が設定されているかどうかを示す値を取得または設定します。 |
| are_editable_actual_costs | AreEditableActualCosts が設定されているかどうかを示す値を取得または設定します。 |
| author | Author の値を取得または設定します。 |
| auto_add_new_resources_and_tasks | AutoAddNewResourcesAndTasks が設定されているかどうかを示す値を取得または設定します。 |
| autolink | Autolink が設定されているかどうかを示す値を取得または設定します。 |
| baseline_for_earned_value | BaselineForEarnedValue の値を取得または設定します。 |
| calendar | Calendar の値を取得または設定します。 |
| category | Category の値を取得または設定します。 |
| comments | Comments の値を取得または設定します。 |
| company | Company の値を取得または設定します。 |
| creation_date | CreationDate の値を取得または設定します。 |
| critical_slack_limit | MS Project では、総スラックがこの日数以下の場合、タスクはクリティカルと見なされます。 |
| currency_code | CurrencyCode の値を取得または設定します。 |
| currency_digits | CurrencyDigits の値を取得または設定します。 |
| currency_symbol | CurrencySymbol の値を取得または設定します。 |
| currency_symbol_position | CurrencySymbolPosition の値を取得または設定します。 |
| current_date | CurrentDate の値を取得または設定します。 |
| date_format | DateFormat の値を取得または設定します。 |
| custom_date_format | CustomDateFormat の値を取得または設定します。 |
| days_per_month | DaysPerMonth の値を取得または設定します。 |
| default_finish_time | DefaultFinishTime の値を取得または設定します。 |
| default_fixed_cost_accrual | DefaultFixedCostAccrual の値を取得または設定します。 |
| default_overtime_rate | DefaultOvertimeRate の値を取得または設定します。 |
| default_standard_rate | DefaultStandardRate の値を取得または設定します。 |
| default_start_time | DefaultStartTime の値を取得または設定します。 |
| default_task_ev_method | DefaultTaskEVMethod の値を取得または設定します。 |
| default_task_type | DefaultTaskType の値を取得または設定します。 |
| duration_format | DurationFormat の値を取得または設定します。 |
| earned_value_method | EarnedValueMethod の値を取得または設定します。 |
| extended_creation_date | ExtendedCreationDate の値を取得または設定します。 |
| finish_date | FinishDate の値を取得または設定します。 |
| fiscal_year_start | FiscalYearStart が設定されているかどうかを示す値を取得または設定します。 |
| fy_start_date | FyStartDate の値を取得または設定します。 |
| honor_constraints | HonorConstraints が設定されているかどうかを示す値を取得または設定します。 |
| hyperlink_base | HyperlinkBase の値を取得または設定します。 |
| inserted_projects_like_summary | InsertedProjectsLikeSummary が設定されているかどうかを示す値を取得または設定します。 |
| keep_task_on_nearest_working_time_when_made_auto_scheduled | KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled が設定されているかどうかを示す値を取得または設定します。 |
| keywords | Keywords の値を取得または設定します。 |
| last_author | LastAuthor の値を取得または設定します。 |
| last_printed | LastPrinted の値を取得または設定します。 |
| last_saved | LastSaved の値を取得または設定します。 |
| manager | Manager の値を取得または設定します。 |
| microsoft_project_server_url | MicrosoftProjectServerURL が設定されているかどうかを示す値を取得または設定します。 |
| minutes_per_day | MinutesPerDay の値を取得または設定します。 |
| minutes_per_week | MinutesPerWeek の値を取得または設定します。 |
| move_completed_ends_back | MoveCompletedEndsBack が設定されているかどうかを示す値を取得または設定します。 |
| move_completed_ends_forward | MoveCompletedEndsForward が設定されているかどうかを示す値を取得または設定します。 |
| move_remaining_starts_back | MoveRemainingStartsBack が設定されているかどうかを示す値を取得または設定します。 |
| move_remaining_starts_forward | MoveRemainingStartsForward が設定されているかどうかを示す値を取得または設定します。 |
| multiple_critical_paths | MultipleCriticalPaths が設定されているかどうかを示す値を取得または設定します。 |
| name | Name の値を取得または設定します。 |
| new_tasks_are_manual | NewTasksAreManual が設定されているかどうかを示す値を取得または設定します。 |
| new_tasks_effort_driven | NewTasksEffortDriven が設定されているかどうかを示す値を取得または設定します。 |
| new_tasks_estimated | NewTasksEstimated が設定されているかどうかを示す値を取得または設定します。 |
| new_task_start_date | NewTaskStartDate の値を取得または設定します。 |
| project_externally_edited | ProjectExternallyEdited が設定されているかどうかを示す値を取得または設定します。 |
| remove_file_properties | RemoveFileProperties が設定されているかどうかを示す値を取得または設定します。 |
| revision | Revision の値を取得または設定します。 |
| save_version | SaveVersion の値を取得または設定します。 |
| schedule_from_start | ScheduleFromStart が設定されているかどうかを示す値を取得または設定します。 |
| show_project_summary_task | ShowProjectSummaryTask が設定されているかどうかを示す値を取得または設定します。 |
| splits_in_progress_tasks | SplitsInProgressTasks が設定されているかどうかを示す値を取得または設定します。 |
| spread_actual_cost | SpreadActualCost が設定されているかどうかを示す値を取得または設定します。 |
| spread_percent_complete | SpreadPercentComplete が設定されているかどうかを示す値を取得または設定します。 |
| start_date | StartDate の値を取得または設定します。 |
| status_date | StatusDate の値を取得または設定します。 |
| subject | Subject の値を取得または設定します。 |
| task_updates_resource | TaskUpdatesResource が設定されているかどうかを示す値を取得または設定します。 |
| テンプレート | Template の値を取得または設定します。 |
| timescale_finish | TimescaleFinish の値を取得または設定します。 |
| timescale_start | TimescaleStart の値を取得または設定します。 |
| title | Title の値を取得または設定します。 |
| uid | Uid の値を取得または設定します。 |
| update_manually_scheduled_tasks_when_editing_links | UpdateManuallyScheduledTasksWhenEditingLinks が設定されているかどうかを示す値を取得または設定します。 |
| week_start_day | WeekStartDay の値を取得または設定します。 |
| work_format | WorkFormat の値を取得または設定します。 |
| guid | Guid の値を取得または設定します。 |
| auto_calculate_assignment_costs | 割り当ての作業とリソースレートを使用して、割り当てコストと残りコストを自動的に計算するかどうかを取得または設定します。 |
| default_view | プロジェクトのデフォルトビューを取得または設定します。 |
| vba_project | [vba_project](/tasks/python-net/aspose.tasks/project/) クラスのインスタンスを取得します。 |
| display_options | [ProjectDisplayOptions](/tasks/python-net/aspose.tasks/projectdisplayoptions/) クラスのインスタンスを取得します。 |
| calculation_mode | プロジェクトの計算モードを取得または設定します。<br/>            [calculation_mode](/tasks/python-net/aspose.tasks/project/) 列挙体の値のいずれかです。 |
| root_task | タスクツリーのルートを取得します。 |
| task_links | [TaskLinkCollection](/tasks/python-net/aspose.tasks/tasklinkcollection/) オブジェクトを取得します。 |
| calendars | この Project インスタンスの [CalendarCollection](/tasks/python-net/aspose.tasks/calendarcollection/) オブジェクトを取得します。 |
| リソース | ResourceCollection オブジェクトを取得します。 |
| アウトラインコード | OutlineCodeDefinitionCollection オブジェクトを取得します。<br/>            プロジェクトに関連付けられたアウトラインコード定義のコレクションです。 |
| リソース割り当て | ResourceAssignmentCollection オブジェクトを取得します。 |
| default_week_working_days | プロジェクトのデフォルトの週の作業日と作業時間のコレクションを表す [WeekDayCollection](/tasks/python-net/aspose.tasks/weekdaycollection/) クラスのインスタンスを取得します。 |
| 組み込みプロパティ | プロジェクトの組み込みプロパティコレクションを取得します。 |
| カスタムプロパティ | プロジェクトのカスタムプロパティコレクションを取得します。 |
| extended_attributes | ExtendedAttributeDefinitionCollection オブジェクトを取得します。<br/>            プロジェクトに関連付けられた拡張属性（カスタムフィールド）定義のコレクションです。 |
| クリティカルパス | このプロジェクトのクリティカルパスを構成するクリティカルタスクのリストを含むコレクションを取得します。 |
| task_filters | タスクベースのフィルター定義をすべて取得します。 <br/>            TaskFilters は [Filter](/tasks/python-net/aspose.tasks/filter/) オブジェクトのコレクションです。 |
| resource_filters | リソースベースのフィルター定義をすべて取得します。 <br/>            ResourceFilters は [Filter](/tasks/python-net/aspose.tasks/filter/) オブジェクトのコレクションです。 |
| views | [View](/tasks/python-net/aspose.tasks/view/) オブジェクトのリストを取得します。 |
| tables | [Table](/tasks/python-net/aspose.tasks/table/) オブジェクトのリストを取得します。 |
| task_groups | タスクベースのグループ定義をすべて取得します。 <br/>            TaskGroups は [Group](/tasks/python-net/aspose.tasks/group/) オブジェクトのコレクションです。 |
| resource_groups | リソースベースのグループ定義をすべて取得します。 <br/>            ResourceGroups は [Group](/tasks/python-net/aspose.tasks/group/) オブジェクトのコレクションです。 |
| WBS コード定義 | プロジェクトの WBS コード定義を取得または設定します。 |
| ole_objects | このプロジェクト ファイルにリンクまたは埋め込まれている [OleObject](/tasks/python-net/aspose.tasks/oleobject/) クラスのインスタンスを含むコレクションを取得します。 |
| Primavera プロパティ | Primavera ファイルから読み取ったプロジェクトの Primavera 固有プロパティを含むオブジェクトを取得します。 |
| globalization_settings | プロジェクトのグローバリゼーション（言語固有）設定を取得または設定します。 |
## メソッド
| 名前 | 説明 |
| :- | :- |
| get_project_file_info(filename) | ファイルからプロジェクトファイル情報を読み取ります。 |
| get_project_file_info(stream) | ストリームからプロジェクトファイル情報を取得します。 |
| recalculate() | リソースの開始日と終了日を再計算します。 |
| recalculate(validate) | すべてのプロジェクトタスクID、アウトラインレベル、開始/終了日を再スケジュールし、早期/遅延日を設定し、スラック、作業およびコストフィールドをオプションの検証とともに計算します。 |
| save(filename, options) | 指定された保存オプションを使用して、ドキュメントをファイルに保存します。 |
| save(filename, format) | プロジェクトデータをファイルに保存します。 |
| save(filename) | 指定された保存オプションを使用して、ドキュメントをファイルに保存します。 |
| save(stream, options) | 指定された保存オプションを使用して、プロジェクトをストリームに保存します。 |
| save(stream, format) | プロジェクトデータをストリームに保存します。 |
| save_report(stream) | プロジェクト概要レポートをストリームに保存します。 |
| save_report(file_name) | プロジェクト概要レポートをPDFファイルに保存します。 |
| save_report(stream, report_type) | 指定されたタイプのプロジェクトレポートを指定されたストリームに保存します。 |
| save_report(file_name, report_type) | 指定されたタイプのプロジェクトレポートを PDF 形式で、指定されたファイルパスに保存します。 |
| save_as_template(file_name, options) | プロジェクトをテンプレートとして保存します。 |
| save_as_template(file_name) | プロジェクトをテンプレートとして保存します。 |
| save_as_template(stream) | プロジェクトをテンプレートとして、指定されたストリームに保存します。 |
| save_as_template(stream, options) | プロジェクトをテンプレートとして、指定されたストリームに保存します。 |
| get_page_count(save_options) | 指定された [SaveOptions](/tasks/python-net/aspose.tasks.saving/saveoptions/) を使用してレンダリングされるプロジェクトのページ数を返します。 |
| get_page_count() | 指定された [SaveOptions](/tasks/python-net/aspose.tasks.saving/saveoptions/) を使用してレンダリングされるプロジェクトのページ数を返します。 |
| get_page_count(scale) | 指定された [Timescale](/tasks/python-net/aspose.tasks.visualization/timescale/) を使用してレンダリングされるプロジェクトのページ数を返します。 |
| get_page_count(format) | デフォルトの [Timescale](/tasks/python-net/aspose.tasks.visualization/timescale/)(Days) と指定された [PresentationFormat](/tasks/python-net/aspose.tasks.visualization/presentationformat/) を使用してレンダリングされるプロジェクトのページ数を返します。 |
| get_page_count(format, scale) | 指定された [Timescale](/tasks/python-net/aspose.tasks.visualization/timescale/) と [PresentationFormat](/tasks/python-net/aspose.tasks.visualization/presentationformat/) を使用してレンダリングされるプロジェクトのページ数を返します。 |
| get_page_count(page_size, scale, start_date, end_date) | 指定された [Timescale](/tasks/python-net/aspose.tasks.visualization/timescale/)、[PresentationFormat](/tasks/python-net/aspose.tasks.visualization/presentationformat/) および日付範囲を使用してレンダリングされるプロジェクトのページ数を返します。 |
| get_page_count(page_size, scale) | 指定された [Timescale](/tasks/python-net/aspose.tasks.visualization/timescale/)、[PresentationFormat](/tasks/python-net/aspose.tasks.visualization/presentationformat/) および日付範囲を使用してレンダリングされるプロジェクトのページ数を返します。 |
| copy_to(another) | プロジェクトの主要データとプロパティを別のプロジェクトにコピーします。 |
| copy_to(another, options) | プロジェクトの主要データとプロパティを別のプロジェクトにコピーします。 |
| print() | 標準（ユーザーインターフェイスなし）印刷コントローラを使用して、デフォルトのプリンター設定でプロジェクトをデフォルトプリンターに印刷します。 |
| print(options) | 標準（ユーザーインターフェイスなし）印刷コントローラを使用して、デフォルトのプリンター設定とカスタム保存オプションでプロジェクトをデフォルトプリンターに印刷します。 |
| print(printer_name) | 標準（ユーザーインターフェイスなし）印刷コントローラを使用して、デフォルトのプリンター設定で指定されたプリンターにプロジェクトを印刷します。 |
| print(printer_settings) | 標準（ユーザーインターフェイスなし）印刷コントローラを使用して、指定されたプリンター設定に従ってプロジェクトを印刷します。 |
| print(printer_settings, document_name) | 標準（ユーザーインターフェイスなし）印刷コントローラを使用して、指定されたプリンター設定に従ってプロジェクトを印刷します。 |
| print(printer_settings, options) | 指定されたプリンター設定とカスタム保存オプションに従って、標準（ユーザーインターフェイスなし）印刷コントローラを使用してプロジェクトを印刷します。 |
| print(printer_settings, options, document_name) | 指定されたプリンター設定、カスタム保存オプション、および指定されたドキュメント名に従って、標準（ユーザーインターフェイスなし）印刷コントローラを使用してプロジェクトを印刷します。 |
| set_baseline(baseline_type) | ベースラインの保存時刻を設定します。 |
| set_baseline(baseline_type, task_collection) |  |
| update_project_work_as_complete(complete_through, set_zero_or_hundred_percent_complete_only) | プロジェクト全体の作業を、指定された日付まで完了として更新します。 |
| update_project_work_as_complete(complete_through, set_zero_or_hundred_percent_complete_only, task_collection) |  |
| reschedule_uncompleted_work_to_start_after(after) | 未完了のプロジェクト作業を、指定された日付以降に開始するように再スケジュールします。 |
| reschedule_uncompleted_work_to_start_after(after, task_collection) |  |
| renumber_wbs_code() | すべてのタスクの WBS コードを再番号付けします。 |
| renumber_wbs_code(task_ids) |  |
| get_duration(val) | プロジェクトの設定 [None](/tasks/python-net/aspose.tasks/prj/) で定義されているデフォルトの期間形式と、指定された単位数を持つ [Duration](/tasks/python-net/aspose.tasks/duration/) オブジェクトを取得します。 |
| get_duration(val, time_unit) | 指定された数の [TimeUnitType](/tasks/python-net/aspose.tasks/timeunittype/) 単位を持つ [Duration](/tasks/python-net/aspose.tasks/duration/) オブジェクトを取得します。 |
| get_duration(time_span, time_unit) | 指定された datetime 値と指定された [TimeUnitType](/tasks/python-net/aspose.tasks/timeunittype/) 値を持つ [Duration](/tasks/python-net/aspose.tasks/duration/) オブジェクトを取得します。 |
| select_all_child_tasks() | ルートタスクのすべての子タスクを再帰的に収集します。 |
| enumerate_all_child_tasks() | ルートタスクを含むプロジェクトのすべてのタスクを再帰的に列挙します。 |
| get_predecessors(task) | 指定されたタスクの前任タスクリンクのコレクションを返します。 |
| recalculate_resource_start_finish() | リソースの開始日と終了日を再計算します。 |
| recalculate_resource_fields() | リソースの Id、開始日、終了日を再計算します。 |
| remove_invalid_resource_assignments() | プロジェクトのリソース割り当てリストから無効なリソース割り当てを削除します。 |
| get_baseline_save_time(baseline_number) | ベースラインの保存時刻を返します。 |
| set_baseline_save_time(baseline_number, value) | ベースラインの保存時刻を設定します。 |
| get_work(val) | 指定された浮動小数点値とデフォルトの作業形式で [Duration](/tasks/python-net/aspose.tasks/duration/) オブジェクトを取得します。 |

### 関連項目

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

