---
title: "FilterCriteria"
second_title: "Aspose.Tasks for Python via .NET API リファレンス"
description: 
type: docs
weight: 350
url: /ja/python-net/aspose.tasks/filtercriteria/
---

## FilterCriteria class

MSPビューに表示されるために、タスクまたはリソースが満たすべき基準を定義します。

FilterCriteria 型は次のメンバーを公開します:
## コンストラクタ
| 名前 | 説明 |
| :- | :- |
| FilterCriteria() | FilterCriteria クラスの新しいインスタンスを初期化します |
## プロパティ
| 名前 | 説明 |
| :- | :- |
| 操作 | FieldName、Test、Value で設定された基準を取得または設定します。これはフィルター内の他の基準と関連します。 |
| field | 変更するための [field](/tasks/python-net/aspose.tasks/filtercriteria/) を取得または設定します。 |
| test | フィルターの選択基準として機能する、FieldName と Value の間で行われる比較のタイプを取得または設定します。<br/>            [FilterComparisonType](/tasks/python-net/aspose.tasks/filtercomparisontype/) |
| values | FieldName で指定されたフィールドの値と比較するオブジェクト値を取得します。 |
| criteria_rows | 子 [FilterCriteria](/tasks/python-net/aspose.tasks/filtercriteria/) 行のリストを取得します。<br/>            フィルターに複数の基準行が含まれる場合、AND 演算子の効果は、両方の行の基準が満たされたときにタスクまたはリソースがこのフィルターの結果として表示されることです。<br/>            OR 演算子の効果は、いずれか一方の行の基準が満たされることです。 |
## メソッド
| 名前 | 説明 |
| :- | :- |
| is_field_value() | FilterCriteria の右側の値が定数ではなくフィールド参照であるかどうかを取得します。 |
| set_value_field(value) | FieldName で指定されたフィールドの値と比較されるフィールドを設定します。 |

### 関連項目

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

