---
title: "Duration"
second_title: "Aspose.Tasks for Python via .NET API リファレンス"
description: 
type: docs
weight: 260
url: /ja/python-net/aspose.tasks/duration/
---

## Duration class

プロジェクト内の期間を表します。

Duration 型は次のメンバーを公開します:
## コンストラクタ
| 名前 | 説明 |
| :- | :- |
| Duration() | Duration クラスの新しいインスタンスを初期化します |
## プロパティ
| 名前 | 説明 |
| :- | :- |
| time_span | この Duration オブジェクトの [time_span](/tasks/python-net/aspose.tasks/duration/) インスタンスを取得します。 |
| time_unit | このオブジェクトの時間単位タイプを取得します。 |
| is_estimated | 時間単位が推定かどうかを示す値を取得します。 |
| is_elapsed | 時間単位が経過かどうかを示す値を取得します。 |
## メソッド
| 名前 | 説明 |
| :- | :- |
| add(d) | 指定された期間をこの期間に加算します。 |
| add(val) | 指定された double 値をこの期間に加算します。 |
| subtract(d) | 指定された期間をこの期間インスタンスから減算します。 |
| subtract(val) | 指定された double 値をこの期間インスタンスから減算します。 |
| parse(p, value) | 指定された文字列を [Duration](/tasks/python-net/aspose.tasks/duration/) 構造体のインスタンスに変換します。 |
| parse_time_span(value) | フォーマット "PT--H--M--S--" の期間文字列を解析します。 |
| to_double() | Duration オブジェクトを float 値に変換します。 |
| convert(time_unit_type) | Duration オブジェクトを、指定された時間単位を持つ別の期間に変換します。 |
| equals(other) | このインスタンスが指定されたオブジェクトと等しいかどうかを示す値を返します。 |

### 関連項目

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

