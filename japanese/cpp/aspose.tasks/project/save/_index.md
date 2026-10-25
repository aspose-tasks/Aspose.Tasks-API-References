---
title: "Aspose::Tasks::Project::Save メソッド"
linktitle: "Save"
articleTitle: "Save"
second_title: "Aspose.Tasks for C++"
description: "指定された保存オプションを使用してプロジェクトをストリームに保存します。"
type: docs
weight: 1190
url: /ja/cpp/aspose.tasks/project/save/
---

## Save (1 of 5) {#save_1}

指定された保存オプションを使用してプロジェクトをストリームに保存します。

**Returns:** void Aspose::Tasks::

```cpp
Save(const System::SharedPtr< System::IO::Stream > & stream, const System::SharedPtr< Saving::SimpleSaveOptions > & options)
```

| パラメーター | 説明 |
| --- | --- |
| stream | このストリーム。 |
| options | この保存オプション。 |

---

## Save (2 of 5) {#save_2}

プロジェクト データをストリームに保存します。

**Returns:** void Aspose::Tasks::

```cpp
Save(const System::SharedPtr< System::IO::Stream > & stream, Saving::SaveFileFormat format)
```

| パラメーター | 説明 |
| --- | --- |
| stream | このストリーム。 |
| 形式 | 指定された保存ファイル形式。 SaveFileFormat |

---

## Save (3 of 5) {#save_3}

プロジェクト データを mpp 形式のファイルに保存します。

**Returns:** void Aspose::Tasks::

```cpp
Save(const System::String & filename)
```

| パラメーター | 説明 |
| --- | --- |
| ファイル名 | ファイル名。 |

---

## Save (4 of 5) {#save_4}

指定された保存オプションを使用して、ドキュメントをファイルに保存します。

**Returns:** void Aspose::Tasks::

```cpp
Save(const System::String & filename, const System::SharedPtr< Saving::SimpleSaveOptions > & options)
```

| パラメーター | 説明 |
| --- | --- |
| ファイル名 | ファイル名。 |
| options | この保存オプション。 |

---

## Save (5 of 5) {#save_5}

プロジェクト データをファイルに保存します。

**Returns:** void Aspose::Tasks::

```cpp
Save(const System::String & filename, Saving::SaveFileFormat format)
```

| パラメーター | 説明 |
| --- | --- |
| ファイル名 | ファイル名。 |
| 形式 | この保存ファイル形式。 |

