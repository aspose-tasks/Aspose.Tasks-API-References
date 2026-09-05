---
title: "LevelingOrder"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "लेवलिंग क्रम के संभावित मानों को परिभाषित करता है।"
type: docs
weight: 143
url: /hi/java/com.aspose.tasks/levelingorder/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class LevelingOrder extends System.Enum
```

लेवलिंग क्रम के संभावित मानों को परिभाषित करता है।
## फ़ील्ड्स

| फ़ील्ड | विवरण |
| --- | --- |
| [IdOnly](#IdOnly) | कार्य Id आरोही क्रम में विलंबित होते हैं। |
| [PriorityThenStandard](#PriorityThenStandard) | प्राथमिकता को पहले माना जाता है, फिर मानक में समान गुणों को। |
| [Standard](#Standard) | निम्नलिखित गुणों को ध्यान में रखा जाता है: पूर्ववर्ती संबंध, कुल स्लैक (जिस कार्य का कुल स्लैक अधिक हो वह पहले विलंबित होता है), प्रारंभ तिथि, प्राथमिकता। |
### IdOnly {#IdOnly}
```
public static final int IdOnly
```


कार्य Id आरोही क्रम में विलंबित होते हैं।

### PriorityThenStandard {#PriorityThenStandard}
```
public static final int PriorityThenStandard
```


प्राथमिकता को पहले माना जाता है, फिर मानक में समान गुणों को।

### Standard {#Standard}
```
public static final int Standard
```


निम्नलिखित गुणों को ध्यान में रखा जाता है: पूर्ववर्ती संबंध, कुल स्लैक (जिस कार्य का कुल स्लैक अधिक हो वह पहले विलंबित होता है), प्रारंभ तिथि, प्राथमिकता। यह डिफ़ॉल्ट मान है।

