---
title: "Aspose::Tasks::ExtendedAttributeDefinition クラス"
linktitle: "ExtendedAttributeDefinition"
articleTitle: "ExtendedAttributeDefinition"
second_title: "Aspose.Tasks for C++"
description: "プロジェクトに関連付けられた拡張属性定義を表します。"
type: docs
weight: 10
url: /ja/cpp/aspose.tasks/extendedattributedefinition/
---

## ExtendedAttributeDefinition class

プロジェクトに関連付けられた拡張属性定義を表します。

## メソッド

| 名前 | 説明 |
| --- | --- |
| [AddLookupValue](./addlookupvalue/) | 内部ルックアップリストに値を追加します。これは ValueList の操作に推奨される方法です。 |
| [CreateExtendedAttribute (7 overloads)](./createextendedattribute/) | このオブジェクトのフィールド ID の値と等しいフィールド ID を持つ新しい拡張属性を作成します。 |
| [CreateLookupResourceDefinition (2 overloads)](./createlookupresourcedefinition/) | ルックアップ付きの拡張属性定義を作成するファクトリーメソッドです。CalculationType は Tasks::CalculationType::Lookup に等しく、Resources でのみ使用できます。このメソッドを呼び出す際には customFieldType、fieldId、alias を指定する必要があります。 |
| [CreateLookupTaskDefinition (2 overloads)](./createlookuptaskdefinition/) | ルックアップ付きの拡張属性定義を作成するファクトリーメソッドです。CalculationType は Tasks::CalculationType::Lookup に等しく、Tasks でのみ使用できます。このメソッドを呼び出す際には customFieldType、fieldId、alias を指定する必要があります。 |
| [CreateResourceDefinition (2 overloads)](./createresourcedefinition/) | Microsoft Project が \"None\" と表示するシンプルな拡張属性定義を作成するファクトリーメソッドです。CalculationType は Tasks::CalculationType::None に等しく、Resource でのみ使用できます。このメソッドを呼び出す際には customFieldType、fieldId、alias を指定する必要があります。 |
| [CreateTaskDefinition (2 overloads)](./createtaskdefinition/) | Microsoft Project が \"None\" と表示するシンプルな拡張属性定義を作成するファクトリーメソッドです。CalculationType は Tasks::CalculationType::None に等しく、Tasks でのみ使用できます。このメソッドを呼び出す際には customFieldType、fieldId、alias を指定する必要があります。 |
| [Equals](./equals/) | このインスタンスが指定されたオブジェクトと等しいかどうかを示すフラグを返します。 |
| [get_Alias](./get_alias/) | カスタム フィールドのエイリアスを取得します。 |
| [get_AppendNewValues](./get_appendnewvalues/) | プロジェクトに追加された新しい値が自動的にリストに追加されるかどうかを示す値を取得します。 |
| [get_AutoRollDown](./get_autorolldown/) | 割り当てへの自動ロールダウンが有効かどうかを示す値を取得します。 |
| [get_CalculationType](./get_calculationtype/) | カスタム属性の値の計算タイプを取得します。 |
| [get_CfType](./get_cftype/) | カスタム フィールドのタイプを取得します。 |
| [get_Default](./get_default/) | リスト内のデフォルト値を取得します。 |
| [get_DefaultGuid](./get_defaultguid/) | デフォルト ルックアップ テーブル エントリの Guid を取得します。 |
| [get_ElementType](./get_elementtype/) | 拡張属性がタスク、リソース、または割り当てに関連付けられているかどうかを取得します。 |
| [get_FieldId](./get_fieldid/) | カスタム フィールドのプロジェクト ID に対応します。FieldId プロパティを指定するには、Aspose::Tasks::ExtendedAttributeTask クラスの定数の文字列表現を使用します。 |
| [get_FieldName](./get_fieldname/) | カスタム フィールドの名前を取得します。 |
| [get_Formula](./get_formula/) | Microsoft Project がカスタム タスク フィールドを入力するために使用する数式を取得します。 |
| [get_GraphicalIndicator](./get_graphicalindicator/) | 拡張属性に関連付けられたグラフィカル インジケータ情報を取得します。MPP 形式に適用されます。 |
| [get_Guid](./get_guid/) | カスタム フィールドの Guid を取得します。 |
| [get_LookupUid](./get_lookupuid/) | カスタム フィールドに関連付けられたルックアップ テーブルの Guid を取得します。 |
| [get_MaxMultiValues](./get_maxmultivalues/) | ピックリストに設定できる最大値の数を取得します。 |
| [get_ParentProject](./get_parentproject/) | ExtendedAttributeDefinition インスタンスの親プロジェクトを取得します。 |
| [get_PhoneticsAlias](./get_phoneticsalias/) | カスタム フィールドのエイリアスの音声表記を取得します。 |
| [get_RestrictValues](./get_restrictvalues/) | カスタム フィールドの値が ValueList の値に制限されているかどうかを示す値を取得します。 |
| [get_RollupType](./get_rolluptype/) | ロールアップの計算方法を取得します。 |
| [get_SecondaryGuid](./get_secondaryguid/) | 拡張属性のセカンダリ GUID を取得します。 |
| [get_SecondaryPid](./get_secondarypid/) | カスタム フィールドのセカンダリ PID を取得します。 |
| [get_SummaryRowsCalculationType](./get_summaryrowscalculationtype/) | サマリ行のカスタム属性値の計算タイプを取得します。 |
| [get_UserDef](./get_userdef/) | カスタム フィールドがユーザー定義かどうかを示す値を取得します。 |
| [get_ValueList](./get_valuelist/) | List< Value > ValueList を取得します。 |
| [get_ValuelistSortOrder](./get_valuelistsortorder/) | 値リストのソート方法を取得します。値は: 0=降順、1=昇順です。 |
| [GetHashCode](./gethashcode/) | ExtendedAttributeDefinition クラスのインスタンスのハッシュコードを返します。 |
| [RemoveLookupValue](./removelookupvalue/) | 内部ルックアップリストから値を削除します。これは ValueList の操作に推奨される方法です。 |
| [set_Alias](./set_alias/) | カスタム フィールドのエイリアスを設定します。 |
| [set_AppendNewValues](./set_appendnewvalues/) | プロジェクトに追加された新しい値が自動的にリストに追加されるかどうかを示す値を設定します。 |
| [set_AutoRollDown](./set_autorolldown/) | 割り当てへの自動ロールダウンが有効かどうかを示す値を設定します。 |
| [set_CalculationType](./set_calculationtype/) | カスタム属性の値の計算タイプを設定します。 |
| [set_Default](./set_default/) | リストのデフォルト値を設定します。 |
| [set_DefaultGuid](./set_defaultguid/) | デフォルト ルックアップテーブル エントリの Guid を設定します。 |
| [set_ElementType](./set_elementtype/) | 拡張属性がタスク、リソース、または割り当てに関連付けられるかどうかを設定します。 |
| [set_FieldId](./set_fieldid/) | カスタム フィールドのプロジェクト ID に対応します。FieldId プロパティを指定するには、Aspose::Tasks::ExtendedAttributeTask クラスの定数の文字列表現を使用します。 |
| [set_Formula](./set_formula/) | Microsoft Project がカスタム タスク フィールドを入力する際に使用する数式を設定します。 |
| [set_GraphicalIndicator](./set_graphicalindicator/) | 拡張属性に関連付けられたグラフィカル インジケータ情報を設定します。MPP 形式に適用可能です。 |
| [set_Guid](./set_guid/) | カスタム フィールドの Guid を設定します。 |
| [set_MaxMultiValues](./set_maxmultivalues/) | ピックリストに設定できる最大値の数を設定します。 |
| [set_PhoneticsAlias](./set_phoneticsalias/) | カスタム フィールドのエイリアスの音声表記を設定します。 |
| [set_RestrictValues](./set_restrictvalues/) | カスタム フィールドの値が ValueList の値に制限されているかどうかを示す値を設定します。 |
| [set_RollupType](./set_rolluptype/) | ロールアップの計算方法を設定します。 |
| [set_SecondaryGuid](./set_secondaryguid/) | 拡張属性のセカンダリ Guid を設定します。 |
| [set_SecondaryPid](./set_secondarypid/) | カスタム フィールドのセカンダリ PID を設定します。 |
| [set_SummaryRowsCalculationType](./set_summaryrowscalculationtype/) | サマリ行に対するカスタム属性の値の計算タイプを設定します。 |
| [set_UserDef](./set_userdef/) | カスタム フィールドがユーザー定義かどうかを示す値を設定します。 |
| [set_ValuelistSortOrder](./set_valuelistsortorder/) | 値リストのソート方法を設定します。値は: 0=降順、1=昇順です。 |

