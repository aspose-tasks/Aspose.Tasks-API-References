---
title: "PixelFormat"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يحدد تنسيق بيانات اللون لكل بكسل في الصورة."
type: docs
weight: 193
url: /ar/java/com.aspose.tasks/pixelformat/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class PixelFormat extends System.Enum
```

يحدد تنسيق بيانات اللون لكل بكسل في الصورة.
## الحقول

| حقل | الوصف |
| --- | --- |
| [Alpha](#Alpha) | بيانات البكسل تحتوي على قيم ألفا غير مضاعفة مسبقًا. |
| [Canonical](#Canonical) | تنسيق البكسل الافتراضي 32 بت لكل بكسل. |
| [DontCare](#DontCare) | لم يتم تحديد تنسيق البكسل. |
| [Extended](#Extended) | محجوز. |
| [Format16bppArgb1555](#Format16bppArgb1555) | تنسيق البكسل هو 16 بت لكل بكسل. |
| [Format16bppGrayScale](#Format16bppGrayScale) | تنسيق البكسل هو 16 بت لكل بكسل. |
| [Format16bppRgb555](#Format16bppRgb555) | يحدد أن التنسيق هو 16 بت لكل بكسل؛ تُستخدم 5 بت لكل من مكونات الأحمر والأخضر والأزرق. |
| [Format16bppRgb565](#Format16bppRgb565) | يحدد أن التنسيق هو 16 بت لكل بكسل؛ تُستخدم 5 بت للمكون الأحمر، و6 بت للمكون الأخضر، و5 بت للمكون الأزرق. |
| [Format1bppIndexed](#Format1bppIndexed) | يحدد أن تنسيق البكسل هو 1 بت لكل بكسل وأنه يستخدم ألوانًا مفهرسة. |
| [Format24bppRgb](#Format24bppRgb) | يحدد أن التنسيق هو 24 بت لكل بكسل؛ تُستخدم 8 بت لكل من مكونات الأحمر والأخضر والأزرق. |
| [Format32bppArgb](#Format32bppArgb) | يحدد أن التنسيق هو 32 بت لكل بكسل؛ تُستخدم 8 بت لكل من مكونات ألفا، الأحمر، الأخضر، والأزرق. |
| [Format32bppPArgb](#Format32bppPArgb) | يحدد أن التنسيق هو 32 بت لكل بكسل؛ تُستخدم 8 بت لكل من مكونات ألفا، الأحمر، الأخضر، والأزرق. |
| [Format32bppRgb](#Format32bppRgb) | يحدد أن التنسيق هو 32 بت لكل بكسل؛ تُستخدم 8 بت لكل من مكونات الأحمر والأخضر والأزرق. |
| [Format48bppRgb](#Format48bppRgb) | يحدد أن التنسيق هو 48 بت لكل بكسل؛ تُستخدم 16 بت لكل من مكونات الأحمر والأخضر والأزرق. |
| [Format4bppIndexed](#Format4bppIndexed) | يحدد أن التنسيق هو 4 بت لكل بكسل، مفهرس. |
| [Format64bppArgb](#Format64bppArgb) | يحدد أن التنسيق هو 64 بت لكل بكسل؛ تُستخدم 16 بت لكل من مكونات ألفا، الأحمر، الأخضر، والأزرق. |
| [Format64bppPArgb](#Format64bppPArgb) | يحدد أن التنسيق هو 64 بت لكل بكسل؛ تُستخدم 16 بت لكل من مكونات ألفا، الأحمر، الأخضر، والأزرق. |
| [Format8bppIndexed](#Format8bppIndexed) | يحدد أن التنسيق هو 8 بت لكل بكسل، مفهرس. |
| [Gdi](#Gdi) | تحتوي بيانات البكسل على ألوان GDI. |
| [Indexed](#Indexed) | تحتوي بيانات البكسل على قيم مفهرسة بالألوان، مما يعني أن القيم هي فهرس للألوان في جدول ألوان النظام، بدلاً من قيم ألوان فردية. |
| [Max](#Max) | القيمة القصوى لهذا التعداد. |
| [PAlpha](#PAlpha) | تنسيق البكسل يحتوي على قيم ألفا مضاعفة مسبقًا. |
| [Undefined](#Undefined) | تنسيق البكسل غير معرف. |
### Alpha {#Alpha}
```
public static final int Alpha
```


بيانات البكسل تحتوي على قيم ألفا غير مضاعفة مسبقًا.

### Canonical {#Canonical}
```
public static final int Canonical
```


تنسيق البكسل الافتراضي هو 32 بت لكل بكسل. يحدد التنسيق عمق لون 24 بت وقناة ألفا 8 بت.

### DontCare {#DontCare}
```
public static final int DontCare
```


لم يتم تحديد تنسيق البكسل.

### Extended {#Extended}
```
public static final int Extended
```


محجوز.

### Format16bppArgb1555 {#Format16bppArgb1555}
```
public static final int Format16bppArgb1555
```


تنسيق البكسل هو 16 بت لكل بكسل. تحدد معلومات اللون 32,768 درجة لون، حيث 5 بت للأحمر، 5 بت للأخضر، 5 بت للأزرق، و1 بت لألفا.

### Format16bppGrayScale {#Format16bppGrayScale}
```
public static final int Format16bppGrayScale
```


تنسيق البكسل هو 16 بت لكل بكسل. تحدد معلومات اللون 65,536 درجة من الرمادي.

### Format16bppRgb555 {#Format16bppRgb555}
```
public static final int Format16bppRgb555
```


يحدد أن التنسيق هو 16 بت لكل بكسل؛ تُستخدم 5 بت لكل من مكونات الأحمر والأخضر والأزرق. البت المتبقي غير مستخدم.

### Format16bppRgb565 {#Format16bppRgb565}
```
public static final int Format16bppRgb565
```


يحدد أن التنسيق هو 16 بت لكل بكسل؛ تُستخدم 5 بت للمكون الأحمر، و6 بت للمكون الأخضر، و5 بت للمكون الأزرق.

### Format1bppIndexed {#Format1bppIndexed}
```
public static final int Format1bppIndexed
```


يحدد أن تنسيق البكسل هو 1 بت لكل بكسل وأنه يستخدم ألوانًا مفهرسة. وبالتالي يحتوي جدول الألوان على لونين.

### Format24bppRgb {#Format24bppRgb}
```
public static final int Format24bppRgb
```


يحدد أن التنسيق هو 24 بت لكل بكسل؛ تُستخدم 8 بت لكل من مكونات الأحمر والأخضر والأزرق.

### Format32bppArgb {#Format32bppArgb}
```
public static final int Format32bppArgb
```


يحدد أن التنسيق هو 32 بت لكل بكسل؛ تُستخدم 8 بت لكل من مكونات ألفا، الأحمر، الأخضر، والأزرق.

### Format32bppPArgb {#Format32bppPArgb}
```
public static final int Format32bppPArgb
```


يحدد أن التنسيق هو 32 بت لكل بكسل؛ تُستخدم 8 بت لكل من مكونات ألفا، الأحمر، الأخضر، والأزرق. مكونات الأحمر والأخضر والأزرق مضاعفة مسبقًا وفقًا لمكون ألفا.

### Format32bppRgb {#Format32bppRgb}
```
public static final int Format32bppRgb
```


يحدد أن التنسيق هو 32 بت لكل بكسل؛ تُستخدم 8 بت لكل من مكونات الأحمر والأخضر والأزرق. الـ 8 بت المتبقية غير مستخدمة.

### Format48bppRgb {#Format48bppRgb}
```
public static final int Format48bppRgb
```


يحدد أن التنسيق هو 48 بت لكل بكسل؛ تُستخدم 16 بت لكل من مكونات الأحمر والأخضر والأزرق.

### Format4bppIndexed {#Format4bppIndexed}
```
public static final int Format4bppIndexed
```


يحدد أن التنسيق هو 4 بت لكل بكسل، مفهرس.

### Format64bppArgb {#Format64bppArgb}
```
public static final int Format64bppArgb
```


يحدد أن التنسيق هو 64 بت لكل بكسل؛ تُستخدم 16 بت لكل من مكونات ألفا، الأحمر، الأخضر، والأزرق.

### Format64bppPArgb {#Format64bppPArgb}
```
public static final int Format64bppPArgb
```


يحدد أن التنسيق هو 64 بت لكل بكسل؛ تُستخدم 16 بت لكل من مكوّنات ألفا، الأحمر، الأخضر، والأزرق. مكوّنات الأحمر، الأخضر، والأزرق مضاعفة مسبقًا وفقًا لمكوّن ألفا.

### Format8bppIndexed {#Format8bppIndexed}
```
public static final int Format8bppIndexed
```


يحدد أن التنسيق هو 8 بت لكل بكسل، مفهرس. وبالتالي يحتوي جدول الألوان على 256 لونًا.

### Gdi {#Gdi}
```
public static final int Gdi
```


تحتوي بيانات البكسل على ألوان GDI.

### Indexed {#Indexed}
```
public static final int Indexed
```


تحتوي بيانات البكسل على قيم مفهرسة بالألوان، مما يعني أن القيم هي فهرس للألوان في جدول ألوان النظام، بدلاً من قيم ألوان فردية.

### Max {#Max}
```
public static final int Max
```


القيمة القصوى لهذا التعداد.

### PAlpha {#PAlpha}
```
public static final int PAlpha
```


تنسيق البكسل يحتوي على قيم ألفا مضاعفة مسبقًا.

### Undefined {#Undefined}
```
public static final int Undefined
```


تنسيق البكسل غير معرف.

