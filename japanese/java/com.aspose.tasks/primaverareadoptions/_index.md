---
title: "PrimaveraReadOptions"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "Primavera Xml または Primavera Xer ファイルを読み取る際に追加オプションを指定できます。"
type: docs
weight: 206
url: /ja/java/com.aspose.tasks/primaverareadoptions/
---

**Inheritance:**
java.lang.Object
```
public class PrimaveraReadOptions
```

Primavera Xml または Primavera Xer ファイルを読み取る際に追加オプションを指定できます。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [PrimaveraReadOptions()](#PrimaveraReadOptions--) | 新しいインスタンスを初期化します [PrimaveraReadOptions](../../com.aspose/tasks/primaverareadoptions) クラス。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getPreserveUids()](#getPreserveUids--) | エンティティの元の一意識別子を保持するかどうかを指定するフラグを取得します。 |
| [getProjectUid()](#getProjectUid--) | 複数のプロジェクトを含むファイルから読み取るプロジェクトの UID を取得します。 |
| [getReadBaselineProjects()](#getReadBaselineProjects--) | ベースラインプロジェクトをロードするかどうかを指定するフラグを取得します。 |
| [getUndefinedConstraintHandlingBehavior()](#getUndefinedConstraintHandlingBehavior--) | XER 形式から読み取った未定義の制約を持つタスクを処理する際に使用される動作を指定します。 |
| [setPreserveUids(boolean value)](#setPreserveUids-boolean-) | エンティティの元の一意識別子を保持するかどうかを指定するフラグを設定します。 |
| [setProjectUid(int value)](#setProjectUid-int-) | 複数のプロジェクトを含むファイルから読み取るプロジェクトの UID を設定します。 |
| [setReadBaselineProjects(boolean value)](#setReadBaselineProjects-boolean-) | ベースラインプロジェクトをロードするかどうかを指定するフラグを設定します。 |
| [setUndefinedConstraintHandlingBehavior(int value)](#setUndefinedConstraintHandlingBehavior-int-) | XER 形式から読み取った未定義の制約を持つタスクを処理する際に使用される動作を指定します。 |
### PrimaveraReadOptions() {#PrimaveraReadOptions--}
```
public PrimaveraReadOptions()
```


新しいインスタンスを初期化します [PrimaveraReadOptions](../../com.aspose/tasks/primaverareadoptions) クラス。

### getPreserveUids() {#getPreserveUids--}
```
public final boolean getPreserveUids()
```


エンティティの元の一意識別子を保持するかどうかを指定するフラグを取得します。

**Returns:**
boolean - エンティティの元の一意識別子を保持するかどうかを指定するフラグ。
### getProjectUid() {#getProjectUid--}
```
public final int getProjectUid()
```


複数のプロジェクトを含むファイルから読み取るプロジェクトの UID を取得します。

**Returns:**
int - 複数のプロジェクトを含むファイルから読み取るプロジェクトの UID。
### getReadBaselineProjects() {#getReadBaselineProjects--}
```
public final boolean getReadBaselineProjects()
```


ベースラインプロジェクトをロードするかどうかを指定するフラグを取得します。デフォルト値は true です。

--------------------

このフラグはベースラインプロジェクトを含む Primavera XML ファイルに適用されます（ベースラインは XER 形式ではサポートされていません）。ベースラインデータが不要な場合、大規模プロジェクトのロードを高速化するためにオプションを false に設定できます。

**Returns:**
boolean - ベースラインプロジェクトをロードするかどうかを指定するフラグ。
### getUndefinedConstraintHandlingBehavior() {#getUndefinedConstraintHandlingBehavior--}
```
public final int getUndefinedConstraintHandlingBehavior()
```


XER 形式から読み取った未定義の制約を持つタスクを処理する際に使用される動作を指定します。

**Returns:**
int - XER 形式から読み取った未定義の制約を持つタスクを処理する際に使用される動作。
### setPreserveUids(boolean value) {#setPreserveUids-boolean-}
```
public final void setPreserveUids(boolean value)
```


エンティティの元の一意識別子を保持するかどうかを指定するフラグを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | エンティティの元の一意識別子を保持するかどうかを指定するフラグ。 |

### setProjectUid(int value) {#setProjectUid-int-}
```
public final void setProjectUid(int value)
```


複数のプロジェクトを含むファイルから読み取るプロジェクトの UID を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | 複数のプロジェクトを含むファイルから読み取るプロジェクトの UID。 |

### setReadBaselineProjects(boolean value) {#setReadBaselineProjects-boolean-}
```
public final void setReadBaselineProjects(boolean value)
```


ベースラインプロジェクトをロードするかどうかを指定するフラグを設定します。デフォルト値は true です。

--------------------

このフラグはベースラインプロジェクトを含む Primavera XML ファイルに適用されます（ベースラインは XER 形式ではサポートされていません）。ベースラインデータが不要な場合、大規模プロジェクトのロードを高速化するためにオプションを false に設定できます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | ベースラインプロジェクトをロードするかどうかを指定するフラグ。 |

### setUndefinedConstraintHandlingBehavior(int value) {#setUndefinedConstraintHandlingBehavior-int-}
```
public final void setUndefinedConstraintHandlingBehavior(int value)
```


XER 形式から読み取った未定義の制約を持つタスクを処理する際に使用される動作を指定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | XER 形式から読み取った未定義の制約を持つタスクを処理するために使用される動作。 |

