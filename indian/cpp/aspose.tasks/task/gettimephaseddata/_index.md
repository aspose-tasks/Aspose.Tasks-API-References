---
title: "Aspose::Tasks::Task::GetTimephasedData विधि"
linktitle: "GetTimephasedData"
articleTitle: "GetTimephasedData"
second_title: "Aspose.Tasks C++ के लिए"
description: "दिए गए प्रारंभ और समाप्ति तिथियों के भीतर TimephasedData मानों के साथ TimephasedDataCollection ऑब्जेक्ट लौटाता है।"
type: docs
weight: 1360
url: /hi/cpp/aspose.tasks/task/gettimephaseddata/
---

## GetTimephasedData (1 of 2) {#gettimephaseddata_1}

दिए गए प्रारंभ और समाप्ति तिथियों के भीतर TimephasedData मानों के साथ TimephasedDataCollection ऑब्जेक्ट लौटाता है।

**Returns:** List of Aspose::Tasks::TimephasedData to be filled in.

```cpp
GetTimephasedData(System::DateTime start, System::DateTime end)
```

| पैरामीटर | विवरण |
| --- | --- |
| शुरू | समय‑फ़ेज़्ड डेटा के लिए प्रारंभ तिथि। |
| end | समय-फ़ेज़्ड डेटा की समाप्ति तिथि। |

---

## GetTimephasedData (2 of 2) {#gettimephaseddata_2}

निर्दिष्ट समय-फ़ेज़्ड डेटा प्रकार की दी गई प्रारंभ और समाप्ति तिथियों के भीतर TimephasedData मानों के साथ TimephasedDataCollection ऑब्जेक्ट लौटाता है।

**Returns:** A TimephasedDataCollection object with TimephasedData values within given start and end dates of specified timephased data type.

```cpp
GetTimephasedData(System::DateTime start, System::DateTime end, TimephasedDataType timephasedType)
```

| पैरामीटर | विवरण |
| --- | --- |
| शुरू | समय‑फ़ेज़्ड डेटा के लिए प्रारंभ तिथि। |
| end | समय-फ़ेज़्ड डेटा की समाप्ति तिथि। |
| timephasedType | समय-फ़ेज़्ड डेटा का प्रकार ( Aspose::Tasks::TimephasedDataType ). |

