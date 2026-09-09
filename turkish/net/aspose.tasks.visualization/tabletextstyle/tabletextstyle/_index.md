---
title: "TableTextStyle.TableTextStyle"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "TableTextStyle yapıcı. TableTextStyle sınıfının yeni bir örneğini başlatır"
type: docs
weight: 10
url: /tr/net/aspose.tasks.visualization/tabletextstyle/tabletextstyle/
---
## TableTextStyle(int) {#constructor}

[`TableTextStyle`](../) sınıfının yeni bir örneğini başlatır.

```csharp
public TableTextStyle(int rowUid)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowUid | Int32 | Belirtilen bir satırın benzersiz kimliği. |

## Örnekler

Bir projedeki farklı metin öğelerini biçimlendirmek için kullanılan tablo metin stillerinin nasıl özelleştirileceğini gösterir.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.NewTasksAreManual, false);

var view = (GanttChartView)project.Views.ToList()[0];

// ilk görev adı metin stilini ayarla
var style1 = new TableTextStyle(1);
// stilin uygulanacağı bir alan ayarla.
style1.Field = Field.TaskName;
// metin stilinin <see cref="P:Aspose.Tasks.Visualization.TextStyle.Font" /> ayarla.
style1.Font = new FontDescriptor("Impact", 12F, FontStyles.Bold | FontStyles.Italic);
// metin stili yazı tipinin punto cinsinden boyutunu ayarla.

// ikinci görev süresi metin stilini ayarla
var style2 = new TableTextStyle(2);
style2.Field = Field.TaskDurationText;
style2.Font = new FontDescriptor("Impact", 16F, FontStyles.Underline);

view.TableTextStyles.Add(style1);
view.TableTextStyles.Add(style2);

SimpleSaveOptions options = new MPPSaveOptions
{
    // görünüm verisinin yazılması gerektiğini gösteren bir bayrak ayarla
    WriteViewData = true
};
project.Save(OutDir + "WorkWithTableTextStyle_out.mpp", options);
```

### Ayrıca Bakınız

* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TableTextStyle(int, FontDescriptor) {#constructor_1}

[`TableTextStyle`](../) sınıfının belirtilen yazı tipiyle yeni bir örneğini başlatır.

```csharp
public TableTextStyle(int rowUid, FontDescriptor font)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowUid | Int32 | Belirtilen bir satırın benzersiz kimliği. |
| font | FontDescriptor | Bir metin stilinin temel alındığı yazı tipi. |

### Ayrıca Bakınız

* class [FontDescriptor](../../fontdescriptor/)
* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TableTextStyle(int, float, FontStyles) {#constructor_3}

[`TableTextStyle`](../) sınıfının belirtilen yazı tipi boyutu ve yazı tipi stiliyle yeni bir örneğini başlatır.

```csharp
public TableTextStyle(int rowUid, float fontSize, FontStyles fontStyle)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowUid | Int32 | Belirtilen bir satırın benzersiz kimliği. |
| fontSize | Single | Bir metin stilinin temel alındığı yazı tipinin boyutu. |
| fontStyle | FontStyles | Bir metin stilinin temel alındığı yazı tipinin stili. |

### Ayrıca Bakınız

* enum [FontStyles](../../fontstyles/)
* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TableTextStyle(int, FontStyles) {#constructor_2}

[`TableTextStyle`](../) sınıfının varsayılan yazı tipi ayarları ve belirtilen yazı tipi stiliyle yeni bir örneğini başlatır.

```csharp
public TableTextStyle(int rowUid, FontStyles fontStyle)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowUid | Int32 | Belirtilen bir satırın benzersiz kimliği. |
| fontStyle | FontStyles | Bir metin stilinin temel alındığı yazı tipinin stili. |

### Ayrıca Bakınız

* enum [FontStyles](../../fontstyles/)
* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)


