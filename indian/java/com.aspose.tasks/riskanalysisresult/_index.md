---
title: "RiskAnalysisResult"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "जोखिम विश्लेषण के परिणाम का प्रतिनिधित्व करता है।"
type: docs
weight: 262
url: /hi/java/com.aspose.tasks/riskanalysisresult/
---

**Inheritance:**
java.lang.Object
```
public class RiskAnalysisResult
```

जोखिम विश्लेषण के परिणाम का प्रतिनिधित्व करता है।
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [getRiskItems(int itemType)](#getRiskItems-int-) | निर्दिष्ट जोखिम प्रकार के लिए [RiskItemStatisticsCollection](../../com.aspose.tasks/riskitemstatisticscollection) का एक उदाहरण लौटाता है। |
| [saveReport(InputStream stream)](#saveReport-java.io.InputStream-) | जोखिम विश्लेषण रिपोर्ट को PDF प्रारूप में स्ट्रीम पर सहेजता है। |
| [saveReport(String fileName)](#saveReport-java.lang.String-) | जोखिम विश्लेषण रिपोर्ट को निर्दिष्ट फ़ाइल पथ पर PDF प्रारूप में सहेजता है। |
### getRiskItems(int itemType) {#getRiskItems-int-}
```
public final RiskItemStatisticsCollection getRiskItems(int itemType)
```


निर्दिष्ट जोखिम प्रकार के लिए [RiskItemStatisticsCollection](../../com.aspose.tasks/riskitemstatisticscollection) का एक उदाहरण लौटाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| itemType | int | निर्दिष्ट जोखिम प्रकार; यह [RiskItemType](../../com.aspose.tasks/riskitemtype) enumeration के मानों में से एक हो सकता है। |

**Returns:**
[RiskItemStatisticsCollection](../../com.aspose.tasks/riskitemstatisticscollection) - an instance of the [RiskItemStatisticsCollection](../../com.aspose.tasks/riskitemstatisticscollection) for the specified risk type.
### saveReport(InputStream stream) {#saveReport-java.io.InputStream-}
```
public final void saveReport(InputStream stream)
```


जोखिम विश्लेषण रिपोर्ट को PDF प्रारूप में स्ट्रीम पर सहेजता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| stream | java.io.InputStream | जोखिम विश्लेषण रिपोर्ट को सहेजने के लिए स्ट्रीम। |

### saveReport(String fileName) {#saveReport-java.lang.String-}
```
public final void saveReport(String fileName)
```


जोखिम विश्लेषण रिपोर्ट को निर्दिष्ट फ़ाइल पथ पर PDF प्रारूप में सहेजता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| fileName | java.lang.String | निर्दिष्ट फ़ाइल नाम। |

