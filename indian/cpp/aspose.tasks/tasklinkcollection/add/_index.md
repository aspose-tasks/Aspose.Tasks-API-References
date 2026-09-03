---
title: "Aspose::Tasks::TaskLinkCollection::Add मेथड"
linktitle: "जोड़ें"
articleTitle: "जोड़ें"
second_title: "Aspose.Tasks C++ के लिए"
description: "Finish-Start TaskLink की एक इंस्टेंस लौटाता है जिसे TaskLinkCollection ऑब्जेक्ट में जोड़ा गया है।"
type: docs
weight: 10
url: /hi/cpp/aspose.tasks/tasklinkcollection/add/
---

## Add (1 of 4) {#add_1}

Finish-Start TaskLink की एक इंस्टेंस लौटाता है जिसे TaskLinkCollection ऑब्जेक्ट में जोड़ा गया है।

**Returns:** a task link instance which has been added to this object.

```cpp
Add(const System::SharedPtr< Task > & pred, const System::SharedPtr< Task > & succ)
```

| पैरामीटर | विवरण |
| --- | --- |
| pred | पूर्ववर्ती कार्य। |
| succ | उत्तराधिकारी कार्य। |

---

## Add (2 of 4) {#add_2}

TaskLink का एक उदाहरण लौटाता है जिसे TaskLinkCollection ऑब्जेक्ट में जोड़ा गया है।

**Returns:** a task link instance which has been added to this object.

```cpp
Add(const System::SharedPtr< Task > & pred, const System::SharedPtr< Task > & succ, TaskLinkType linkType)
```

| पैरामीटर | विवरण |
| --- | --- |
| pred | पूर्ववर्ती कार्य। |
| succ | उत्तराधिकारी कार्य। |
| linkType | लिंक प्रकार TaskLinkType |

---

## Add (3 of 4) {#add_3}

TaskLink का एक उदाहरण लौटाता है जिसे TaskLinkCollection ऑब्जेक्ट में जोड़ा गया है।

**Returns:** a task link which has been added to this object.

```cpp
Add(const System::SharedPtr< Task > & pred, const System::SharedPtr< Task > & succ, TaskLinkType linkType, Duration lag)
```

| पैरामीटर | विवरण |
| --- | --- |
| pred | पूर्ववर्ती कार्य। |
| succ | उत्तराधिकारी कार्य। |
| linkType | लिंक प्रकार TaskLinkType |
| lag | लिंक लैग अवधि। |

---

## Add (4 of 4) {#add_4}

यह ICollection की Add मेथड की स्टब इम्प्लीमेंटेशन है, जो केवल NotSupportedException को थ्रो करती है।

**Returns:** void Aspose::Tasks::

```cpp
Add(const System::SharedPtr< TaskLink > & item)
```

| पैरामीटर | विवरण |
| --- | --- |
| वस्तु | जोड़ने के लिए आइटम। |

