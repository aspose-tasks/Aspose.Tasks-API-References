---
title: "Aspose::Tasks::ICalendar::GetWorkingHours विधि"
linktitle: "GetWorkingHours"
articleTitle: "GetWorkingHours"
second_title: "Aspose.Tasks C++ के लिए"
description: "निर्दिष्ट तिथि पर कार्य घंटे की मात्रा लौटाता है।"
type: docs
weight: 60
url: /hi/cpp/aspose.tasks/icalendar/getworkinghours/
---

## GetWorkingHours (1 of 2) {#getworkinghours_1}

निर्दिष्ट तिथि पर कार्य घंटे की मात्रा लौटाता है।

**Returns:** Working hours at the specified date.

```cpp
GetWorkingHours(System::DateTime dt)
```

| पैरामीटर | विवरण |
| --- | --- |
| dt | कार्य समय प्राप्त करने के लिए तिथि। |

---

## GetWorkingHours (2 of 2) {#getworkinghours_2}

निर्दिष्ट तिथि समय अंतराल के लिए कार्य समय की शुरुआत, समाप्ति और अवधि के साथ WorkUnit लौटाता है।

**Returns:** Instance of WorkUnit class containing Start, Finish and Duration of working hours.

```cpp
GetWorkingHours(System::DateTime start, System::DateTime finish)
```

| पैरामीटर | विवरण |
| --- | --- |
| शुरू | अंतराल की प्रारंभ तिथि। |
| समाप्ति | अंतराल की समाप्ति तिथि। |

