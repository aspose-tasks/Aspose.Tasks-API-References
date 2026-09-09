---
title: "Table.ShowAddNewColumn"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Table özelliği. Yeni Sütun Ekle arayüzünün gösterilip gösterilmeyeceğini belirten bir değeri alır veya ayarlar. MSP 2010 ve sonraki sürümler tarafından desteklenir"
type: docs
weight: 70
url: /tr/net/aspose.tasks/table/showaddnewcolumn/
---
## Table.ShowAddNewColumn property

'Add New Column' arayüzünün gösterilip gösterilmeyeceğini belirten bir değeri alır veya ayarlar. MSP 2010 ve sonraki sürümler tarafından desteklenir.

```csharp
public bool ShowAddNewColumn { get; set; }
```

## Örnekler

Yeni bir tabloyu (görünümler için kullanarak) nasıl tanımlayacağınızı gösterir.

```csharp
var project = new Project(DataDir + "Project1.mpp");

// düzenlemek için bir tablo al
var table = project.Tables.ToList()[0];
Console.WriteLine("Uid of the table: " + table.Uid);
Console.WriteLine("Name of the table: " + table.Name);
Console.WriteLine("Type of the table: " + table.TableType);

// bazı özellikleri ayarla
// tablonun başlık satırı yüksekliğinin ayarlanıp ayarlanamayacağını belirten bir değer ayarlar
table.AdjustHeaderRowHeight = true;

// tablonun tarih formatını ayarlar.
table.DateFormat = DateFormat.DateDdMmYyyy;

// tablonun ilk sütununun kilitli mi yoksa düzenlenebilir mi olduğunu belirten bir değer ayarlar
table.LockFirstColumn = true;

// tablodaki satır yüksekliğini, satır yüksekliğinin metin satır sayısı olduğu şekilde ayarlar
table.RowHeight = 10;

// 'Yeni Sütun Ekle' arayüzünün gösterilip gösterilmeyeceğini belirten bir değer ayarlar
table.ShowAddNewColumn = true;

// projenin, Şerit'in Görünüm sekmesindeki Tablolar açılır listesindeki tablo adını gösterip göstermeyeceğini belirten bir değer ayarlar
table.ShowInMenu = true;

// güncellenmiş tabloyu kaydetmeye izin verir
project.Save(OutDir + "WorkWithTable_out.mpp", SaveFileFormat.Mpp);
```

### Ayrıca Bakınız

* class [Table](../)
* namespace [Aspose.Tasks](../../table/)
* assembly [Aspose.Tasks](../../../)


