---
title: "مقياس الزمن"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يحدد الخيارات التي تحدد كيفية عرض مقياس الزمن في عروض مخطط جانت لاستخدام المهام أو استخدام الموارد عندما يتم تصدير المشروع إلى تنسيق رسومي."
type: docs
weight: 323
url: /ar/java/com.aspose.tasks/timescale/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class Timescale extends System.Enum
```

يحدد الخيارات التي تحدد كيفية عرض مقياس الوقت في مخطط جانت أو عرض استخدام المهمة أو عرض استخدام الموارد عندما يتم تصدير المشروع إلى تنسيق رسومي.
## الحقول

| حقل | الوصف |
| --- | --- |
| [Days](#Days) | مقياس زمن ثنائي الطبقات محدد مسبقًا حيث الحد الأدنى للتفصيل هو يوم واحد. |
| [DefinedInView](#DefinedInView) | استخدم إعدادات مقياس الزمن المحددة في خصائص عرض المشروع: `GanttChartView.BottomTimescaleTier`([GanttChartView.getBottomTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getBottomTimescaleTier--)/[GanttChartView.setBottomTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setBottomTimescaleTier-TimescaleTier-)), `GanttChartView.MiddleTimescaleTier`([GanttChartView.getMiddleTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getMiddleTimescaleTier--)/[GanttChartView.setMiddleTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setMiddleTimescaleTier-TimescaleTier-)), `GanttChartView.TopTimescaleTier`([GanttChartView.getTopTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getTopTimescaleTier--)/[GanttChartView.setTopTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setTopTimescaleTier-TimescaleTier-)). |
| [Months](#Months) | مقياس زمن ثنائي الطبقات محدد مسبقًا حيث الحد الأدنى للتفصيل هو شهر واحد. |
| [ThirdsOfMonths](#ThirdsOfMonths) | مقياس زمني ثنائي المستوى محدد مسبقًا حيث مستوى التفاصيل هو ثلث الشهر. |
### Days {#Days}
```
public static final int Days
```


مقياس زمن ثنائي الطبقات محدد مسبقًا حيث الحد الأدنى للتفصيل هو يوم واحد.

### DefinedInView {#DefinedInView}
```
public static final int DefinedInView
```


استخدم إعدادات المقياس الزمني المحددة في خصائص عرض المشروع: `GanttChartView.BottomTimescaleTier`([GanttChartView.getBottomTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getBottomTimescaleTier--)/[GanttChartView.setBottomTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setBottomTimescaleTier-TimescaleTier-)), `GanttChartView.MiddleTimescaleTier`([GanttChartView.getMiddleTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getMiddleTimescaleTier--)/[GanttChartView.setMiddleTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setMiddleTimescaleTier-TimescaleTier-)), `GanttChartView.TopTimescaleTier`([GanttChartView.getTopTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getTopTimescaleTier--)/[GanttChartView.setTopTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setTopTimescaleTier-TimescaleTier-)). صالحة للتنسيقات التي تحتوي على بيانات العرض. على سبيل المثال، المشاريع التي تُقرأ من تنسيق MPP.

--------------------

إذا لم يتم تعيين إعدادات المقياس الزمني للعرض، يتم استخدام إعداد Timescale.Days المحدد مسبقًا بدلاً من ذلك.

### Months {#Months}
```
public static final int Months
```


مقياس زمن ثنائي الطبقات محدد مسبقًا حيث الحد الأدنى للتفصيل هو شهر واحد.

### ThirdsOfMonths {#ThirdsOfMonths}
```
public static final int ThirdsOfMonths
```


مقياس زمني ثنائي المستوى محدد مسبقًا حيث مستوى التفاصيل هو ثلث الشهر.

