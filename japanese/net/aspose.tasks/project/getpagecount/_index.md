---
title: GetPageCount
second_title: Aspose.Tasks for .NET API リファレンス
description: 指定されたものを使用してレンダリングされるプロジェクトのページ数を返しますSaveOptionsaspose.tasks.saving/saveoptions/.
type: docs
weight: 1080
url: /ja/net/aspose.tasks/project/getpagecount/
---
## GetPageCount(SaveOptions) {#getpagecount_1}

指定されたものを使用してレンダリングされるプロジェクトのページ数を返します[`SaveOptions`](../../../aspose.tasks.saving/saveoptions/).

```csharp
public int GetPageCount(SaveOptions saveOptions)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| saveOptions | SaveOptions | ページ数を取得する保存オプション。 |

### 戻り値

レンダリングされるページ数。

### 例

この例では、HtmlSaveOptions のインスタンスと結果の HTML のページ数がコンソールに書き込まれます。

```csharp
[C#]
Project project = new Project(@"test.mpp");
HtmlSaveOptions saveOptions = new HtmlSaveOptions
{
    IncludeProjectNameInPageHeader = false,
    IncludeProjectNameInTitle = false,
    PageSize = PageSize.A4,
    Timescale = Timescale.Days,
    StartDate = project.Get(Prj.StartDate).Date,
    EndDate = project.Get(Prj.FinishDate).Date
};

Console.WriteLine(project.GetPageCount(saveOptions));
```

### 関連項目

* class [SaveOptions](../../../aspose.tasks.saving/saveoptions/)
* class [Project](../)
* 名前空間 [Aspose.Tasks](../../project/)
* 組み立て [Aspose.Tasks](../../../)

---

## GetPageCount() {#getpagecount}

デフォルトを使用してレンダリングされるプロジェクトのページ数を返します[`Timescale`](../../../aspose.tasks.visualization/timescale/)(日).

```csharp
public int GetPageCount()
```

### 戻り値

レンダリングするページ数。

### 関連項目

* class [Project](../)
* 名前空間 [Aspose.Tasks](../../project/)
* 組み立て [Aspose.Tasks](../../../)

---

## GetPageCount(Timescale) {#getpagecount_6}

指定されたものを使用してレンダリングされるプロジェクトのページ数を返します[`Timescale`](../../../aspose.tasks.visualization/timescale/).

```csharp
public int GetPageCount(Timescale scale)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| scale | Timescale | ページ数を取得するスケール。 |

### 戻り値

レンダリングするページ数。

### 関連項目

* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* 名前空間 [Aspose.Tasks](../../project/)
* 組み立て [Aspose.Tasks](../../../)

---

## GetPageCount(PresentationFormat) {#getpagecount_4}

デフォルトを使用してレンダリングされるプロジェクトのページ数を返します[`Timescale`](../../../aspose.tasks.visualization/timescale/) (日) および与えられた[`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/)

```csharp
public int GetPageCount(PresentationFormat format)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| format | PresentationFormat | ページ数を取得する形式。 |

### 戻り値

レンダリングするページ数。

### 関連項目

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat/)
* class [Project](../)
* 名前空間 [Aspose.Tasks](../../project/)
* 組み立て [Aspose.Tasks](../../../)

---

## GetPageCount(PresentationFormat, Timescale) {#getpagecount_5}

指定されたものを使用してレンダリングされるプロジェクトのページ数を返します[`Timescale`](../../../aspose.tasks.visualization/timescale/)と[`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/).

```csharp
public int GetPageCount(PresentationFormat format, Timescale scale)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| format | PresentationFormat | ページ数を取得する形式。 |
| scale | Timescale | ページ数を取得するスケール。 |

### 戻り値

レンダリングされるページ数。

### 関連項目

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* 名前空間 [Aspose.Tasks](../../project/)
* 組み立て [Aspose.Tasks](../../../)

---

## GetPageCount(PageSize, Timescale, DateTime, DateTime) {#getpagecount_3}

指定されたものを使用してレンダリングされるプロジェクトのページ数を返します[`Timescale`](../../../aspose.tasks.visualization/timescale/)、[`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/)および日付範囲.

```csharp
public int GetPageCount(PageSize pageSize, Timescale scale, DateTime startDate, DateTime endDate)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| pageSize | PageSize | ページ数を取得するサイズ。 |
| scale | Timescale | ページ数を取得するスケール。 |
| startDate | DateTime | ページ数を取得する開始日。 |
| endDate | DateTime | ページ数を取得する終了日。 |

### 戻り値

レンダリングするページ数。

### 関連項目

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* 名前空間 [Aspose.Tasks](../../project/)
* 組み立て [Aspose.Tasks](../../../)

---

## GetPageCount(PageSize, Timescale) {#getpagecount_2}

指定されたものを使用してレンダリングされるプロジェクトのページ数を返します[`Timescale`](../../../aspose.tasks.visualization/timescale/)と[`PageSize`](../../../aspose.tasks.visualization/pagesize/).

```csharp
public int GetPageCount(PageSize pageSize, Timescale scale)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| pageSize | PageSize | ページ数を取得するサイズ。 |
| scale | Timescale | ページ数を取得するスケール。 |

### 戻り値

レンダリングするページ数。

### 関連項目

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* 名前空間 [Aspose.Tasks](../../project/)
* 組み立て [Aspose.Tasks](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->