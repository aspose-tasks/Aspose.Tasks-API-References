---
title: "RiskAnalyzer"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "निर्दिष्ट जोखिम विश्लेषण सेटिंग्स के आधार पर मोन्टे कार्लो सिमुलेशन करता है।"
type: docs
weight: 264
url: /hi/java/com.aspose.tasks/riskanalyzer/
---

**Inheritance:**
java.lang.Object
```
public class RiskAnalyzer
```

निर्दिष्ट जोखिम विश्लेषण सेटिंग्स के आधार पर मोन्टे कार्लो सिमुलेशन करता है।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [RiskAnalyzer(RiskAnalysisSettings settings)](#RiskAnalyzer-com.aspose.tasks.RiskAnalysisSettings-) | नए [RiskAnalyzer](../../com.aspose/tasks/riskanalyzer) क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है। |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [analyze(Project project)](#analyze-com.aspose.tasks.Project-) | निर्दिष्ट प्रोजेक्ट के लिए जोखिम विश्लेषण करता है। |
| [getSettings()](#getSettings--) | उस [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) क्लास का इंस्टेंस प्राप्त करता है जो जोखिम विश्लेषण के लिए आवश्यक सेटिंग्स को परिभाषित करता है। |
| [setSettings(RiskAnalysisSettings value)](#setSettings-com.aspose.tasks.RiskAnalysisSettings-) | उस [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) क्लास का इंस्टेंस सेट करता है जो जोखिम विश्लेषण के लिए आवश्यक सेटिंग्स को परिभाषित करता है। |
### RiskAnalyzer(RiskAnalysisSettings settings) {#RiskAnalyzer-com.aspose.tasks.RiskAnalysisSettings-}
```
public RiskAnalyzer(RiskAnalysisSettings settings)
```


नए [RiskAnalyzer](../../com.aspose/tasks/riskanalyzer) क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| settings | [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) | निर्दिष्ट [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) क्लास का इंस्टेंस। |

### analyze(Project project) {#analyze-com.aspose.tasks.Project-}
```
public final RiskAnalysisResult analyze(Project project)
```


निर्दिष्ट प्रोजेक्ट के लिए जोखिम विश्लेषण करता है। विश्लेषण मोन्टे कार्लो सिमुलेशन पर आधारित है और परिणाम एक [RiskAnalysisResult](../../com.aspose.tasks/riskanalysisresult) क्लास का इंस्टेंस है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | विश्लेषण के लिए निर्दिष्ट [Project](../../com.aspose.tasks/project) क्लास का इंस्टेंस। |

**Returns:**
[RiskAnalysisResult](../../com.aspose.tasks/riskanalysisresult) - the instance of the [RiskAnalysisResult](../../com.aspose.tasks/riskanalysisresult) which represents a result of the analysis.
### getSettings() {#getSettings--}
```
public final RiskAnalysisSettings getSettings()
```


उस [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) क्लास का इंस्टेंस प्राप्त करता है जो जोखिम विश्लेषण के लिए आवश्यक सेटिंग्स को परिभाषित करता है।

**Returns:**
[RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) - the instance of the [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) class which defines necessary settings for risk analysis.
### setSettings(RiskAnalysisSettings value) {#setSettings-com.aspose.tasks.RiskAnalysisSettings-}
```
public final void setSettings(RiskAnalysisSettings value)
```


उस [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) क्लास का इंस्टेंस सेट करता है जो जोखिम विश्लेषण के लिए आवश्यक सेटिंग्स को परिभाषित करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) | जो [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) क्लास का इंस्टेंस है वह जोखिम विश्लेषण के लिए आवश्यक सेटिंग्स को परिभाषित करता है। |

