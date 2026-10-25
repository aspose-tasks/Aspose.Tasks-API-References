---
title: "Task.MoveToSibling"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Task मेथड। वर्तमान कार्य को उसी Outline Level पर निर्दिष्ट कार्य से पहले ले जाता है। यदि ParentProject.CalculationMode None है तो उपयोगकर्ता को इस मेथड का उपयोग करने के बाद Project.Recalculate को कॉल करना चाहिए। यह सभी प्रोजेक्ट कार्यों की शुरू/समाप्ति तिथियों को पुनः निर्धारित करेगा, प्रारंभिक/विलंबित तिथियों को सेट करेगा और स्लैक, कार्य और लागत फ़ील्ड जैसे निर्भर फ़ील्ड की गणना करेगा। यदि ParentProject.CalculationMode Manual है तो मेथड केवल कार्य की आईडी, Outline Level और Outline Numbers की स्वचालित गणना करेगा। यदि ParentProject.CalculationMode Automatic है तो मेथड सभी प्रोजेक्ट कार्यों की शुरू/समाप्ति तिथियों को स्वचालित रूप से पुनः निर्धारित करेगा, प्रारंभिक/विलंबित तिथियों को सेट करेगा, स्लैक, कार्य और लागत फ़ील्ड की गणना करेगा, आईडी और Outline Levels को पुनः गणना करेगा।"
type: docs
weight: 1370
url: /hi/net/aspose.tasks/task/movetosibling/
---
## MoveToSibling(Task) {#movetosibling}

वर्तमान कार्य को उसी रूपरेखा स्तर पर निर्दिष्ट कार्य से पहले ले जाता है। यदि ParentProject.CalculationMode None है तो उपयोगकर्ता को इस विधि का उपयोग करने के बाद Project.Recalculate() को बुलाना चाहिए (यह सभी प्रोजेक्ट कार्यों को (प्रारंभ/समाप्ति तिथियों, प्रारंभिक/विलंबित तिथियों को सेट करता है) पुनः‑निर्धारित करेगा और स्लैक, कार्य और लागत फ़ील्ड, रूपरेखा स्तर जैसी निर्भर फ़ील्डों की गणना करेगा)। यदि ParentProject.CalculationMode Manual है तो यह विधि केवल कार्य Id, रूपरेखा स्तर और रूपरेखा संख्याओं की स्वचालित रूप से गणना करेगी। यदि ParentProject.CalculationMode Automatic है तो यह विधि सभी प्रोजेक्ट कार्यों को स्वचालित रूप से पुनः‑निर्धारित करेगी (प्रारंभ/समाप्ति तिथियों, प्रारंभिक/विलंबित तिथियों को सेट करती है, स्लैक, कार्य और लागत फ़ील्डों की गणना करती है, Ids और रूपरेखा स्तरों को पुनः‑गणना करती है)।

```csharp
public void MoveToSibling(Task beforeTask)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| beforeTask | कार्य | वह Task जिसके पहले वर्तमान कार्य सम्मिलित किया जाएगा। |

## उदाहरण

दिखाता है कि समान पैरेंट के तहत कार्य को कैसे ले जाएँ।

```csharp
var project = new Project(DataDir + "MoveTask.mpp");

// आईडी 5 वाले कार्यों को आईडी 3 वाले कार्य से पहले ले जाएँ
var task = project.RootTask.Children.GetById(5);

var targetTask = project.RootTask.Children.First(t => t.Get(Tsk.Name) == "Task4");
task.MoveToSibling(targetTask);

// या
// कार्य को संग्रह के अंत में ले जाएँ
// task.MoveToSibling(null);
project.Save(OutDir + "MoveTaskUnderSameParent_out.mpp", SaveFileFormat.Mpp);
```

### संबंधित देखें

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)

---

## MoveToSibling(int) {#movetosibling_1}

वर्तमान कार्य को उसी रूपरेखा स्तर पर निर्दिष्ट Id वाले कार्य से पहले ले जाता है। यदि ParentProject.CalculationMode None है तो उपयोगकर्ता को इस विधि का उपयोग करने के बाद Project.Recalculate() को बुलाना चाहिए (यह सभी प्रोजेक्ट कार्यों को (प्रारंभ/समाप्ति तिथियों, प्रारंभिक/विलंबित तिथियों को सेट करता है) पुनः‑निर्धारित करेगा और स्लैक, कार्य और लागत फ़ील्ड, रूपरेखा स्तर जैसी निर्भर फ़ील्डों की गणना करेगा)। यदि ParentProject.CalculationMode Manual है तो यह विधि केवल कार्य Id, रूपरेखा स्तर और रूपरेखा संख्याओं की स्वचालित रूप से गणना करेगी। यदि ParentProject.CalculationMode Automatic है तो यह विधि सभी प्रोजेक्ट कार्यों को स्वचालित रूप से पुनः‑निर्धारित करेगी (प्रारंभ/समाप्ति तिथियों, प्रारंभिक/विलंबित तिथियों को सेट करती है, स्लैक, कार्य और लागत फ़ील्डों की गणना करती है, Ids और रूपरेखा स्तरों को पुनः‑गणना करती है)।

```csharp
public void MoveToSibling(int beforeTaskId)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| beforeTaskId | Int32 | वर्तमान कार्य के सम्मिलित होने से पहले वाले कार्य की Id ([`Id`](../../tsk/id/)) |

## उदाहरण

दिखाता है कि कार्य की Id का उपयोग करके समान पैरेंट के तहत कार्य को कैसे ले जाएँ।

```csharp
var project = new Project(DataDir + "MoveTask.mpp");

// आईडी 5 वाले कार्यों को आईडी 3 वाले कार्य से पहले ले जाएँ
var task = project.RootTask.Children.GetById(5);

task.MoveToSibling(3);

// या
// कार्य को संग्रह के अंत में ले जाएँ
// task.MoveToSibling(-1);
project.Save(OutDir + "MoveTaskUnderSameParent_out.mpp", SaveFileFormat.Mpp);
```

### संबंधित देखें

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


