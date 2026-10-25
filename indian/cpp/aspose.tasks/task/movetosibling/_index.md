---
title: "Aspose::Tasks::Task::MoveToSibling विधि"
linktitle: "MoveToSibling"
articleTitle: "MoveToSibling"
second_title: "Aspose.Tasks C++ के लिए"
description: "वर्तमान कार्य को समान रूपरेखा स्तर पर निर्दिष्ट कार्य से पहले ले जाता है।"
type: docs
weight: 1370
url: /hi/cpp/aspose.tasks/task/movetosibling/
---

## MoveToSibling (1 of 2) {#movetosibling_1}

वर्तमान कार्य को उसी Outline Level पर निर्दिष्ट कार्य से पहले ले जाता है। यदि ParentProject.CalculationMode None है तो उपयोगकर्ता को इस विधि का उपयोग करने के बाद Project.Recalculate() को बुलाना चाहिए (यह सभी प्रोजेक्ट कार्यों को (प्रारंभ/समाप्ति तिथियों, प्रारंभिक/विलंबित तिथियों को सेट करता है) पुनः समय-सारिणी करेगा और स्लैक, कार्य और लागत फ़ील्ड जैसे निर्भर फ़ील्ड की गणना करेगा, outline levels)। यदि ParentProject.CalculationMode Manual है तो यह विधि केवल कार्य आईडी, outline level और outline numbers को स्वचालित रूप से गणना करेगी। यदि ParentProject.CalculationMode Automatic है तो यह विधि सभी प्रोजेक्ट कार्यों को स्वचालित रूप से पुनः समय-सारिणी करेगी (प्रारंभ/समाप्ति तिथियों, प्रारंभिक/विलंबित तिथियों को सेट करती है, स्लैक, कार्य और लागत फ़ील्ड की गणना करती है, आईडी और outline levels को पुनः गणना करती है)।

**Returns:** void Aspose::Tasks::

```cpp
MoveToSibling(const System::SharedPtr< Task > & beforeTask)
```

| पैरामीटर | विवरण |
| --- | --- |
| beforeTask | कार्य जिसके पहले वर्तमान कार्य सम्मिलित किया जाएगा। |

---

## MoveToSibling (2 of 2) {#movetosibling_2}

वर्तमान कार्य को समान रूपरेखा स्तर पर निर्दिष्ट Id वाले कार्य से पहले ले जाता है। यदि ParentProject.CalculationMode None है तो उपयोगकर्ता को इस विधि का उपयोग करने के बाद Project.Recalculate() को बुलाना चाहिए (यह सभी प्रोजेक्ट कार्यों (प्रारंभ/समाप्ति तिथियों, प्रारंभिक/अंतिम तिथियों को सेट करता है) को पुनः निर्धारित करेगा और स्लैक, कार्य और लागत फ़ील्ड जैसे आश्रित फ़ील्डों की गणना करेगा, रूपरेखा स्तर)। यदि ParentProject.CalculationMode Manual है तो यह विधि केवल कार्य Id, रूपरेखा स्तर और रूपरेखा संख्याओं की स्वचालित रूप से गणना करेगी। यदि ParentProject.CalculationMode Automatic है तो यह विधि सभी प्रोजेक्ट कार्यों को स्वचालित रूप से पुनः निर्धारित करेगी (प्रारंभ/समाप्ति तिथियों, प्रारंभिक/अंतिम तिथियों को सेट करती है, स्लैक, कार्य और लागत फ़ील्डों की गणना करती है, Id और रूपरेखा स्तरों को पुनः गणना करती है)।

**Returns:** void Aspose::Tasks::

```cpp
MoveToSibling(int32_t beforeTaskId)
```

| पैरामीटर | विवरण |
| --- | --- |
| beforeTaskId | Id ( Tsk::Id ) वह कार्य जिसका पहले वर्तमान कार्य सम्मिलित किया जाएगा। |

