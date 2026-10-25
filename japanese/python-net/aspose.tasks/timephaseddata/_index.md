---
title: "TimephasedData"
second_title: "Aspose.Tasks for Python via .NET API リファレンス"
description: 
type: docs
weight: 1270
url: /ja/python-net/aspose.tasks/timephaseddata/
---

## TimephasedData class

時間フェーズデータを表します。

TimephasedData 型は次のメンバーを公開します：
## コンストラクタ
| 名前 | 説明 |
| :- | :- |
| TimephasedData() | [TimephasedData](/tasks/python-net/aspose.tasks/timephaseddata/) クラスの新しいインスタンスを初期化します。 |
## プロパティ
| 名前 | 説明 |
| :- | :- |
| value_to_units | 単位ベースの時間相関データに対するこのオブジェクトの文字列値を表す float インスタンスを取得します。 |
| uid | 時間相関データの一意識別子を取得または設定します |
| start | 時間相関データ期間の開始日を取得または設定します。 |
| finish | 時間相関データ期間の終了日を取得または設定します。 |
| unit | 時間相関データ期間の時間単位を取得または設定します。 |
| timephased_data_type | 時間相関データのタイプを取得または設定します。 |
| value | 時間分割データ期間の単位時間あたりの値を取得または設定します。 |
| value_to_duration | このオブジェクトの文字列値を表す datatime インスタンスを取得します。 |
| value_to_cost | このオブジェクトの文字列値を表す float インスタンスを取得します。 |
## メソッド
| 名前 | 説明 |
| :- | :- |
| create_cost_timephased(uid, start, finish, value, time_unit, type) |  |
| create_cost_timephased(uid, start, finish, value, type) |  |
| create_work_timephased(uid, start, finish, value, time_unit, type) | 作業ベースの時間分割データ用に、[TimephasedData](/tasks/python-net/aspose.tasks/timephaseddata/) クラスの新しいインスタンスを作成し、初期化します。 |
| create_unit_timephased(uid, start, finish, units, type) | 素材リソースの割り当ての単位ベース時間分割データ用に、[TimephasedData](/tasks/python-net/aspose.tasks/timephaseddata/) クラスの新しいインスタンスを作成し、初期化します。 |

### 関連項目

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

