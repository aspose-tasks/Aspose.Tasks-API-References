---
title: Project.GetPageCount
second_title: Aspose.Tasks لمرجع .NET API
description: Project طريقة. إرجاع عدد الصفحات للمشروع الذي سيتم عرضه باستخدام ما هو محددSaveOptions .
type: docs
weight: 1080
url: /ar/net/aspose.tasks/project/getpagecount/
---
## GetPageCount(SaveOptions) {#getpagecount_1}

إرجاع عدد الصفحات للمشروع الذي سيتم عرضه باستخدام ما هو محدد[`SaveOptions`](../../../aspose.tasks.saving/saveoptions/) .

```csharp
public int GetPageCount(SaveOptions saveOptions)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| saveOptions | SaveOptions | خيارات الحفظ للحصول على عدد الصفحات. |

### قيمة الإرجاع

عدد الصفحات التي سيتم عرضها.

### أمثلة

في هذا المثال ، تتم كتابة مثيل HtmlSaveOptions وعدد الصفحات في HTML الناتج إلى وحدة التحكم.

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

### أنظر أيضا

* class [SaveOptions](../../../aspose.tasks.saving/saveoptions/)
* class [Project](../)
* مساحة الاسم [Aspose.Tasks](../../project/)
* المجسم [Aspose.Tasks](../../../)

---

## GetPageCount() {#getpagecount}

إرجاع عدد الصفحات للمشروع الذي سيتم عرضه باستخدام الافتراضي[`Timescale`](../../../aspose.tasks.visualization/timescale/) (أيام) .

```csharp
public int GetPageCount()
```

### قيمة الإرجاع

عدد الصفحات المراد تقديمها.

### أنظر أيضا

* class [Project](../)
* مساحة الاسم [Aspose.Tasks](../../project/)
* المجسم [Aspose.Tasks](../../../)

---

## GetPageCount(Timescale) {#getpagecount_6}

إرجاع عدد الصفحات للمشروع الذي سيتم عرضه باستخدام ما هو محدد[`Timescale`](../../../aspose.tasks.visualization/timescale/) .

```csharp
public int GetPageCount(Timescale scale)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| scale | Timescale | المقياس المطلوب حساب عدد الصفحات له. |

### قيمة الإرجاع

عدد الصفحات المراد تقديمها.

### أنظر أيضا

* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* مساحة الاسم [Aspose.Tasks](../../project/)
* المجسم [Aspose.Tasks](../../../)

---

## GetPageCount(PresentationFormat) {#getpagecount_4}

إرجاع عدد الصفحات للمشروع الذي سيتم عرضه باستخدام الافتراضي[`Timescale`](../../../aspose.tasks.visualization/timescale/) (أيام) ومعطاء[`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/)

```csharp
public int GetPageCount(PresentationFormat format)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| format | PresentationFormat | تنسيق الحصول على عدد الصفحات. |

### قيمة الإرجاع

عدد الصفحات المراد تقديمها.

### أنظر أيضا

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat/)
* class [Project](../)
* مساحة الاسم [Aspose.Tasks](../../project/)
* المجسم [Aspose.Tasks](../../../)

---

## GetPageCount(PresentationFormat, Timescale) {#getpagecount_5}

إرجاع عدد الصفحات للمشروع الذي سيتم عرضه باستخدام ما هو محدد[`Timescale`](../../../aspose.tasks.visualization/timescale/) و[`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) .

```csharp
public int GetPageCount(PresentationFormat format, Timescale scale)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| format | PresentationFormat | تنسيق الحصول على عدد الصفحات. |
| scale | Timescale | المقياس المطلوب حساب عدد الصفحات له. |

### قيمة الإرجاع

عدد الصفحات التي سيتم عرضها.

### أنظر أيضا

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* مساحة الاسم [Aspose.Tasks](../../project/)
* المجسم [Aspose.Tasks](../../../)

---

## GetPageCount(PageSize, Timescale, DateTime, DateTime) {#getpagecount_3}

إرجاع عدد الصفحات للمشروع الذي سيتم عرضه باستخدام ما هو محدد[`Timescale`](../../../aspose.tasks.visualization/timescale/) و[`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) ونطاق التاريخ.

```csharp
public int GetPageCount(PageSize pageSize, Timescale scale, DateTime startDate, DateTime endDate)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| pageSize | PageSize | الحجم المطلوب حساب عدد الصفحات له. |
| scale | Timescale | المقياس المطلوب حساب عدد الصفحات له. |
| startDate | DateTime | تاريخ البدء للحصول على عدد الصفحات. |
| endDate | DateTime | تاريخ الانتهاء للحصول على عدد الصفحات. |

### قيمة الإرجاع

عدد الصفحات المراد تقديمها.

### أنظر أيضا

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* مساحة الاسم [Aspose.Tasks](../../project/)
* المجسم [Aspose.Tasks](../../../)

---

## GetPageCount(PageSize, Timescale) {#getpagecount_2}

إرجاع عدد الصفحات للمشروع الذي سيتم عرضه باستخدام ما هو محدد[`Timescale`](../../../aspose.tasks.visualization/timescale/) و[`PageSize`](../../../aspose.tasks.visualization/pagesize/) .

```csharp
public int GetPageCount(PageSize pageSize, Timescale scale)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| pageSize | PageSize | الحجم المطلوب حساب عدد الصفحات له. |
| scale | Timescale | المقياس المطلوب حساب عدد الصفحات له. |

### قيمة الإرجاع

عدد الصفحات المراد تقديمها.

### أنظر أيضا

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* مساحة الاسم [Aspose.Tasks](../../project/)
* المجسم [Aspose.Tasks](../../../)


