---
title: "Aspose::Tasks::Project::UpdateProjectWorkAsComplete विधि"
linktitle: "UpdateProjectWorkAsComplete"
articleTitle: "UpdateProjectWorkAsComplete"
second_title: "Aspose.Tasks C++ के लिए"
description: "पूरे प्रोजेक्ट के लिए निर्दिष्ट तिथि तक सभी कार्य को पूर्ण के रूप में अपडेट करता है।"
type: docs
weight: 2080
url: /hi/cpp/aspose.tasks/project/updateprojectworkascomplete/
---

## UpdateProjectWorkAsComplete (1 of 2) {#updateprojectworkascomplete_1}

पूरे प्रोजेक्ट के लिए निर्दिष्ट तिथि तक सभी कार्य को पूर्ण के रूप में अपडेट करता है।

**Returns:** void Aspose::Tasks::

```cpp
UpdateProjectWorkAsComplete(System::DateTime completeThrough, bool setZeroOrHundredPercentCompleteOnly)
```

| पैरामीटर | विवरण |
| --- | --- |
| completeThrough | कार्य को पूर्ण के रूप में अपडेट करने की तिथि। |
| setZeroOrHundredPercentCompleteOnly | यदि true पर सेट किया जाता है तो केवल उन कार्यों को 100% पूर्ण के रूप में अपडेट करता है जिनकी समाप्ति तिथि निर्दिष्ट complete-through तिथि से पहले है। अन्यथा, निर्धारित प्रारंभ और complete-through तिथियों के आधार पर पूर्णता प्रतिशत मान की गणना करता है। |

---

## UpdateProjectWorkAsComplete (2 of 2) {#updateprojectworkascomplete_2}

निर्दिष्ट कार्यों की सूची के लिए निर्दिष्ट तिथि तक सभी कार्यों को पूर्ण के रूप में अपडेट करता है।

**Returns:** void Aspose::Tasks::

```cpp
UpdateProjectWorkAsComplete(System::DateTime completeThrough, bool setZeroOrHundredPercentCompleteOnly, const System::SharedPtr< System::Collections::Generic::List< System::SharedPtr< Task >>> & taskCollection)
```

| पैरामीटर | विवरण |
| --- | --- |
| completeThrough | कार्य को पूर्ण के रूप में अपडेट करने की तिथि। |
| setZeroOrHundredPercentCompleteOnly | यदि true पर सेट किया जाता है तो केवल उन कार्यों को 100% पूर्ण के रूप में अपडेट करता है जिनकी समाप्ति तिथि निर्दिष्ट complete-through तिथि से पहले है। अन्यथा, निर्धारित प्रारंभ और complete-through तिथियों के आधार पर पूर्णता प्रतिशत मान की गणना करता है। |
| taskCollection | कार्य को अपडेट करने के लिए कार्यों की List< Task >। |

