---
title: "Enum DateFormat"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.DateFormat enum. तिथि प्रारूप को निर्दिष्ट करता है।"
type: docs
weight: 430
url: /hi/net/aspose.tasks/dateformat/
---
## DateFormat enumeration

तारीख प्रारूप को निर्दिष्ट करता है।

```csharp
public enum DateFormat
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| DateMmDdYyHhMmAM | `0` | उदाहरण: 09/30/02 13:00 PM |
| DateMmDdYy | `1` | उदाहरण: 9/30/02 |
| DateMmmmDdYyyyHhMmAM | `2` | उदाहरण: September 30, 2002 13:00 PM |
| DateMmmmDdYyyy | `3` | उदाहरण: September 30, 2002 |
| DateMmmDdHhMmAM | `4` | उदाहरण: Sep 30 13:00 PM |
| DateMmmDdYyy | `5` | उदाहरण: Sep 30, '02 |
| DateMmmmDd | `6` | उदाहरण: September 30 |
| DateMmmDd | `7` | उदाहरण: Sep 30 |
| DateDddMmDdYyHhMmAM | `8` | उदाहरण: Tue 9/30/02 13:00 PM |
| DateDddMmDdYy | `9` | उदाहरण: Tue 9/30/02 |
| DateDddMmmDdYyy | `10` | उदाहरण: Tue Sep 30, '02 |
| DateDddHhMmAM | `11` | उदाहरण: Tue 13:00 PM |
| DateMmDd | `12` | उदाहरण: 9/30 |
| DateDd | `13` | उदाहरण: 30 |
| DateHhMmAm | `14` | उदाहरण: 13:00 PM |
| DateDddMmmDd | `15` | उदाहरण: Tue Sep 30 |
| DateDddMmDd | `16` | उदाहरण: Tue 9/30 |
| DateDddDd | `17` | उदाहरण: Tue 30 |
| DateWwwDd | `18` | उदाहरण: W41/2 |
| DateWwwDdYyHhMmAm | `19` | उदाहरण: W41/2/02 13:00 PM |
| DateMmDdYyyy | `20` | उदाहरण: 9/30/2002 |
| Custom | `21` | DateTime मानों को फ़ॉर्मेट स्ट्रिंग का उपयोग करके स्वरूपित किया जाता है जो प्रोजेक्ट की [`CustomDateFormat`](../prj/customdateformat/) प्रॉपर्टी पर सेट है। |
| DateDdMmYyyy | `256` | उदाहरण: 19/07/2016 |
| Default | `255` | उदाहरण: डिफ़ॉल्ट तिथि प्रारूप। |

## उदाहरण

दिखाता है कि प्रोजेक्ट में सभी तिथियों के फ़ॉर्मेट को निर्यात करने के लिए कैसे अनुकूलित किया जाए।

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
project.Set(Prj.StartDate, new DateTime(2014, 9, 22));

// डिफ़ॉल्ट रूप से project.DateFormat == DateFormat.Date_ddd_mm_dd_yy (Mon 09/22/14) DateFormat को अनुकूलित करें (September 22, 2014)
project.Set(Prj.DateFormat, DateFormat.DateMmmmDdYyyy);
project.Save(OutDir + "CustomizeDateFormats1_out.pdf", SaveFileFormat.Pdf);

// 19/07/2016 तिथि प्रारूप में निर्यात करें
project.Set(Prj.DateFormat, DateFormat.DateDdMmYyyy);
project.Save(OutDir + "CustomizeDateFormats2_out.pdf", SaveFileFormat.Pdf);
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


