---
title: "UsageView.DisplayDetailsHeaderColumn"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "UsageView प्रॉपर्टी। प्राप्त करता है या सेट करता है एक मान जो दर्शाता है कि व्यू में विवरण हेडर कॉलम प्रदर्शित करना है या नहीं"
type: docs
weight: 30
url: /hi/net/aspose.tasks/usageview/displaydetailsheadercolumn/
---
## UsageView.DisplayDetailsHeaderColumn property

व्यू में विवरण हेडर कॉलम दिखाना है या नहीं, यह दर्शाने वाला मान प्राप्त करता है या सेट करता है।

```csharp
public bool DisplayDetailsHeaderColumn { get; set; }
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

* class [UsageView](../)
* namespace [Aspose.Tasks](../../usageview/)
* assembly [Aspose.Tasks](../../../)


