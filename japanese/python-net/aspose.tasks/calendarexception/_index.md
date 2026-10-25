---
title: "CalendarException"
second_title: "Aspose.Tasks for Python via .NET API リファレンス"
description: 
type: docs
weight: 160
url: /ja/python-net/aspose.tasks/calendarexception/
---

## CalendarException class

カレンダー内の例外的な期間を表します。

CalendarException 型は次のメンバーを公開します：
## コンストラクタ
| 名前 | 説明 |
| :- | :- |
| CalendarException() | 新しい [CalendarException](/tasks/python-net/aspose.tasks/calendarexception/) クラスのインスタンスを初期化します。 |
## プロパティ
| 名前 | 説明 |
| :- | :- |
| entered_by_occurrences | 繰り返し範囲が発生回数の入力によって定義されているかどうかを示す値を取得または設定します。<br/>            False は、繰り返し範囲が終了日を入力して定義されていることを指定します。 |
| from_date | 例外の開始時刻を取得または設定します。 |
| to_date | 例外の終了時刻を取得または設定します。 |
| occurrences | カレンダー例外が有効な発生回数を取得または設定します。 |
| name | 例外の名前を取得または設定します。 |
| type | 例外のタイプを取得または設定します。 |
| period | 例外の繰り返し期間を取得または設定します。 |
| days_of_week | このオブジェクトの DayTypeCollection を取得します。<br/>            例外が有効な曜日です。 |
| month_item | 例外の繰り返しがスケジュールされている月の項目を取得または設定します。 |
| month_position | 月内の月項目の位置を取得または設定します。 |
| 月 | 例外の繰り返しがスケジュールされている月を取得または設定します。 |
| month_day | 例外の繰り返しがスケジュールされている月の日を取得または設定します。 |
| day_working | 指定された日付または日タイプが作業日かどうかを示す値を取得または設定します。 |
| working_times | WorkingTimeCollection オブジェクトを取得または設定します。<br/>            平日に作業した時間を定義する作業時間のコレクションです。 |
| parent_calendar | このオブジェクトの親カレンダーを取得します。 |
## メソッド
| 名前 | 説明 |
| :- | :- |
| delete() | 親カレンダーの CalendarExceptionCollection オブジェクトから Exception インスタンスを削除します。 |
| check_exception(dt) | 指定された datetime 構造体のインスタンスが例外日である場合に true を返します。 |
| get_working_time() | カレンダー例外の作業時間を返します。 |
| get_exception_dates() | カレンダー例外が適用される日付を返します。 |

### 関連項目

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

