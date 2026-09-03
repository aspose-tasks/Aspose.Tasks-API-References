---
title: "Aspose::Tasks::Project::SaveReport メソッド"
linktitle: "SaveReport"
articleTitle: "SaveReport"
second_title: "Aspose.Tasks for C++"
description: "プロジェクト概要レポートをストリームに保存します。"
type: docs
weight: 1210
url: /ja/cpp/aspose.tasks/project/savereport/
---

## SaveReport (1 of 4) {#savereport_1}

プロジェクト概要レポートをストリームに保存します。

**Returns:** void Aspose::Tasks::

```cpp
SaveReport(const System::SharedPtr< System::IO::Stream > & stream)
```

| パラメーター | 説明 |
| --- | --- |
| stream | プロジェクトレポートを保存するストリーム。 |

---

## SaveReport (2 of 4) {#savereport_2}

指定されたタイプのプロジェクトレポートを指定されたストリームに保存します。

**Returns:** void Aspose::Tasks::

```cpp
SaveReport(const System::SharedPtr< System::IO::Stream > & stream, Visualization::ReportType reportType)
```

| パラメーター | 説明 |
| --- | --- |
| stream | プロジェクトレポートを保存する指定されたストリーム。 |
| reportType | 指定されたレポートタイプ。ReportType |

---

## SaveReport (3 of 4) {#savereport_3}

プロジェクト概要レポートをPDFファイルに保存します。

**Returns:** void Aspose::Tasks::

```cpp
SaveReport(const System::String & fileName)
```

| パラメーター | 説明 |
| --- | --- |
| fileName | ファイル名。 |

---

## SaveReport (4 of 4) {#savereport_4}

指定されたタイプのプロジェクトレポートをPDF形式で指定されたファイルパスに保存します。

**Returns:** void Aspose::Tasks::

```cpp
SaveReport(const System::String & fileName, Visualization::ReportType reportType)
```

| パラメーター | 説明 |
| --- | --- |
| fileName | 指定されたファイル名。 |
| reportType | 指定されたレポートタイプ。ReportType |

