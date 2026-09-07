---
title: "UsageView.DisplayShortDetailHeaderNames"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "UsageView property. एक मान प्राप्त या सेट करता है जो यह दर्शाता है कि छोटे विवरण हेडर नाम दिखाए जाएँ या नहीं"
type: docs
weight: 40
url: /hi/net/aspose.tasks/usageview/displayshortdetailheadernames/
---
## UsageView.DisplayShortDetailHeaderNames property

छोटे विवरण हेडर नामों को प्रदर्शित करने के लिए मान प्राप्त करता है या सेट करता है।

```csharp
public bool DisplayShortDetailHeaderNames { get; set; }
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


