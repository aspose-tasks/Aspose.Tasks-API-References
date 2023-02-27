---
title: ExtendedAttributeDefinition
second_title: Aspose.Tasks for .NET API リファレンス
description: プロジェクトに関連付けられた拡張属性定義を表します
type: docs
weight: 540
url: /ja/net/aspose.tasks/extendedattributedefinition/
---
## ExtendedAttributeDefinition class

プロジェクトに関連付けられた拡張属性定義を表します。

```csharp
public class ExtendedAttributeDefinition
```

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [Alias](../../aspose.tasks/extendedattributedefinition/alias/) { get; set; } | カスタム フィールドのエイリアスを取得または設定します。 |
| [AppendNewValues](../../aspose.tasks/extendedattributedefinition/appendnewvalues/) { get; set; } | プロジェクトに追加された新しい値が自動的にリストに追加されるかどうかを示す値を取得または設定します。 |
| [AutoRollDown](../../aspose.tasks/extendedattributedefinition/autorolldown/) { get; set; } | 割り当てへの自動ロールダウンが有効かどうかを示す値を取得または設定します。 |
| [CalculationType](../../aspose.tasks/extendedattributedefinition/calculationtype/) { get; set; } | カスタム属性の値の計算のタイプを取得または設定します。 |
| [CfType](../../aspose.tasks/extendedattributedefinition/cftype/) { get; } | カスタム フィールドのタイプを取得します。 |
| [Default](../../aspose.tasks/extendedattributedefinition/default/) { get; set; } | リストのデフォルト値を取得または設定します。 |
| [DefaultGuid](../../aspose.tasks/extendedattributedefinition/defaultguid/) { get; set; } | 既定のルックアップ テーブル エントリの Guid を取得または設定します。 |
| [ElementType](../../aspose.tasks/extendedattributedefinition/elementtype/) { get; set; } | 拡張属性を取得または設定します がタスク、リソース、または割り当てに関連付けられています. |
| [FieldId](../../aspose.tasks/extendedattributedefinition/fieldid/) { get; set; } | カスタム フィールドのプロジェクト ID に対応する取得または設定を行います。 から定数の文字列表現を使用します。[`ExtendedAttributeTask`](../extendedattributetask/)指定するクラス[`FieldId`](./fieldid/)プロパティ. |
| [FieldName](../../aspose.tasks/extendedattributedefinition/fieldname/) { get; } | カスタム フィールドの名前を取得します。 |
| [Formula](../../aspose.tasks/extendedattributedefinition/formula/) { get; set; } | Microsoft Project がカスタム タスク フィールドに入力するために使用する数式を取得または設定します。 |
| [Guid](../../aspose.tasks/extendedattributedefinition/guid/) { get; set; } | カスタム フィールドの Guid を取得または設定します。 |
| [LookupUid](../../aspose.tasks/extendedattributedefinition/lookupuid/) { get; } | カスタム フィールドに関連付けられたルックアップ テーブルの Guid を取得します。 |
| [MaxMultiValues](../../aspose.tasks/extendedattributedefinition/maxmultivalues/) { get; set; } | 選択リストに設定できる値の最大数を取得または設定します。 |
| [ParentProject](../../aspose.tasks/extendedattributedefinition/parentproject/) { get; } | の親プロジェクトを取得します`ExtendedAttributeDefinition`インスタンス. |
| [PhoneticsAlias](../../aspose.tasks/extendedattributedefinition/phoneticsalias/) { get; set; } | カスタム フィールドのエイリアスの発音を取得または設定します。 |
| [RestrictValues](../../aspose.tasks/extendedattributedefinition/restrictvalues/) { get; set; } | カスタム フィールドの値が[`ValueList`](./valuelist/). |
| [RollupType](../../aspose.tasks/extendedattributedefinition/rolluptype/) { get; set; } | ロールアップの計算方法を取得または設定します。 |
| [SecondaryGuid](../../aspose.tasks/extendedattributedefinition/secondaryguid/) { get; set; } | 拡張属性のセカンダリ GUID を取得または設定します。 |
| [SecondaryPid](../../aspose.tasks/extendedattributedefinition/secondarypid/) { get; set; } | カスタム フィールドのセカンダリ PID を取得または設定します。 |
| [SummaryRowsCalculationType](../../aspose.tasks/extendedattributedefinition/summaryrowscalculationtype/) { get; set; } | 集計行のカスタム属性の値の計算のタイプを取得または設定します。 |
| [UserDef](../../aspose.tasks/extendedattributedefinition/userdef/) { get; set; } | カスタム フィールドがユーザー定義かどうかを示す値を取得または設定します。 |
| [ValueList](../../aspose.tasks/extendedattributedefinition/valuelist/) { get; } | List&lt;Value&gt; ValueList を取得します。 |
| [ValuelistSortOrder](../../aspose.tasks/extendedattributedefinition/valuelistsortorder/) { get; set; } | 値リストの並べ替え方法を取得または設定します。値は次のとおりです: 0=降順、1=昇順. |

## メソッド

