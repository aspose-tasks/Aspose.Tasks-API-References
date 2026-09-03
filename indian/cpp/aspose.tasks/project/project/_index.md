---
title: "Aspose::Tasks::Project::Project निर्माता"
linktitle: "प्रोजेक्ट"
articleTitle: "प्रोजेक्ट"
second_title: "Aspose.Tasks C++ के लिए"
description: "Project क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।"
type: docs
weight: 10
url: /hi/cpp/aspose.tasks/project/project/
---

## Project (1 of 13) {#project_1}

Project क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।

**Returns:** Aspose::Tasks::

```cpp
Project()
```

---

## Project (2 of 13) {#project_2}

पासवर्ड-संरक्षित टेम्पलेट (मौजूदा mpp या mpt फ़ाइल) से Project क्लास का नया उदाहरण आरंभ करता है।

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate, const System::String & protectionPassword)
```

| पैरामीटर | विवरण |
| --- | --- |
| projectTemplate | प्रोजेक्ट बनाने के लिए टेम्पलेट का पथ। |
| protectionPassword | सुरक्षा पासवर्ड। |

---

## Project (3 of 13) {#project_3}

टेम्पलेट (मौजूदा mpp या mpt फ़ाइल) से Project क्लास का नया उदाहरण आरंभ करता है।

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate)
```

| पैरामीटर | विवरण |
| --- | --- |
| projectTemplate | प्रोजेक्ट बनाने के लिए टेम्पलेट का पथ। |

---

## Project (4 of 13) {#project_4}

निर्दिष्ट PrimaveraReadOptions क्लास के उदाहरण के साथ Stream से Project क्लास का नया उदाहरण आरंभ करता है।

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream, const System::SharedPtr< PrimaveraReadOptions > & options)
```

| पैरामीटर | विवरण |
| --- | --- |
| stream | Project System::IO::Stream क्लास की Stream |
| options | PrimaveraReadOptions क्लास का निर्दिष्ट उदाहरण जो Primavera फ़ॉर्मेट (XER या XML) के पढ़ने को अनुकूलित करने की अनुमति देता है। |

---

## Project (5 of 13) {#project_5}

टेम्पलेट (मौजूदा mpp या mpt फ़ाइल) से Project क्लास का नया उदाहरण आरंभ करता है।

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate, ParseErrorCallback parseErrorHandler)
```

| पैरामीटर | विवरण |
| --- | --- |
| projectTemplate | प्रोजेक्ट बनाने के लिए टेम्पलेट का पथ। |
| parseErrorHandler | XML पार्स त्रुटियों को संभालने के लिए निर्दिष्ट कॉलबैक विधि। |

---

## Project (6 of 13) {#project_6}

Stream से Project क्लास का नया उदाहरण आरंभ करता है।

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream)
```

| पैरामीटर | विवरण |
| --- | --- |
| stream | टेम्पलेट लोड करने के लिए Stream। |

---

## Project (7 of 13) {#project_7}

StreamReader उदाहरण से Project क्लास का नया उदाहरण आरंभ करता है।

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::StreamReader > & reader)
```

| पैरामीटर | विवरण |
| --- | --- |
| reader | टेम्पलेट लोड करने के लिए स्ट्रीम रीडर। |

---

## Project (8 of 13) {#project_8}

एक टेम्पलेट (मौजूदा MPP या MPT फ़ाइल) से Project क्लास का नया इंस्टेंस प्रारंभ करता है, जिसमें निर्दिष्ट PrimaveraReadOptions क्लास का इंस्टेंस होता है।

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate, const System::SharedPtr< PrimaveraReadOptions > & options)
```

| पैरामीटर | विवरण |
| --- | --- |
| projectTemplate | प्रोजेक्ट बनाने के लिए टेम्पलेट का पथ |
| options | PrimaveraReadOptions क्लास का निर्दिष्ट इंस्टेंस। |

---

## Project (9 of 13) {#project_9}

डेटाबेस से डेटा पढ़ने के लिए Project क्लास का नया इंस्टेंस प्रारंभ करता है, जो DbSettings क्लास के इंस्टेंस द्वारा निर्दिष्ट है।

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< Connectivity::DbSettings > & settings)
```

| पैरामीटर | विवरण |
| --- | --- |
| सेटिंग्स | DbSettings क्लास का निर्दिष्ट इंस्टेंस। |

---

## Project (10 of 13) {#project_10}

एक टेम्पलेट (मौजूदा mpp या mpt फ़ाइल) से Project क्लास का नया इंस्टेंस प्रारंभ करता है।

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream, ParseErrorCallback parseErrorHandler)
```

| पैरामीटर | विवरण |
| --- | --- |
| stream | टेम्पलेट लोड करने के लिए Stream। |
| parseErrorHandler | XML पार्स त्रुटियों को संभालने के लिए निर्दिष्ट कॉलबैक विधि। |

---

## Project (11 of 13) {#project_11}

एक टेम्पलेट (मौजूदा mpp या mpt फ़ाइल) से Project क्लास का नया इंस्टेंस प्रारंभ करता है।

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream, const System::String & protectionPassword)
```

| पैरामीटर | विवरण |
| --- | --- |
| stream | टेम्पलेट लोड करने के लिए Stream। |
| protectionPassword | सुरक्षा पासवर्ड। |

---

## Project (12 of 13) {#project_12}

एक टेम्पलेट (मौजूदा mpp या mpt फ़ाइल) से Project क्लास का नया इंस्टेंस प्रारंभ करता है, जिसमें निर्दिष्ट LoadOptions क्लास का इंस्टेंस होता है।

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate, const System::SharedPtr< LoadOptions > & options)
```

| पैरामीटर | विवरण |
| --- | --- |
| projectTemplate | प्रोजेक्ट बनाने के लिए टेम्पलेट का पथ |
| options | LoadOptions क्लास का निर्दिष्ट इंस्टेंस। |

---

## Project (13 of 13) {#project_13}

स्ट्रीम से Project क्लास का नया इंस्टेंस प्रारंभ करता है, जिसमें निर्दिष्ट LoadOptions क्लास का इंस्टेंस होता है।

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream, const System::SharedPtr< LoadOptions > & options)
```

| पैरामीटर | विवरण |
| --- | --- |
| stream | Project System::IO::Stream क्लास की Stream |
| options | LoadOptions क्लास का निर्दिष्ट इंस्टेंस |

