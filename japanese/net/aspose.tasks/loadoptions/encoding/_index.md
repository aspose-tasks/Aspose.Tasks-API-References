---
title: "LoadOptions.Encoding"
second_title: "Aspose.Tasks for .NET API リファレンス"
description: "LoadOptions プロパティ。HTML、MPX、XER、Primavera XML 形式からプロジェクトを読み込む際に使用されるエンコーディングを取得または設定します。デフォルトのエンコーディングは UTF8 です。"
type: docs
weight: 30
url: /ja/net/aspose.tasks/loadoptions/encoding/
---
## LoadOptions.Encoding property

HTML、MPX、XER、Primavera XML 形式からプロジェクトを読み込む際に使用されるエンコーディングを取得または設定します。デフォルトのエンコーディングは UTF8 です。

```csharp
public Encoding Encoding { get; set; }
```

## 例

Primavera XER ファイルからプロジェクトを開く際にエンコーディングを指定する方法を示します。

```csharp
LoadOptions lo = new LoadOptions();
lo.Encoding = Encoding.GetEncoding(1251);
lo.PrimaveraReadOptions = new PrimaveraReadOptions();
var project = new Project("encoding1251.xer", lo);
```

### 関連項目

* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


