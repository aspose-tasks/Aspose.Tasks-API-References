---
title: "Timescale"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "विकल्पों को परिभाषित करता है जो यह निर्दिष्ट करते हैं कि प्रोजेक्ट को ग्राफिक फ़ॉर्मेट में निर्यात करने पर Gantt Chart Task Usage या Resource Usage दृश्यों में टाइमस्केल को कैसे रेंडर किया जाए।"
type: docs
weight: 323
url: /hi/java/com.aspose.tasks/timescale/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class Timescale extends System.Enum
```

परियोजना को ग्राफिक फ़ॉर्मेट में निर्यात करते समय गैंट चार्ट, टास्क उपयोग या रिसोर्स उपयोग दृश्यों में टाइमस्केल को कैसे रेंडर किया जाए, इसे निर्दिष्ट करने वाले विकल्पों को परिभाषित करता है।
## फ़ील्ड्स

| फ़ील्ड | विवरण |
| --- | --- |
| [Days](#Days) | पूर्वनिर्धारित दो-स्तरीय टाइमस्केल जहाँ न्यूनतम विवरण स्तर एक दिन है। |
| [DefinedInView](#DefinedInView) | परियोजना दृश्य की गुणों में परिभाषित टाइमस्केल सेटिंग्स का उपयोग करें: `GanttChartView.BottomTimescaleTier`([GanttChartView.getBottomTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getBottomTimescaleTier--)/[GanttChartView.setBottomTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setBottomTimescaleTier-TimescaleTier-)), `GanttChartView.MiddleTimescaleTier`([GanttChartView.getMiddleTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getMiddleTimescaleTier--)/[GanttChartView.setMiddleTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setMiddleTimescaleTier-TimescaleTier-)), `GanttChartView.TopTimescaleTier`([GanttChartView.getTopTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getTopTimescaleTier--)/[GanttChartView.setTopTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setTopTimescaleTier-TimescaleTier-)). |
| [Months](#Months) | पूर्वनिर्धारित दो-स्तरीय टाइमस्केल जहाँ न्यूनतम विवरण स्तर एक माह है। |
| [ThirdsOfMonths](#ThirdsOfMonths) | पूर्वनिर्धारित दो-स्तरीय टाइमस्केल जहाँ विवरण का स्तर महीने का एक तिहाई होता है। |
### Days {#Days}
```
public static final int Days
```


पूर्वनिर्धारित दो-स्तरीय टाइमस्केल जहाँ न्यूनतम विवरण स्तर एक दिन है।

### DefinedInView {#DefinedInView}
```
public static final int DefinedInView
```


परियोजना दृश्य की प्रॉपर्टीज़ में परिभाषित टाइमस्केल सेटिंग्स का उपयोग करें: `GanttChartView.BottomTimescaleTier`([GanttChartView.getBottomTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getBottomTimescaleTier--)/[GanttChartView.setBottomTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setBottomTimescaleTier-TimescaleTier-)), `GanttChartView.MiddleTimescaleTier`([GanttChartView.getMiddleTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getMiddleTimescaleTier--)/[GanttChartView.setMiddleTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setMiddleTimescaleTier-TimescaleTier-)), `GanttChartView.TopTimescaleTier`([GanttChartView.getTopTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getTopTimescaleTier--)/[GanttChartView.setTopTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setTopTimescaleTier-TimescaleTier-)). यह उन फ़ॉर्मैट्स के लिए मान्य है जिनमें दृश्य डेटा शामिल है। उदाहरण के लिए, वे परियोजनाएँ जो MPP फ़ॉर्मेट से पढ़ी गई हैं।

--------------------

यदि दृश्य के लिए टाइमस्केल सेटिंग्स सेट नहीं की गई हैं, तो पूर्वनिर्धारित Timescale.Days सेटिंग का उपयोग किया जाता है।

### Months {#Months}
```
public static final int Months
```


पूर्वनिर्धारित दो-स्तरीय टाइमस्केल जहाँ न्यूनतम विवरण स्तर एक माह है।

### ThirdsOfMonths {#ThirdsOfMonths}
```
public static final int ThirdsOfMonths
```


पूर्वनिर्धारित दो-स्तरीय टाइमस्केल जहाँ विवरण का स्तर महीने का एक तिहाई होता है।

