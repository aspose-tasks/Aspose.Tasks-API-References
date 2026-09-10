---
title: "ExtendedAttributeDefinition"
second_title: "Aspose.Tasks for Python via .NET API リファレンス"
description: 
type: docs
weight: 310
url: /ja/python-net/aspose.tasks/extendedattributedefinition/
---

## ExtendedAttributeDefinition class

プロジェクトに関連付けられた拡張属性定義を表します。

ExtendedAttributeDefinition 型は次のメンバーを公開します：
## プロパティ
| 名前 | 説明 |
| :- | :- |
| field_id | 取得または設定は、カスタム フィールドのプロジェクト ID に対応します。<br/>            [ExtendedAttributeTask](/tasks/python-net/aspose.tasks/extendedattributetask/) クラスの定数の文字列表現を使用して、[field_id](/tasks/python-net/aspose.tasks/extendedattributedefinition/) プロパティを指定します。 |
| field_name | カスタム フィールドの名前を取得します。 |
| cf_type | カスタム フィールドのタイプを取得します。 |
| guid | カスタム フィールドの Guid を取得または設定します。 |
| element_type | 取得または設定は、拡張属性がタスク、リソース、または割り当てに関連付けられるかどうかを示します。<br/>            タスク、リソース、または割り当てと関連付けられます。 |
| max_multi_values | ピックリストで設定できる最大の値の数を取得または設定します。 |
| user_def | カスタム フィールドがユーザー定義かどうかを示す値を取得または設定します。 |
| alias | カスタム フィールドのエイリアスを取得または設定します。 |
| secondary_pid | カスタム フィールドのセカンダリ PID を取得または設定します。 |
| auto_roll_down | 割り当てへの自動ロールダウンが有効かどうかを示す値を取得または設定します。 |
| default_guid | デフォルトのルックアップ テーブル エントリの Guid を取得または設定します。 |
| lookup_uid | カスタム フィールドに関連付けられたルックアップ テーブルの Guid を取得します。 |
| phonetics_alias | カスタム フィールドのエイリアスの音声表記を取得または設定します。 |
| rollup_type | ロールアップの計算方法を取得または設定します。 |
| calculation_type | カスタム属性の値の計算タイプを取得または設定します。 |
| summary_rows_calculation_type | サマリ行のカスタム属性の値の計算タイプを取得または設定します。 |
| formula | Microsoft Project がカスタム タスク フィールドを埋めるために使用する数式を取得または設定します。 |
| graphical_indicator | 拡張属性に関連付けられたグラフィカルインジケータ情報を取得または設定します。<br/>            MPP形式に適用されます。 |
| restrict_values | カスタムフィールドの値が[value_list](/tasks/python-net/aspose.tasks/extendedattributedefinition/) の値に制限されているかどうかを示す値を取得または設定します。 |
| valuelist_sort_order | 値リストのソート方法を取得または設定します。値は: 0=降順, 1=昇順です。 |
| append_new_values | プロジェクトに追加された新しい値が自動的にリストに追加されるかどうかを示す値を取得または設定します。 |
| default | リスト内のデフォルト値を取得または設定します。 |
| value_list | List<Value> ValueList を取得します。 |
| secondary_guid | 拡張属性のセカンダリ GUID を取得または設定します。 |
| parent_project | [ExtendedAttributeDefinition](/tasks/python-net/aspose.tasks/extendedattributedefinition/) インスタンスの親プロジェクトを取得します。 |
## メソッド
| 名前 | 説明 |
| :- | :- |
| create_extended_attribute() | このオブジェクトのフィールドID値と等しいフィールドIDを持つ新しい拡張属性を作成します。 |
| create_extended_attribute(text_value) | このオブジェクトのフィールドID値と等しいフィールドIDを持ち、指定されたテキスト値を持つ新しい拡張属性を作成します。 |
| create_extended_attribute(numeric_value) | このオブジェクトのフィールドID値と等しいフィールドIDを持ち、指定された数値を持つ新しい拡張属性を作成します。 |
| create_extended_attribute(date_time_value) | このオブジェクトのフィールドID値と等しいフィールドIDを持ち、指定された日付値を持つ新しい拡張属性を作成します。 |
| create_extended_attribute(duration_value) | このオブジェクトのフィールドID値と等しいフィールドIDを持ち、指定された期間値を持つ新しい拡張属性を作成します。 |
| create_extended_attribute(flag_value) | このオブジェクトのフィールドID値と等しいフィールドIDを持ち、指定されたフラグ値を持つ新しい拡張属性を作成します。 |
| create_extended_attribute(lookup_value) | 指定された [Value](/tasks/python-net/aspose.tasks/value/) アイテムにリンクされた新しい拡張属性を作成します。 |
| create_task_definition(custom_field_type, field_id, alias) | Microsoft Project が「None」と表示するシンプルな拡張属性定義を作成するファクトリ メソッドです。<br/>            それは [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) が [NONE](/tasks/python-net/aspose.tasks/calculationtype/) に等しく、タスクでのみ使用できます。<br/>            指定が必要です。 |
| create_task_definition(field_id, alias) | Microsoft Project が「None」と表示するシンプルな拡張属性定義を作成するファクトリ メソッドです。<br/>            それは [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) が [NONE](/tasks/python-net/aspose.tasks/calculationtype/) に等しく、タスクでのみ使用できます。<br/>            指定が必要です。 |
| create_resource_definition(custom_field_type, field_id, alias) | Microsoft Project が「None」と表示するシンプルな拡張属性定義を作成するファクトリ メソッドです。<br/>            それは [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) が [NONE](/tasks/python-net/aspose.tasks/calculationtype/) に等しく、リソースでのみ使用できます。<br/>            指定が必要です。 |
| create_resource_definition(field_id, alias) | Microsoft Project が「None」と表示するシンプルな拡張属性定義を作成するファクトリ メソッドです。<br/>            それは [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) が [NONE](/tasks/python-net/aspose.tasks/calculationtype/) に等しく、リソースでのみ使用できます。<br/>            指定が必要です。 |
| create_lookup_task_definition(field_id, alias) | ルックアップ付きの拡張属性定義を作成するファクトリ メソッドです。<br/>            それは [calculation_type](/tasks/python-net/aspose.tasks/extendedattributeddefinition/) が [LOOKUP](/tasks/python-net/aspose.tasks/calculationtype/) に等しく、タスクでのみ使用できます。<br/>            指定が必要です。 |
| create_lookup_task_definition(custom_field_type, field_id, alias) | ルックアップ付きの拡張属性定義を作成するファクトリ メソッドです。<br/>            それは [calculation_type](/tasks/python-net/aspose.tasks/extendedattributeddefinition/) が [LOOKUP](/tasks/python-net/aspose.tasks/calculationtype/) に等しく、タスクでのみ使用できます。<br/>            指定が必要です。 |
| create_lookup_resource_definition(field_id, alias) | ルックアップ付きの拡張属性定義を作成するファクトリ メソッドです。<br/>            それは [calculation_type](/tasks/python-net/aspose.tasks/extendedattributeddefinition/) が [LOOKUP](/tasks/python-net/aspose.tasks/calculationtype/) に等しく、リソースでのみ使用できます。<br/>            指定が必要です。 |
| create_lookup_resource_definition(custom_field_type, field_id, alias) | ルックアップ付きの拡張属性定義を作成するファクトリ メソッドです。<br/>            それは [calculation_type](/tasks/python-net/aspose.tasks/extendedattributeddefinition/) が [LOOKUP](/tasks/python-net/aspose.tasks/calculationtype/) に等しく、リソースでのみ使用できます。<br/>            指定が必要です。 |
| add_lookup_value(value) | 内部ルックアップリストに値を追加します。これは [value_list](/tasks/python-net/aspose.tasks/extendedattributedefinition/) の操作に推奨される方法です。 |
| remove_lookup_value(value) | 内部ルックアップリストから値を削除します。これは [value_list](/tasks/python-net/aspose.tasks/extendedattributedefinition/) の操作に推奨される方法です。 |

### 関連項目

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

