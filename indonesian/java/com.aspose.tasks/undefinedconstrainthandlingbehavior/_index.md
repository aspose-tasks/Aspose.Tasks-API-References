---
title: "UndefinedConstraintHandlingBehavior"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Menentukan perilaku yang digunakan untuk menangani tugas dengan batasan yang tidak terdefinisi."
type: docs
weight: 329
url: /id/java/com.aspose.tasks/undefinedconstrainthandlingbehavior/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class UndefinedConstraintHandlingBehavior extends System.Enum
```

Menentukan perilaku yang digunakan untuk menangani tugas dengan batasan yang tidak terdefinisi.
## Bidang

| Bidang | Deskripsi |
| --- | --- |
| [None](#None) | Perilaku default untuk memuat dari format XER. |
| [SubstituteWithStartNoEarlierThan](#SubstituteWithStartNoEarlierThan) | Kendala dengan tipe 'ConstraintType.StartNoEarlierThan' dan tanggal = Start ditambahkan untuk tugas dengan kendala 'Undefined'. |
### None {#None}
```
public static final int None
```


Perilaku default untuk memuat dari format XER. Tidak ada tindakan yang diambil. Tipe kendala tugas diatur ke 'ConstraintType.Undefined'.

### SubstituteWithStartNoEarlierThan {#SubstituteWithStartNoEarlierThan}
```
public static final int SubstituteWithStartNoEarlierThan
```


Kendala dengan tipe 'ConstraintType.StartNoEarlierThan' dan tanggal = Start ditambahkan untuk tugas dengan kendala 'Undefined'.

