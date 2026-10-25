---
title: "Calendar"
second_title: "Aspose.Tasks for Python via .NET API リファレンス"
description: 
type: docs
weight: 140
url: /ja/python-net/aspose.tasks/calendar/
---

## Calendar class

プロジェクトで使用されるカレンダーを表します。

Calendar 型は次のメンバーを公開します：
## プロパティ
| 名前 | 説明 |
| :- | :- |
| name | カレンダーの名前を取得または設定します。 |
| uid | カレンダーの一意の識別子を取得または設定します。 |
| week_days | このカレンダーの WeekDaysCollection を取得します。<br/>            カレンダーを定義する平日のコレクションです。 |
| exceptions | CalendarExceptionCollection オブジェクトを取得します。<br/>            カレンダーに関連付けられた例外のコレクションです。 |
| work_weeks | WorkWeekCollections オブジェクトを取得します。<br/>            カレンダーに関連付けられた作業週のコレクションです。 |
| is_base_calendar | カレンダーがベースカレンダーかどうかを示す値を取得します。 |
| base_calendar | このカレンダーが依存するベースカレンダーを取得または設定します。<br/>            カレンダーがベースカレンダーでない場合にのみ適用されます。 |
| is_baseline_calendar | カレンダーがベースラインカレンダーかどうかを示す値を取得または設定します。 |
| guid | カレンダーの Guid を取得します。 |
| Primavera プロパティ | Primavera 形式から読み込んだカレンダーの Primavera 固有プロパティを含むオブジェクトを取得します。 |
## メソッド
| 名前 | 説明 |
| :- | :- |
| get_start_date_from_finish_and_duration(finish, duration) | 指定された終了日と期間に基づいて開始日を返します。 |
| get_start_date_from_finish_and_duration(finish, duration) | 指定された終了日と期間に基づいて開始日を返します。 |
| get_working_hours(start, finish) | 指定された日時間隔の作業時間の開始、終了、および期間を表す WorkUnit を返します。 |
| get_working_hours(dt) | 指定された日時間隔の作業時間の開始、終了、および期間を表す WorkUnit を返します。 |
| get_finish_date_by_start_and_work(start, work) | カレンダーに従って、指定された作業時間が経過する日時を計算します。 |
| get_finish_date_by_start_and_work(start, work) | カレンダーに従って、指定された作業時間が経過する日時を計算します。 |
| get_intersection_calendar(calendar1, calendar2) | 2 つのカレンダーの作業スケジュールの交差点で計算を実行できる [ICalendar](/tasks/python-net/aspose.tasks/icalendar/) インスタンスを取得します。 |
| make_standard_calendar(calendar) | デフォルトの標準カレンダーを作成します。 |
| make_24_hour_calendar(calendar) | 指定されたカレンダーを 24 時間カレンダーにします。<br/>            24Hours カレンダーは、週のすべての日が 24 時間体制で稼働するカレンダーです。 |
| make_night_shift_calendar(calendar) | 指定されたカレンダーを夜勤シフトカレンダーにします。 |
| delete() | プロジェクトからカレンダーを削除します。 |
| is_day_working(dt) | カレンダーに従って、指定された日が稼働日かどうかを判定します。 |
| get_working_hours_time_span(start, finish) | 指定された日付間の稼働時間の量を返します。 |
| get_task_finish_date_from_duration(task, duration) | 開始日、分割部分、および作業期間からタスクの終了日時を計算します。 |
| get_working_times(dt) | 指定された日の作業時間の [WorkingTimeCollection](/tasks/python-net/aspose.tasks/workingtimecollection/) を返します。 |
| get_previous_working_day_end(date) | 指定された日付から前の稼働日の終了時刻を計算します。 |
| get_next_working_day_start(date) | 指定された日付の次の稼働日の開始時刻を計算します。 |
| get_work_start(date) | 指定された日付と時刻から始まる次の稼働時間の開始時刻を計算します。 |
| is_empty() | カレンダーに稼働時間が定義されていないかどうかを返します。 |

### 関連項目

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

