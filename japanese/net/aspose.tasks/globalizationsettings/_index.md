---
title: "クラス GlobalizationSettings"
second_title: "Aspose.Tasks for .NET API リファレンス"
description: "Aspose.Tasks.GlobalizationSettings クラス。プロジェクトのグローバリゼーション設定を表します"
type: docs
weight: 720
url: /ja/net/aspose.tasks/globalizationsettings/
---
## GlobalizationSettings class

プロジェクトのグローバリゼーション設定を表します。

```csharp
public class GlobalizationSettings
```

## コンストラクタ

| 名前 | 説明 |
| --- | --- |
| [GlobalizationSettings](globalizationsettings/)() | デフォルトコンストラクタです。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| virtual [FalseLiteral](../../aspose.tasks/globalizationsettings/falseliteral/) { get; } | 式で使用されるブール値 'false' リテラルの文字列を取得します。 |
| virtual [FormulaDateNA](../../aspose.tasks/globalizationsettings/formuladatena/) { get; } | 日付フィールドの式で使用される "NA"（空の値）リテラルを取得します。 |
| virtual [TrueLiteral](../../aspose.tasks/globalizationsettings/trueliteral/) { get; } | 式で使用されるブール値 'true' リテラルの文字列を取得します。 |

## 備考

推奨される方法は、プロジェクト全体で文化に依存しないリテラルまたはフォーマットを使用することです。ただし、プロジェクトが文化固有のリテラルを使用している場合、このクラスを使用して式計算エンジンがそれらのリテラルを解析できるように支援できます。

## 例

プロジェクトの言語固有設定の設定方法を示します。

```csharp
var project = new Project();

var attribute = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Number1, "Number");
attribute.Formula = "IIf(ProjDateValue('n.a.')=[Date1];100;200)";

project.ExtendedAttributes.Add(attribute);

var task = project.RootTask.Children.Add("Task");

// 拡張属性を作成する
var extendedAttribute = attribute.CreateExtendedAttribute();
task.ExtendedAttributes.Add(extendedAttribute);

var attributeDate = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Date1, "Date");

task.ExtendedAttributes.Add(attributeDate.CreateExtendedAttribute(DateTime.MinValue));

Console.WriteLine(extendedAttribute.NumericValue);

project.GlobalizationSettings = new MyGlobalizationSettings();

Console.WriteLine(extendedAttribute.NumericValue);
```

### 関連項目

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


