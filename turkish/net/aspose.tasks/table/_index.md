---
title: "Table sınıfı"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Table sınıfı. Project içinde bir tabloyu temsil eder."
type: docs
weight: 2320
url: /tr/net/aspose.tasks/table/
---
## Table class

Project içinde bir tabloyu temsil eder.

```csharp
public class Table
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [Table](table/)() | `Table` sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [AdjustHeaderRowHeight](../../aspose.tasks/table/adjustheaderrowheight/) { get; set; } | Tablonun başlık satırı yüksekliğinin ayarlanıp ayarlanamayacağını gösteren bir değeri alır veya ayarlar. |
| [DateFormat](../../aspose.tasks/table/dateformat/) { get; set; } | Tablonun tarih formatını alır veya ayarlar. |
| [LockFirstColumn](../../aspose.tasks/table/lockfirstcolumn/) { get; set; } | Tablonun ilk sütununun kilitli mi yoksa düzenlenebilir mi olduğunu gösteren bir değeri alır veya ayarlar. |
| [Name](../../aspose.tasks/table/name/) { get; set; } | Bir Table nesnesinin adını alır veya ayarlar. |
| [RowHeight](../../aspose.tasks/table/rowheight/) { get; set; } | Tablodaki satır yüksekliğini alır veya ayarlar; satır yüksekliği metin satır sayısıdır. |
| [ShowAddNewColumn](../../aspose.tasks/table/showaddnewcolumn/) { get; set; } | 'Add New Column' arayüzünün gösterilip gösterilmeyeceğini belirten bir değeri alır veya ayarlar. MSP 2010 ve sonraki sürümler tarafından desteklenir. |
| [ShowInMenu](../../aspose.tasks/table/showinmenu/) { get; set; } | Projenin, Şeritteki Görünüm sekmesindeki Tablolar açılır listesinde tablo adını gösterip göstermeyeceğini belirten bir değeri alır veya ayarlar. |
| [TableFields](../../aspose.tasks/table/tablefields/) { get; } | Tablodaki alanları temsil eden bir TableFields koleksiyonunu alır. |
| [TableType](../../aspose.tasks/table/tabletype/) { get; set; } | Belirtilen tablo için tablo tipini alır veya ayarlar. |
| [Uid](../../aspose.tasks/table/uid/) { get; } | Bir tablonun benzersiz tanımlayıcısını alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| override [Equals](../../aspose.tasks/table/equals/)(object) | Bu örneğin belirtilen nesneye eşit olup olmadığını gösteren bir değer döndürür. |
| override [GetHashCode](../../aspose.tasks/table/gethashcode/)() | Bu Tablo için bir karma kodu döndürür. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


