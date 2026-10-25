---
title: "Aspose::Tasks::TaskCollection::Add विधि"
linktitle: "जोड़ें"
articleTitle: "जोड़ें"
second_title: "Aspose.Tasks C++ के लिए"
description: "पिछले टास्क के समान आउटलाइन स्तर पर प्रोजेक्ट टास्क संग्रह में नया टास्क जोड़ता है।"
type: docs
weight: 10
url: /hi/cpp/aspose.tasks/taskcollection/add/
---

## Add (1 of 5) {#add_1}

पिछले टास्क के समान आउटलाइन स्तर पर प्रोजेक्ट टास्क संग्रह में नया टास्क जोड़ता है।

**Returns:** returns the newly added instance of the Task class.

```cpp
Add()
```

---

## Add (2 of 5) {#add_2}

निर्दिष्ट आईडी वाले कार्य से पहले और समान रूपरेखा स्तर पर एक नया कार्य इन्सर्ट करता है।

**Returns:** returns the newly added instance of the Task class.

```cpp
Add(const System::SharedPtr< RecurringTaskParameters > & parameters)
```

| पैरामीटर | विवरण |
| --- | --- |
| पैरामीटर | आवर्ती कार्य के निर्माण के लिए निर्दिष्ट पैरामीटर। |

---

## Add (3 of 5) {#add_3}

निर्दिष्ट कार्य को TaskCollection क्लास के इंस्टेंस में जोड़ें। यदि ParentProject.CalculationMode None है तो उपयोगकर्ता को इस विधि का उपयोग करने के बाद Project.Recalculate() को कॉल करना चाहिए (यह सभी प्रोजेक्ट कार्यों को पुनः निर्धारित करेगा (शुरू/समाप्ति तिथियां, प्रारंभिक/अंतिम तिथियां सेट करेगा) और स्लैक, कार्य और लागत फ़ील्ड, आईडी और रूपरेखा स्तर जैसे आश्रित फ़ील्ड की गणना करेगा)। यदि ParentProject.CalculationMode Manual है तो यह विधि केवल कार्य आईडी, रूपरेखा स्तर और रूपरेखा संख्याओं की स्वचालित रूप से गणना करेगी। यदि ParentProject.CalculationMode Automatic है तो यह विधि सभी प्रोजेक्ट कार्यों को स्वचालित रूप से पुनः निर्धारित करेगी (शुरू/समाप्ति तिथियां, प्रारंभिक/अंतिम तिथियां सेट करेगी, स्लैक, कार्य और लागत फ़ील्ड की गणना करेगी, आईडी और रूपरेखा स्तर को पुनः गणना करेगी)।

**Returns:** void Aspose::Tasks::

```cpp
Add(const System::SharedPtr< Task > & item)
```

| पैरामीटर | विवरण |
| --- | --- |
| वस्तु | निर्दिष्ट कार्य जिसे इस कार्य संग्रह में जोड़ा जाना चाहिए. |

---

## Add (4 of 5) {#add_4}

बच्चों के कार्य संग्रह में एक नया कार्य जोड़ता है.

**Returns:** returns the newly added instance of the Task class.

```cpp
Add(const System::String & taskName)
```

| पैरामीटर | विवरण |
| --- | --- |
| taskName | निर्दिष्ट कार्य नाम. |

---

## Add (5 of 5) {#add_5}

बच्चों के कार्य संग्रह में एक नया आवर्ती कार्य जोड़ता है.

**Returns:** returns a task which was inserted before a task with the specified id.

```cpp
Add(const System::String & taskName, int32_t beforeTaskId)
```

| पैरामीटर | विवरण |
| --- | --- |
| taskName | निर्दिष्ट कार्य नाम. |
| beforeTaskId | निर्दिष्ट आईडी जो एक कार्य का है, जिसके पहले एक नया कार्य डाला जाएगा. |

