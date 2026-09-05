---
title: "PrimaveraProjectInfo"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "Primavera フォーマットから読み込まれたプロジェクトに関する簡単な情報を表します。"
type: docs
weight: 204
url: /ja/java/com.aspose.tasks/primaveraprojectinfo/
---

**Inheritance:**
java.lang.Object
```
public final class PrimaveraProjectInfo
```

Primavera フォーマットから読み込まれたプロジェクトに関する簡単な情報を表します。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getExportFlag()](#getExportFlag--) | プロジェクトのエクスポートフラグを取得します。 |
| [getName()](#getName--) | プロジェクトの名前を取得します。 |
| [getShortName()](#getShortName--) | プロジェクトの短縮名（プロジェクト ID）を取得します。 |
| [getUid()](#getUid--) | プロジェクトの UID を取得します。 |
### getExportFlag() {#getExportFlag--}
```
public final boolean getExportFlag()
```


プロジェクトのエクスポートフラグを取得します。Primavera でプロジェクトがエクスポート対象として選択されると、その ExportFlag は true になります。明示的にエクスポート対象として選択されていないプロジェクトでも、エクスポートされたプロジェクトとの関係により XER ファイルにエクスポートされることがあります。

**Returns:**
boolean - プロジェクトのエクスポートフラグ。
### getName() {#getName--}
```
public final String getName()
```


プロジェクトの名前を取得します。

**Returns:**
java.lang.String - プロジェクトの名前。
### getShortName() {#getShortName--}
```
public final String getShortName()
```


プロジェクトの短縮名（プロジェクト ID）を取得します。

**Returns:**
java.lang.String - プロジェクトの短縮名（プロジェクト ID）。
### getUid() {#getUid--}
```
public final int getUid()
```


プロジェクトの UID を取得します。

**Returns:**
int - プロジェクトの UID。
