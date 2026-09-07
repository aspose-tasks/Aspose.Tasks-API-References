---
title: "एनम ConstraintType"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.ConstraintType एनम। कार्य की प्रारंभ या समाप्ति तिथि पर प्रतिबंध निर्दिष्ट करता है।"
type: docs
weight: 330
url: /hi/net/aspose.tasks/constrainttype/
---
## ConstraintType enumeration

कार्य की प्रारंभ या समाप्ति तिथि पर बाधा को निर्दिष्ट करता है।

```csharp
public enum ConstraintType
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| Undefined | `-1` | मूल प्रोजेक्ट फ़ाइल में मान परिभाषित नहीं था। |
| AsSoonAsPossible | `0` | [`Start`](../tsk/start/) और [`Finish`](../tsk/finish/) तिथियां [`Task`](../task/) की माता-पिता [`Start`](../tsk/start/) और [`Finish`](../tsk/finish/) तिथियों के सापेक्ष ASAP निर्धारित की गई हैं और [`TaskLinks`](../project/tasklinks/) को ध्यान में रखते हुए। |
| AsLateAsPossible | `1` | [`Start`](../tsk/start/) और [`Finish`](../tsk/finish/) की तिथियां [`Task`](../task/) की ALAP के अनुसार निर्धारित हैं, जो पैरेंट [`Start`](../tsk/start/) और [`Finish`](../tsk/finish/) तिथियों के सापेक्ष हैं और [`TaskLinks`](../project/tasklinks/) को ध्यान में रखते हैं। |
| MustStartOn | `2` | शुरू होना आवश्यक है |
| MustFinishOn | `3` | समाप्त होना आवश्यक है |
| StartNoEarlierThan | `4` | शुरू नहीं हो सकता इससे पहले |
| StartNoLaterThan | `5` | शुरू नहीं हो सकता इससे बाद में |
| FinishNoEarlierThan | `6` | समाप्त नहीं हो सकता इससे पहले |
| FinishNoLaterThan | `7` | समाप्त नहीं हो सकता इससे बाद में |

## टिप्पणियाँ

XML में निर्यात करते समय अपरिभाषित मानों को परिणामी XML से हटा दिया जाएगा।

## उदाहरण

दिखाता है कि कैसे बाधा &lt;see cref=\"Aspose.Tasks.ConstraintType\" /&gt; ConstraintType.AsSoonAsPossible बाधा को एक कार्य के लिए सेट किया जाए।

```csharp
var project = new Project(DataDir + "Constraints/ConstraintAsLateAsPossible.mpp");

// कार्य जिसका Id 11 है, उसके लिए बाधा As Soon As Possible सेट करें
var task = project.RootTask.Children.GetById(11);
task.Set(Tsk.ConstraintType, ConstraintType.AsSoonAsPossible);

SaveOptions options = new PdfSaveOptions();
options.StartDate = project.Get(Prj.StartDate);
options.Timescale = Timescale.ThirdsOfMonths;
project.Save(OutDir + "AsSoonAsPossible_out.pdf", options);
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


