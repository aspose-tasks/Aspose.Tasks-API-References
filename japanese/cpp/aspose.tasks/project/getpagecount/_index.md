---
title: "Aspose::Tasks::Project::GetPageCount メソッド"
linktitle: "GetPageCount"
articleTitle: "GetPageCount"
second_title: "Aspose.Tasks for C++"
description: "デフォルトの Timescale（Days）を使用してレンダリングされるプロジェクトのページ数を返します。"
type: docs
weight: 1090
url: /ja/cpp/aspose.tasks/project/getpagecount/
---

## GetPageCount (1 of 7) {#getpagecount_1}

デフォルトの Timescale（Days）を使用してレンダリングされるプロジェクトのページ数を返します。

**Returns:** Page count to be rendered.

```cpp
GetPageCount()
```

---

## GetPageCount (2 of 7) {#getpagecount_2}

指定された SaveOptions を使用してレンダリングされるプロジェクトのページ数を返します。

**Returns:** a page count to be rendered.

```cpp
GetPageCount(const System::SharedPtr< Saving::SaveOptions > & saveOptions)
```

| パラメーター | 説明 |
| --- | --- |
| saveOptions | ページ数を取得するための保存オプション。 |

---

## GetPageCount (3 of 7) {#getpagecount_3}

指定されたタイムスケールとページサイズを使用してレンダリングされるプロジェクトのページ数を返します。

**Returns:** Page count to be rendered.

```cpp
GetPageCount(Visualization::PageSize pageSize, Visualization::Timescale scale)
```

| パラメーター | 説明 |
| --- | --- |
| pageSize | ページ数を取得するためのサイズです。 |
| scale | ページ数を取得するためのスケールです。 |

---

## GetPageCount (4 of 7) {#getpagecount_4}

指定されたタイムスケール、プレゼンテーション形式、および日付範囲を使用してレンダリングされるプロジェクトのページ数を返します。

**Returns:** Page count to be rendered.

```cpp
GetPageCount(Visualization::PageSize pageSize, Visualization::Timescale scale, System::DateTime startDate, System::DateTime endDate)
```

| パラメーター | 説明 |
| --- | --- |
| pageSize | ページ数を取得するためのサイズです。 |
| scale | ページ数を取得するためのスケールです。 |
| startDate | ページ数を取得する開始日です。 |
| endDate | ページ数を取得する終了日です。 |

---

## GetPageCount (5 of 7) {#getpagecount_5}

デフォルトのタイムスケール（日）と指定されたプレゼンテーション形式を使用してレンダリングされるプロジェクトのページ数を返します。

**Returns:** Page count to be rendered.

```cpp
GetPageCount(Visualization::PresentationFormat format)
```

| パラメーター | 説明 |
| --- | --- |
| 形式 | ページ数を取得する形式です。 |

---

## GetPageCount (6 of 7) {#getpagecount_6}

指定されたタイムスケールとプレゼンテーション形式を使用してレンダリングされるプロジェクトのページ数を返します。

**Returns:** a page count to be rendered.

```cpp
GetPageCount(Visualization::PresentationFormat format, Visualization::Timescale scale)
```

| パラメーター | 説明 |
| --- | --- |
| 形式 | ページ数を取得する形式です。 |
| scale | ページ数を取得するためのスケールです。 |

---

## GetPageCount (7 of 7) {#getpagecount_7}

指定されたタイムスケールを使用してレンダリングされるプロジェクトのページ数を返します。

**Returns:** Page count to be rendered.

```cpp
GetPageCount(Visualization::Timescale scale)
```

| パラメーター | 説明 |
| --- | --- |
| scale | ページ数を取得するためのスケールです。 |

