---
title: "TaskCollection"
second_title: "Aspose.Tasks Python के लिए .NET API संदर्भ"
description: 
type: docs
weight: 1140
url: /hi/python-net/aspose.tasks/taskcollection/
---

## TaskCollection class

एक संग्रह में [Task](/tasks/python-net/aspose.tasks/task/) वस्तुओं को दर्शाता है।

TaskCollection प्रकार निम्नलिखित सदस्य उजागर करता है:
## गुणधर्म
| नाम | विवरण |
| :- | :- |
| parent_project | TaskCollection ऑब्जेक्ट के पैरेंट प्रोजेक्ट को प्राप्त करता है। |
## Methods
| नाम | विवरण |
| :- | :- |
| add() | निर्दिष्ट कार्य को [TaskCollection](/tasks/python-net/aspose.tasks/taskcollection/) क्लास के इंस्टेंस में जोड़ें।<br/>            यदि ParentProject.CalculationMode None है तो उपयोगकर्ता को इस मेथड के उपयोग के बाद Project.Recalculate() को कॉल करना चाहिए (यह सभी प्रोजेक्ट कार्यों को पुनः शेड्यूल करेगा (शुरू/समाप्ति तिथियां, प्रारंभिक/अंतिम तिथियां सेट करेगा) और स्लैक, कार्य और लागत फ़ील्ड, आईडी और आउटलाइन लेवल जैसे निर्भर फ़ील्ड की गणना करेगा)।<br/>            यदि ParentProject.CalculationMode Manual है तो मेथड केवल कार्य आईडी, आउटलाइन लेवल और आउटलाइन नंबर स्वचालित रूप से गणना करेगा।<br/>            यदि ParentProject.CalculationMode Automatic है तो मेथड सभी प्रोजेक्ट के कार्यों को स्वचालित रूप से पुनः शेड्यूल करेगा<br/>            (शुरू/समाप्ति तिथियां, प्रारंभिक/अंतिम तिथियां सेट करेगा, स्लैक, कार्य और लागत फ़ील्ड की गणना करेगा, आईडी और आउटलाइन लेवल को पुनः गणना करेगा)। |
| add(task_name) | बच्चों के कार्य संग्रह में एक नया कार्य जोड़ता है। |
| add(task_name, before_task_id) |  |
| add(parameters) | निर्दिष्ट आईडी वाले कार्य से पहले और समान आउटलाइन लेवल पर एक नया कार्य सम्मिलित करता है। |
| to_list() | TaskCollection ऑब्जेक्ट को [Task](/tasks/python-net/aspose.tasks/task/) ऑब्जेक्ट्स की सूची में परिवर्तित करता है। |
| get_by_uid(uid) | इस संग्रह के पैरेंट टास्क के पूर्वज वाले निर्दिष्ट Uid के साथ एक कार्य लौटाता है। |
| get_by_id(id) | इस संग्रह के पैरेंट टास्क के पूर्वज वाले निर्दिष्ट Id के साथ एक कार्य लौटाता है। |

### संबंधित देखें

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

