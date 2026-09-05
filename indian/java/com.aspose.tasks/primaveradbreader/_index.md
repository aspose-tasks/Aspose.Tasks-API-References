---
title: "PrimaveraDbReader"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "Primavera DB से प्रोजेक्ट जानकारी पढ़ने के लिए रीडर का प्रतिनिधित्व करता है।"
type: docs
weight: 200
url: /hi/java/com.aspose.tasks/primaveradbreader/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.PrimaveraBaseReader](../../com.aspose.tasks/primaverabasereader)
```
public final class PrimaveraDbReader extends PrimaveraBaseReader
```

Primavera DB से प्रोजेक्ट जानकारी पढ़ने के लिए रीडर का प्रतिनिधित्व करता है।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [PrimaveraDbReader(PrimaveraDbSettings dbSettings)](#PrimaveraDbReader-com.aspose.tasks.PrimaveraDbSettings-) | एक नया उदाहरण प्रारंभ करता है [PrimaveraXerReader](../../com.aspose.tasks/primaveraxerreader) क्लास का। |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [loadProject(int projectUid)](#loadProject-int-) | निर्दिष्ट अद्वितीय पहचानकर्ता के साथ प्रोजेक्ट लोड करता है। |
### PrimaveraDbReader(PrimaveraDbSettings dbSettings) {#PrimaveraDbReader-com.aspose.tasks.PrimaveraDbSettings-}
```
public PrimaveraDbReader(PrimaveraDbSettings dbSettings)
```


एक नया उदाहरण प्रारंभ करता है [PrimaveraXerReader](../../com.aspose.tasks/primaveraxerreader) क्लास का।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| dbSettings | [PrimaveraDbSettings](../../com.aspose.tasks/primaveradbsettings) | सेटिंग्स जो निर्धारित करती हैं कि Primavera DB से कैसे कनेक्ट किया जाए। |

### loadProject(int projectUid) {#loadProject-int-}
```
public Project loadProject(int projectUid)
```


निर्दिष्ट अद्वितीय पहचानकर्ता के साथ प्रोजेक्ट लोड करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| projectUid | int | लोड करने के लिए प्रोजेक्ट का अद्वितीय पहचानकर्ता। |

**Returns:**
[Project](../../com.aspose.tasks/project) - Project with specified unique identifier read from Primavera DB. Null if project doesn't exist.
