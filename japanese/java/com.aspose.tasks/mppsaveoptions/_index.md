---
title: "MPPSaveOptions"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "プロジェクトデータを MPP に保存する際に追加オプションを指定できます。"
type: docs
weight: 149
url: /ja/java/com.aspose.tasks/mppsaveoptions/
---

**Inheritance:**
java.lang.Object、[com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class MPPSaveOptions extends SimpleSaveOptions
```

プロジェクトデータを MPP に保存する際に追加オプションを指定できます。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [MPPSaveOptions()](#MPPSaveOptions--) | 新しい [MPPSaveOptions](../../com.aspose.tasks/mppsaveoptions) クラスのインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getClearVba()](#getClearVba--) | プロジェクトを MPP 形式で保存する際に既存の VBA マクロ データを削除するかどうかを示す値を取得します。 |
| [getProtectionPassword()](#getProtectionPassword--) | 生成された MPP ファイルを保護するために使用されるパスワードを取得します。 |
| [getRemoveInvalidAssignments()](#getRemoveInvalidAssignments--) | MPP に保存する際に無効なリソース割り当てを削除するかどうかを示す値を取得します。 |
| [getWriteFilters()](#getWriteFilters--) | プロジェクトを MPP 形式で保存する際にフィルタ データを書き込むかどうかを示す値を取得します。 |
| [getWriteGroups()](#getWriteGroups--) | プロジェクトを MPP 形式で保存する際にグループ データを書き込むかどうかを示す値を取得します。 |
| [getWriteVba()](#getWriteVba--) | MPP ファイル内の既存の VBA マクロ データを更新するかどうかを示す値を取得します。 |
| [getWriteViewData()](#getWriteViewData--) | プロジェクトを MPP 形式で保存する際にビュー データを書き込むかどうかを示す値を取得します。 |
| [setClearVba(boolean value)](#setClearVba-boolean-) | プロジェクトを MPP 形式で保存する際に既存の VBA マクロ データを削除するかどうかを示す値を設定します。 |
| [setProtectionPassword(String value)](#setProtectionPassword-java.lang.String-) | 生成された MPP ファイルを保護するために使用されるパスワードを設定します。 |
| [setRemoveInvalidAssignments(boolean value)](#setRemoveInvalidAssignments-boolean-) | MPP に保存する際に無効なリソース割り当てを削除するかどうかを示す値を設定します。 |
| [setWriteFilters(boolean value)](#setWriteFilters-boolean-) | プロジェクトを MPP 形式で保存する際にフィルタ データを書き込むかどうかを示す値を設定します。 |
| [setWriteGroups(boolean value)](#setWriteGroups-boolean-) | プロジェクトを MPP 形式で保存する際にグループ データを書き込むかどうかを示す値を設定します。 |
| [setWriteVba(boolean value)](#setWriteVba-boolean-) | MPP ファイル内の既存の VBA マクロ データを更新するかどうかを示す値を設定します。 |
| [setWriteViewData(boolean value)](#setWriteViewData-boolean-) | プロジェクトを MPP 形式で保存する際にビュー データを書き込むかどうかを示す値を設定します。 |
### MPPSaveOptions() {#MPPSaveOptions--}
```
public MPPSaveOptions()
```


新しい [MPPSaveOptions](../../com.aspose.tasks/mppsaveoptions) クラスのインスタンスを初期化します。

### getClearVba() {#getClearVba--}
```
public final boolean getClearVba()
```


プロジェクトを MPP 形式で保存する際に既存の VBA マクロ データを削除するかどうかを示す値を取得します。

**Returns:**
boolean - プロジェクトを MPP 形式で保存する際に既存の VBA マクロ データを削除するかどうかを示す値。
### getProtectionPassword() {#getProtectionPassword--}
```
public final String getProtectionPassword()
```


生成された MPP ファイルを保護するために使用されるパスワードを取得します。現在、MS Project 2010 以降の形式がサポートされています。

--------------------

null 値はプロジェクト ファイルが保護されていないことを示します。

**Returns:**
java.lang.String - 生成された MPP ファイルを保護するために使用されるパスワード。
### getRemoveInvalidAssignments() {#getRemoveInvalidAssignments--}
```
public final boolean getRemoveInvalidAssignments()
```


MPP に保存する際に無効なリソース割り当てを削除するかどうかを示す値を取得します。

--------------------

MS Project は各タスクに対して空のリソース割り当てを作成します。保存時にそれらを削除するには、このフラグを true に設定します。

**Returns:**
boolean - MPP に保存する際に無効なリソース割り当てを削除するかどうかを示す値。
### getWriteFilters() {#getWriteFilters--}
```
public final boolean getWriteFilters()
```


プロジェクトを MPP 形式で保存する際にフィルタ データを書き込むかどうかを示す値を取得します。

--------------------

フィルター データには Project.TaskFilters と Project.ResourceFilters コレクションが含まれます。

--------------------

現在、MSP 2010 以降の形式がサポートされています。

**Returns:**
boolean - プロジェクトを MPP 形式で保存する際にフィルター データを書き込むかどうかを示す値。
### getWriteGroups() {#getWriteGroups--}
```
public final boolean getWriteGroups()
```


プロジェクトを MPP 形式で保存する際にグループ データを書き込むかどうかを示す値を取得します。

--------------------

グループ データには Project.TaskGroups と Project.ResourceGroups コレクションが含まれます。

**Returns:**
boolean - プロジェクトを MPP 形式で保存する際にグループ データを書き込むかどうかを示す値。
### getWriteVba() {#getWriteVba--}
```
public final boolean getWriteVba()
```


MPP ファイル内の既存の VBA マクロ データを更新するかどうかを示す値を取得します。現在、VbaModule.SourceCode の書き込みがサポートされています。

**Returns:**
boolean - MPP ファイル内の既存の VBA マクロ データを更新するかどうかを示す値。
### getWriteViewData() {#getWriteViewData--}
```
public final boolean getWriteViewData()
```


プロジェクトを MPP 形式で保存する際にビュー データを書き込むかどうかを示す値を取得します。

--------------------

ビュー データには Project.Views、Filters、Tables コレクションが含まれます。

**Returns:**
boolean - プロジェクトを MPP 形式で保存する際にビュー データを書き込むかどうかを示す値。
### setClearVba(boolean value) {#setClearVba-boolean-}
```
public final void setClearVba(boolean value)
```


プロジェクトを MPP 形式で保存する際に既存の VBA マクロ データを削除するかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | プロジェクトを MPP 形式で保存する際に既存の VBA マクロ データを削除するかどうかを示す値。 |

### setProtectionPassword(String value) {#setProtectionPassword-java.lang.String-}
```
public final void setProtectionPassword(String value)
```


生成された MPP ファイルを保護するために使用されるパスワードを設定します。現在、MS Project 2010 以降の形式がサポートされています。

--------------------

null 値はプロジェクト ファイルが保護されていないことを示します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | 生成された MPP ファイルを保護するために使用されるパスワード。 |

### setRemoveInvalidAssignments(boolean value) {#setRemoveInvalidAssignments-boolean-}
```
public final void setRemoveInvalidAssignments(boolean value)
```


MPP に保存する際に無効なリソース割り当てを削除するかどうかを示す値を設定します。

--------------------

MS Project は各タスクに対して空のリソース割り当てを作成します。保存時にそれらを削除するには、このフラグを true に設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | MPP に保存する際に無効なリソース割り当てを削除するかどうかを示す値。 |

### setWriteFilters(boolean value) {#setWriteFilters-boolean-}
```
public final void setWriteFilters(boolean value)
```


プロジェクトを MPP 形式で保存する際にフィルタ データを書き込むかどうかを示す値を設定します。

--------------------

フィルター データには Project.TaskFilters と Project.ResourceFilters コレクションが含まれます。

--------------------

現在、MSP 2010 以降の形式がサポートされています。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | プロジェクトを MPP 形式で保存する際にフィルター データを書き込むかどうかを示す値。 |

### setWriteGroups(boolean value) {#setWriteGroups-boolean-}
```
public final void setWriteGroups(boolean value)
```


プロジェクトを MPP 形式で保存する際にグループ データを書き込むかどうかを示す値を設定します。

--------------------

グループ データには Project.TaskGroups と Project.ResourceGroups コレクションが含まれます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | プロジェクトを MPP 形式で保存する際にグループ データを書き込むかどうかを示す値。 |

### setWriteVba(boolean value) {#setWriteVba-boolean-}
```
public final void setWriteVba(boolean value)
```


MPP ファイル内の既存の VBA マクロ データを更新するかどうかを示す値を設定します。現在、VbaModule.SourceCode の書き込みがサポートされています。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | MPP ファイル内の既存の VBA マクロ データを更新するかどうかを示す値。 |

### setWriteViewData(boolean value) {#setWriteViewData-boolean-}
```
public final void setWriteViewData(boolean value)
```


プロジェクトを MPP 形式で保存する際にビュー データを書き込むかどうかを示す値を設定します。

--------------------

ビュー データには Project.Views、Filters、Tables コレクションが含まれます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | プロジェクトを MPP 形式で保存する際にビュー データを書き込むかどうかを示す値。 |

