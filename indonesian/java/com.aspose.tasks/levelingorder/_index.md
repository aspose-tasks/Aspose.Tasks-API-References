---
title: "LevelingOrder"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Mendefinisikan nilai yang mungkin dari urutan penyeimbangan."
type: docs
weight: 143
url: /id/java/com.aspose.tasks/levelingorder/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class LevelingOrder extends System.Enum
```

Mendefinisikan nilai yang mungkin dari urutan penyeimbangan.
## Bidang

| Bidang | Deskripsi |
| --- | --- |
| [IdOnly](#IdOnly) | Tugas ditunda dalam urutan Id naik. |
| [PriorityThenStandard](#PriorityThenStandard) | Prioritas dipertimbangkan pertama, kemudian properti yang sama seperti di Standard. |
| [Standard](#Standard) | Properti berikut dipertimbangkan: hubungan pendahulu, slack total (tugas dengan slack total lebih tinggi ditunda pertama), tanggal mulai, prioritas. |
### IdOnly {#IdOnly}
```
public static final int IdOnly
```


Tugas ditunda dalam urutan Id naik.

### PriorityThenStandard {#PriorityThenStandard}
```
public static final int PriorityThenStandard
```


Prioritas dipertimbangkan pertama, kemudian properti yang sama seperti di Standard.

### Standard {#Standard}
```
public static final int Standard
```


Properti berikut dipertimbangkan: hubungan pendahulu, slack total (tugas dengan slack total lebih tinggi ditunda pertama), tanggal mulai, prioritas. Ini adalah nilai default.

