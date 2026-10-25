---
title: "Table.Uid"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Table özelliği. Bir tablonun benzersiz tanımlayıcısını alır"
type: docs
weight: 110
url: /tr/net/aspose.tasks/table/uid/
---
## Table.Uid property

Bir tablonun benzersiz tanımlayıcısını alır.

```csharp
public int Uid { get; }
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


