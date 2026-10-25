---
title: "PrimaveraDbReader"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Primavera DB'den Proje Bilgisi okumak için bir okuyucuyu temsil eder."
type: docs
weight: 200
url: /tr/java/com.aspose.tasks/primaveradbreader/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.PrimaveraBaseReader](../../com.aspose.tasks/primaverabasereader)
```
public final class PrimaveraDbReader extends PrimaveraBaseReader
```

Primavera DB'den Proje Bilgisi okumak için bir okuyucuyu temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [PrimaveraDbReader(PrimaveraDbSettings dbSettings)](#PrimaveraDbReader-com.aspose.tasks.PrimaveraDbSettings-) | Yeni bir [PrimaveraXerReader](../../com.aspose.tasks/primaveraxerreader) sınıfının örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [loadProject(int projectUid)](#loadProject-int-) | Belirtilen benzersiz tanımlayıcı ile projeyi yükler. |
### PrimaveraDbReader(PrimaveraDbSettings dbSettings) {#PrimaveraDbReader-com.aspose.tasks.PrimaveraDbSettings-}
```
public PrimaveraDbReader(PrimaveraDbSettings dbSettings)
```


Yeni bir [PrimaveraXerReader](../../com.aspose.tasks/primaveraxerreader) sınıfının örneğini başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dbSettings | [PrimaveraDbSettings](../../com.aspose.tasks/primaveradbsettings) | Primavera DB'ye nasıl bağlanılacağını belirten ayarlar. |

### loadProject(int projectUid) {#loadProject-int-}
```
public Project loadProject(int projectUid)
```


Belirtilen benzersiz tanımlayıcı ile projeyi yükler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| projectUid | int | Yüklenmekte olan projenin benzersiz tanımlayıcısı. |

**Returns:**
[Project](../../com.aspose.tasks/project) - Project with specified unique identifier read from Primavera DB. Null if project doesn't exist.
