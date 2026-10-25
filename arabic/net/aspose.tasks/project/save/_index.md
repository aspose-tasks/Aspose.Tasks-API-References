---
title: "Project.Save"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Project. تحفظ المستند في ملف باستخدام خيارات الحفظ المحددة"
type: docs
weight: 1200
url: /ar/net/aspose.tasks/project/save/
---
## Save(string, SimpleSaveOptions) {#save_4}

يحفظ المستند إلى ملف باستخدام خيارات الحفظ المحددة.

```csharp
public void Save(string filename, SimpleSaveOptions options)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| filename | سلسلة | اسم الملف. |
| خيارات | SimpleSaveOptions | خيارات الحفظ. |

## الأمثلة

يوضح كيفية حفظ المشروع كملف MPP.

```csharp
var project = new Project();
SimpleSaveOptions options = new MPPSaveOptions();
project.Save(OutDir + "EmptyProjectSaveStream_out.xml", options);
```

### انظر أيضًا

* class [SimpleSaveOptions](../../../aspose.tasks.saving/simplesaveoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Save(string, SaveFileFormat) {#save_3}

يحفظ بيانات المشروع إلى الملف.

```csharp
public void Save(string filename, SaveFileFormat format)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| filename | سلسلة | اسم الملف. |
| format | SaveFileFormat | تنسيق ملف الحفظ. |

## الأمثلة

يعرض كيفية إنشاء مشروع وحفظه بتنسيق MPP دون تمرير ملف قالب MPP.

```csharp
var project = new Project();

// سيتم حفظ المشروع بتنسيق MPP باستخدام قالب MPP الداخلي.
project.Save(OutDir + "CreateEmptyProjectSaveMPP_out.mpp", SaveFileFormat.Mpp);
```

### انظر أيضًا

* enum [SaveFileFormat](../../../aspose.tasks.saving/savefileformat/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Save(string) {#save_2}

يحفظ بيانات المشروع إلى الملف بصيغة mpp.

```csharp
public void Save(string filename)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| filename | سلسلة | اسم الملف. |

### انظر أيضًا

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Save(Stream, SimpleSaveOptions) {#save_1}

يحفظ المشروع إلى دفق باستخدام خيارات الحفظ المحددة.

```csharp
public void Save(Stream stream, SimpleSaveOptions options)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| دفق | دفق | الدفق. |
| خيارات | SimpleSaveOptions | خيارات الحفظ. |

## الأمثلة

يوضح كيفية حفظ المشروع في دفق كملف MPP باستخدام خيارات حفظ MPP.

```csharp
using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    var project = new Project();
    SimpleSaveOptions options = new MPPSaveOptions();

    // باستخدام MPPSaveOptions نحفظه بتنسيق MPP.
    project.Save(stream, options);
}
```

يوضح كيفية حفظ المشروع في دفق كصورة والتحكم في خيارات الصورة.

```csharp
var project = new Project();

using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    var options = new ImageSaveOptions(SaveFileFormat.Png);

    // باستخدام ImageSaveOptions نحفظ المشروع بتنسيق صورة
    project.Save(stream, options);
}
```

### انظر أيضًا

* class [SimpleSaveOptions](../../../aspose.tasks.saving/simplesaveoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Save(Stream, SaveFileFormat) {#save}

يحفظ بيانات المشروع إلى الدفق.

```csharp
public void Save(Stream stream, SaveFileFormat format)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| دفق | دفق | الدفق. |
| format | SaveFileFormat | تنسيق ملف الحفظ المحدد.[`SaveFileFormat`](../../../aspose.tasks.saving/savefileformat/) |

## الأمثلة

يوضح كيفية حفظ المشروع في دفق كملف XML لمشروع MS.

```csharp
var project = new Project();

using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    // اكتب الدفق بتنسيق XML
    project.Save(stream, SaveFileFormat.Xml);
}
```

### انظر أيضًا

* enum [SaveFileFormat](../../../aspose.tasks.saving/savefileformat/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