| 名前 | 説明 |
| --- | --- |
| static [CreateLookupResourceDefinition](../../aspose.tasks/extendedattributedefinition/createlookupresourcedefinition/#createlookupresourcedefinition_1)(ExtendedAttributeResource, string) | ルックアップで拡張属性定義を作成するファクトリーメソッド. を持っています[`CalculationType`](./calculationtype/)に等しいLookupリソースのみで使用できます。 指定する必要があります*fieldId*と*alias*このメソッドを呼び出すとき. フィールド型はフィールド ID から推測されます. |
| static [CreateLookupResourceDefinition](../../aspose.tasks/extendedattributedefinition/createlookupresourcedefinition/#createlookupresourcedefinition)(CustomFieldType, ExtendedAttributeResource, string) | ルックアップで拡張属性定義を作成するファクトリーメソッド. を持っています[`CalculationType`](./calculationtype/)に等しいLookupリソースのみで使用できます。 指定する必要があります*customFieldType*、*fieldId*と*alias*このメソッドを呼び出すと. |
| static [CreateLookupTaskDefinition](../../aspose.tasks/extendedattributedefinition/createlookuptaskdefinition/#createlookuptaskdefinition_1)(ExtendedAttributeTask, string) | ルックアップで拡張属性定義を作成するファクトリーメソッド. を持っています[`CalculationType`](./calculationtype/)に等しいLookupタスクでのみ使用できます。 指定する必要があります*fieldId*と*alias*このメソッドを呼び出すとき. フィールド型はフィールド ID から推測されます. |
| static [CreateLookupTaskDefinition](../../aspose.tasks/extendedattributedefinition/createlookuptaskdefinition/#createlookuptaskdefinition)(CustomFieldType, ExtendedAttributeTask, string) | ルックアップで拡張属性定義を作成するファクトリーメソッド. を持っています[`CalculationType`](./calculationtype/)に等しいLookupタスクでのみ使用できます。 指定する必要があります*customFieldType*、*fieldId*と*alias*このメソッドを呼び出すと. |
| static [CreateResourceDefinition](../../aspose.tasks/extendedattributedefinition/createresourcedefinition/#createresourcedefinition_1)(ExtendedAttributeResource, string) | Microsoft Project では「なし」と表示される単純な拡張属性定義を作成するファクトリ メソッド。 [`CalculationType`](./calculationtype/)に等しいNoneリソースのみで使用できます。 指定する必要があります*fieldId*と*alias*このメソッドを呼び出すとき. フィールド型はフィールド ID から推測されます. |
| static [CreateResourceDefinition](../../aspose.tasks/extendedattributedefinition/createresourcedefinition/#createresourcedefinition)(CustomFieldType, ExtendedAttributeResource, string) | Microsoft Project では「なし」と表示される単純な拡張属性定義を作成するファクトリ メソッド。 [`CalculationType`](./calculationtype/)に等しいNoneリソースのみで使用できます。 指定する必要があります*customFieldType*、*fieldId*と*alias*このメソッドを呼び出すと. |
| static [CreateTaskDefinition](../../aspose.tasks/extendedattributedefinition/createtaskdefinition/#createtaskdefinition_1)(ExtendedAttributeTask, string) | Microsoft Project では「なし」と表示される単純な拡張属性定義を作成するファクトリ メソッド。 [`CalculationType`](./calculationtype/)に等しいNoneタスクでのみ使用できます。 指定する必要があります*fieldId*と*alias*このメソッドを呼び出すとき. フィールド型はフィールド ID から推測されます. |
| static [CreateTaskDefinition](../../aspose.tasks/extendedattributedefinition/createtaskdefinition/#createtaskdefinition)(CustomFieldType, ExtendedAttributeTask, string) | Microsoft Project では「なし」と表示される単純な拡張属性定義を作成するファクトリ メソッド。 [`CalculationType`](./calculationtype/)に等しいNoneタスクでのみ使用できます。 指定する必要があります*customFieldType*、*fieldId*と*alias*このメソッドを呼び出すとき. |
| [AddLookupValue](../../aspose.tasks/extendedattributedefinition/addlookupvalue/)(Value) | 内部参照リストに値を追加します。これは、[`ValueList`](./valuelist/). |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute)() | このオブジェクトのフィールド ID 値に等しいフィールド ID を持つ新しい拡張属性を作成します。 |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_3)(bool) | このオブジェクトのフィールド ID 値と指定されたフラグ値に等しいフィールド ID を持つ新しい拡張属性を作成します。 |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_4)(DateTime) | このオブジェクトのフィールド ID 値と指定された日付値に等しいフィールド ID を持つ新しい拡張属性を作成します。 |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_5)(decimal) | このオブジェクトのフィールド ID 値と指定された数値に等しいフィールド ID を持つ新しい拡張属性を作成します。 |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_1)(Duration) | このオブジェクトのフィールド ID 値と指定された期間値に等しいフィールド ID を持つ新しい拡張属性を作成します。 |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_6)(string) | このオブジェクトのフィールド ID 値と指定されたテキスト値に等しいフィールド ID を持つ新しい拡張属性を作成します。 |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_2)(Value) | 指定した属性にリンクされた新しい拡張属性を作成します[`Value`](../value/)item. |
| override [Equals](../../aspose.tasks/extendedattributedefinition/equals/)(object) | このインスタンスが指定されたオブジェクトと等しいかどうかを示すフラグを返します。 |
| override [GetHashCode](../../aspose.tasks/extendedattributedefinition/gethashcode/)() | のインスタンスのハッシュ コードを返します。`ExtendedAttributeDefinition`class. |
| [RemoveLookupValue](../../aspose.tasks/extendedattributedefinition/removelookupvalue/)(Value) | 内部参照リストから値を削除します。これは、[`ValueList`](./valuelist/). |

### 関連項目

* 名前空間 [Aspose.Tasks](../../aspose.tasks/)
* 組み立て [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
