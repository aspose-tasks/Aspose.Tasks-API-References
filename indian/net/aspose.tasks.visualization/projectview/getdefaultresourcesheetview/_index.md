---
title: "ProjectView.GetDefaultResourceSheetView"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ProjectView मेथड। इसमें Uid, रिसोर्स नाम, प्रकार, सामग्री, लेबल, आद्याक्षर, समूह, अधिकतम यूनिट, मानक दर, ओवरटाइम दर, उपयोग प्रति लागत, बेस कैलेंडर पर संचित, और कोड रिसोर्स कॉलम शामिल हैं"
type: docs
weight: 40
url: /hi/net/aspose.tasks.visualization/projectview/getdefaultresourcesheetview/
---
## ProjectView.GetDefaultResourceSheetView method

Uid, संसाधन नाम, प्रकार, सामग्री लेबल, प्रारंभाक्षर, समूह, अधिकतम इकाइयाँ, मानक दर, ओवरटाइम दर, प्रति उपयोग लागत, संचित समय, बेस कैलेंडर और कोड संसाधन कॉलम शामिल करता है।

```csharp
public static ProjectView GetDefaultResourceSheetView()
```

### रिटर्न वैल्यू

एक दृश्य जिसमें [`ResourceViewColumn`](../../resourceviewcolumn/) की सूची शामिल है।

## उदाहरण

दिखाता है कि रिसोर्स शीट दृश्य के साथ प्रोजेक्ट कैसे सहेजें।

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultResourceSheetView()
};

project.Save(OutDir + "WorkWithProjectView_ResourceSheetView_out.pdf", options);
```

### संबंधित देखें

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


