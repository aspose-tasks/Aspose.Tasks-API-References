---
title: "UsageView.AlignDetailsData"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "UsageView property. विवरण डेटा संरेखण को प्राप्त या सेट करता है"
type: docs
weight: 10
url: /hi/net/aspose.tasks/usageview/aligndetailsdata/
---
## UsageView.AlignDetailsData property

विवरण डेटा संरेखण को प्राप्त करता है या सेट करता है।

```csharp
public HorizontalStringAlignment AlignDetailsData { get; set; }
```

## उदाहरण

विवरणों के साथ टास्क उपयोग दृश्य को रेंडर करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "TaskUsageViewWithDetails.mpp");

// दृश्य प्राप्त करें
UsageView view = (TaskUsageView)project.DefaultView;

// विवरण हेडर कॉलम प्रदर्शित नहीं होगा
view.DisplayDetailsHeaderColumn = false;
view.RepeatDetailsHeaderOnAllRows = false;
view.DisplayShortDetailHeaderNames = false;
view.AlignDetailsData = HorizontalStringAlignment.Near;
project.Save(OutDir + "task usage1_out.pdf", SaveFileFormat.Pdf);

// विवरण हेडर कॉलम प्रदर्शित करें
view.DisplayDetailsHeaderColumn = true;

// सभी असाइनमेंट पंक्तियों पर विवरण हेडर दोहराएँ
view.RepeatDetailsHeaderOnAllRows = true;
view.AlignDetailsData = HorizontalStringAlignment.Far;
project.Save(OutDir + "task usage2_out.pdf", SaveFileFormat.Pdf);
```

### संबंधित देखें

* enum [HorizontalStringAlignment](../../../aspose.tasks.visualization/horizontalstringalignment/)
* class [UsageView](../)
* namespace [Aspose.Tasks](../../usageview/)
* assembly [Aspose.Tasks](../../../)


