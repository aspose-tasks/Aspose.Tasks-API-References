---
title: "Project.GlobalizationSettings"
second_title: "Aspose.Tasks for .NET API リファレンス"
description: "Project プロパティ。プロジェクトのグローバリゼーション（言語固有）設定を取得または設定します。"
type: docs
weight: 460
url: /ja/net/aspose.tasks/project/globalizationsettings/
---
## Project.GlobalizationSettings property

プロジェクトのグローバリゼーション（言語固有）設定を取得または設定します。

```csharp
public GlobalizationSettings GlobalizationSettings { get; set; }
```

## 備考

推奨される方法は、プロジェクト全体でカルチャに依存しないリテラルやフォーマットを使用することです。ただし、プロジェクトがカルチャ固有のリテラルを使用する場合、このクラスを使用して計算エンジンがそれらのリテラルを解析できるように支援できます。

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

* class [GlobalizationSettings](../../globalizationsettings/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


