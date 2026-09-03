---
title: "Aspose::Tasks::ResourceAssignmentCollection::Add विधि"
linktitle: "जोड़ें"
articleTitle: "जोड़ें"
second_title: "Aspose.Tasks C++ के लिए"
description: "यह ICollection की Add मेथड की स्टब इम्प्लीमेंटेशन है, जो केवल NotSupportedException को थ्रो करती है।"
type: docs
weight: 10
url: /hi/cpp/aspose.tasks/resourceassignmentcollection/add/
---

## Add (1 of 4) {#add_1}

यह ICollection की Add मेथड की स्टब इम्प्लीमेंटेशन है, जो केवल NotSupportedException को थ्रो करती है।

**Returns:** void Aspose::Tasks::

```cpp
Add(const System::SharedPtr< ResourceAssignment > & item)
```

| पैरामीटर | विवरण |
| --- | --- |
| वस्तु | हटाने के लिए आइटम। |

---

## Add (2 of 4) {#add_2}

ResourceAssignmentCollection में नया असाइनमेंट जोड़ता है।

**Returns:** Added assignment.

```cpp
Add(const System::SharedPtr< Task > & task, const System::SharedPtr< Resource > & resource)
```

| पैरामीटर | विवरण |
| --- | --- |
| कार्य | असाइन करने के लिए एक कार्य। |
| संसाधन | असाइन करने के लिए एक संसाधन। |

---

## Add (3 of 4) {#add_3}

ResourceAssignmentCollection में नया असाइनमेंट जोड़ता है।

**Returns:** Added assignment.

```cpp
Add(const System::SharedPtr< Task > & task, const System::SharedPtr< Resource > & resource, double units)
```

| पैरामीटर | विवरण |
| --- | --- |
| कार्य | असाइन करने के लिए एक कार्य। |
| संसाधन | असाइन करने के लिए एक संसाधन। |
| इकाइयाँ | नए असाइनमेंट के लिए इकाइयों की संख्या। |

---

## Add (4 of 4) {#add_4}

ResourceAssignmentCollection में नया असाइनमेंट जोड़ता है।

**Returns:** Added assignment.

```cpp
Add(const System::SharedPtr< Task > & task, const System::SharedPtr< Resource > & resource, System::Decimal cost)
```

| पैरामीटर | विवरण |
| --- | --- |
| कार्य | असाइन करने के लिए एक कार्य। |
| संसाधन | एक लागत संसाधन जिसे असाइन किया जाना है। |
| लागत | नए असाइनमेंट के लिए लागत। |

