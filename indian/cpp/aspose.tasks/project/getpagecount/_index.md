---
title: "Aspose::Tasks::Project::GetPageCount मेथड"
linktitle: "GetPageCount"
articleTitle: "GetPageCount"
second_title: "Aspose.Tasks C++ के लिए"
description: "डिफ़ॉल्ट Timescale (Days) का उपयोग करके रेंडर किए जाने वाले प्रोजेक्ट के पृष्ठ गणना लौटाता है।"
type: docs
weight: 1090
url: /hi/cpp/aspose.tasks/project/getpagecount/
---

## GetPageCount (1 of 7) {#getpagecount_1}

डिफ़ॉल्ट Timescale (Days) का उपयोग करके रेंडर किए जाने वाले प्रोजेक्ट के पृष्ठ गणना लौटाता है।

**Returns:** Page count to be rendered.

```cpp
GetPageCount()
```

---

## GetPageCount (2 of 7) {#getpagecount_2}

दिए गए SaveOptions का उपयोग करके रेंडर किए जाने वाले प्रोजेक्ट के लिए पृष्ठ गिनती लौटाता है।

**Returns:** a page count to be rendered.

```cpp
GetPageCount(const System::SharedPtr< Saving::SaveOptions > & saveOptions)
```

| पैरामीटर | विवरण |
| --- | --- |
| saveOptions | पृष्ठ गिनती प्राप्त करने के लिए सेव विकल्प। |

---

## GetPageCount (3 of 7) {#getpagecount_3}

दिए गए Timescale और PageSize का उपयोग करके रेंडर किए जाने वाले प्रोजेक्ट के पेज काउंट को लौटाता है।

**Returns:** Page count to be rendered.

```cpp
GetPageCount(Visualization::PageSize pageSize, Visualization::Timescale scale)
```

| पैरामीटर | विवरण |
| --- | --- |
| pageSize | पेज काउंट प्राप्त करने के लिए आकार। |
| scale | पेज काउंट प्राप्त करने के लिए स्केल। |

---

## GetPageCount (4 of 7) {#getpagecount_4}

दिए गए Timescale, PresentationFormat और डेट रेंज का उपयोग करके रेंडर किए जाने वाले प्रोजेक्ट के पेज काउंट को लौटाता है।

**Returns:** Page count to be rendered.

```cpp
GetPageCount(Visualization::PageSize pageSize, Visualization::Timescale scale, System::DateTime startDate, System::DateTime endDate)
```

| पैरामीटर | विवरण |
| --- | --- |
| pageSize | पेज काउंट प्राप्त करने के लिए आकार। |
| scale | पेज काउंट प्राप्त करने के लिए स्केल। |
| startDate | पेज काउंट प्राप्त करने के लिए प्रारंभ तिथि। |
| endDate | पेज काउंट प्राप्त करने के लिए समाप्ति तिथि। |

---

## GetPageCount (5 of 7) {#getpagecount_5}

डिफ़ॉल्ट Timescale (Days) और दिए गए PresentationFormat का उपयोग करके रेंडर किए जाने वाले प्रोजेक्ट के पेज काउंट को लौटाता है।

**Returns:** Page count to be rendered.

```cpp
GetPageCount(Visualization::PresentationFormat format)
```

| पैरामीटर | विवरण |
| --- | --- |
| फ़ॉर्मेट | पेज काउंट प्राप्त करने के लिए फ़ॉर्मेट। |

---

## GetPageCount (6 of 7) {#getpagecount_6}

दिए गए Timescale और PresentationFormat का उपयोग करके रेंडर किए जाने वाले प्रोजेक्ट के पेज काउंट को लौटाता है।

**Returns:** a page count to be rendered.

```cpp
GetPageCount(Visualization::PresentationFormat format, Visualization::Timescale scale)
```

| पैरामीटर | विवरण |
| --- | --- |
| फ़ॉर्मेट | पेज काउंट प्राप्त करने के लिए फ़ॉर्मेट। |
| scale | पेज काउंट प्राप्त करने के लिए स्केल। |

---

## GetPageCount (7 of 7) {#getpagecount_7}

दिए गए Timescale का उपयोग करके रेंडर किए जाने वाले प्रोजेक्ट के पेज काउंट को लौटाता है।

**Returns:** Page count to be rendered.

```cpp
GetPageCount(Visualization::Timescale scale)
```

| पैरामीटर | विवरण |
| --- | --- |
| scale | पेज काउंट प्राप्त करने के लिए स्केल। |

