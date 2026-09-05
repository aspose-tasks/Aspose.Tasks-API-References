---
title: "GlobalizationSettings"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "プロジェクトのグローバリゼーション設定を表します。"
type: docs
weight: 114
url: /ja/java/com.aspose.tasks/globalizationsettings/
---

**Inheritance:**
java.lang.Object
```
public class GlobalizationSettings
```

プロジェクトのグローバリゼーション設定を表します。

推奨される方法は、プロジェクト全体でカルチャに依存しないリテラルまたはフォーマットを使用することです。ただし、プロジェクトがカルチャ固有のリテラルを使用する場合、このクラスを使用して数式計算エンジンがそれらのリテラルを解析できるようにすることができます。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [GlobalizationSettings()](#GlobalizationSettings--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getFalseLiteral()](#getFalseLiteral--) | 数式で使用されるブール値 'false' リテラルの文字列を取得します。 |
| [getFormulaDateNA()](#getFormulaDateNA--) | 日付フィールドの数式で使用される "NA"（空の値）リテラルを取得します。 |
| [getTrueLiteral()](#getTrueLiteral--) | 数式で使用されるブール値 'true' リテラルの文字列を取得します。 |
### GlobalizationSettings() {#GlobalizationSettings--}
```
public GlobalizationSettings()
```


### getFalseLiteral() {#getFalseLiteral--}
```
public String getFalseLiteral()
```


数式で使用されるブール値 'false' リテラルの文字列を取得します。

**Returns:**
java.lang.String - 式で使用されるブール値 'false' リテラルの文字列です。
### getFormulaDateNA() {#getFormulaDateNA--}
```
public String getFormulaDateNA()
```


日付フィールドの数式で使用される "NA"（空の値）リテラルを取得します。

**Returns:**
java.lang.String - 日付フィールドの式で使用される "NA"（空の値）リテラルです。
### getTrueLiteral() {#getTrueLiteral--}
```
public String getTrueLiteral()
```


数式で使用されるブール値 'true' リテラルの文字列を取得します。

**Returns:**
java.lang.String - 式で使用されるブール値 'true' リテラルの文字列です。
