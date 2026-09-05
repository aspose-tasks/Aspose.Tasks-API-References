---
title: "View"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Mewakili tampilan dalam Project."
type: docs
weight: 342
url: /id/java/com.aspose.tasks/view/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Comparable
```
public class View implements Comparable<View>
```

Mewakili tampilan dalam Project.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [View()](#View--) | Menginisialisasi instance baru dari kelas [View](../../com.aspose.tasks/view). |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [compareTo(View other)](#compareTo-com.aspose.tasks.View-) | Membandingkan instance saat ini dengan objek lain dari tipe yang sama dan mengembalikan integer yang menunjukkan apakah instance saat ini mendahului, mengikuti, atau berada pada posisi yang sama dalam urutan penyortiran dibandingkan objek lainnya. |
| [equals(Object obj)](#equals-java.lang.Object-) | Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan. |
| [forViewScreen(int viewScreen)](#forViewScreen-int-) | Membuat instance baru dari kelas [View](../../com.aspose.tasks/view). |
| [getFilter()](#getFilter--) | Mengambil filter yang digunakan dalam satu tampilan. |
| [getGroup()](#getGroup--) | Mengambil grup dari tampilan tunggal. |
| [getHighlightFilter()](#getHighlightFilter--) | Mengambil nilai yang menunjukkan apakah Microsoft Project menyorot filter untuk satu tampilan. |
| [getName()](#getName--) | Mengambil nama objek View. |
| [getPageInfo()](#getPageInfo--) | Mengambil instance dari kelas `PageInfo`([getPageInfo()](../../com.aspose.tasks/view\#getPageInfo--)). |
| [getParentProject()](#getParentProject--) | Mengambil induk dari objek View. |
| [getScreen()](#getScreen--) | Mengambil tipe layar untuk tampilan tunggal. |
| [getShowInMenu()](#getShowInMenu--) | Mengambil nilai yang menunjukkan apakah Microsoft Project menampilkan nama tampilan tunggal di daftar drop-down View atau Other Views pada Ribbon. |
| [getTable()](#getTable--) | Mengambil tabel dari tampilan tunggal. |
| [getType()](#getType--) | Mendapatkan tipe item dalam tampilan tunggal, seperti tugas atau sumber daya. |
| [getUid()](#getUid--) | Mendapatkan pengidentifikasi unik dari sebuah tampilan. |
| [getVisualObjectsPlacements()](#getVisualObjectsPlacements--) | Mendapatkan koleksi objek yang mewakili penempatan dan tampilan [OleObject](../../com.aspose.tasks/oleobject) dalam tampilan. |
| [hashCode()](#hashCode--) | Mengembalikan nilai kode hash untuk instance kelas [Resource](../../com.aspose.tasks/resource). |
| [op_Equality(View a, View b)](#op-Equality-com.aspose.tasks.View-com.aspose.tasks.View-) | Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan. |
| [op_GreaterThan(View a, View b)](#op-GreaterThan-com.aspose.tasks.View-com.aspose.tasks.View-) | Mengembalikan nilai yang menunjukkan apakah instance ini lebih besar dari objek yang ditentukan. |
| [op_GreaterThanOrEqual(View a, View b)](#op-GreaterThanOrEqual-com.aspose.tasks.View-com.aspose.tasks.View-) | Mengembalikan nilai yang menunjukkan apakah instance ini lebih besar atau sama dengan objek yang ditentukan. |
| [op_Inequality(View a, View b)](#op-Inequality-com.aspose.tasks.View-com.aspose.tasks.View-) | Mengembalikan nilai yang menunjukkan apakah instance ini tidak sama dengan objek yang ditentukan. |
| [op_LessThan(View a, View b)](#op-LessThan-com.aspose.tasks.View-com.aspose.tasks.View-) | Mengembalikan nilai yang menunjukkan apakah instance ini lebih kecil dari objek yang ditentukan. |
| [op_LessThanOrEqual(View a, View b)](#op-LessThanOrEqual-com.aspose.tasks.View-com.aspose.tasks.View-) | Mengembalikan nilai yang menunjukkan apakah instance ini lebih kecil atau sama dengan objek yang ditentukan. |
| [setFilter(Filter value)](#setFilter-com.aspose.tasks.Filter-) | Menetapkan filter yang digunakan dalam tampilan tunggal. |
| [setGroup(Group value)](#setGroup-com.aspose.tasks.Group-) | Menetapkan grup dari tampilan tunggal. |
| [setHighlightFilter(boolean value)](#setHighlightFilter-boolean-) | Menetapkan nilai yang menunjukkan apakah Microsoft Project menyoroti filter untuk tampilan tunggal. |
| [setName(String value)](#setName-java.lang.String-) | Menetapkan nama dari objek View. |
| [setShowInMenu(boolean value)](#setShowInMenu-boolean-) | Menetapkan nilai yang menunjukkan apakah Microsoft Project menampilkan nama tampilan tunggal di dalam daftar drop-down View atau Other Views pada Ribbon. |
| [setTable(Table value)](#setTable-com.aspose.tasks.Table-) | Menetapkan tabel dari tampilan tunggal. |
### View() {#View--}
```
public View()
```


Menginisialisasi instance baru dari kelas [View](../../com.aspose.tasks/view).

### compareTo(View other) {#compareTo-com.aspose.tasks.View-}
```
public final int compareTo(View other)
```


Membandingkan instance saat ini dengan objek lain dari tipe yang sama dan mengembalikan integer yang menunjukkan apakah instance saat ini mendahului, mengikuti, atau berada pada posisi yang sama dalam urutan penyortiran dibandingkan objek lainnya.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| other | [View](../../com.aspose.tasks/view) | objek View yang ditentukan untuk dibandingkan dengan instance ini. |

**Returns:**
int - Integer 32-bit bertanda yang menunjukkan urutan relatif objek-objek yang dibandingkan. Nilai kembali memiliki arti berikut: Nilai Arti Kurang dari nol Instance ini mendahului `other` dalam urutan penyortiran. Nol Instance ini berada pada posisi yang sama dalam urutan penyortiran dengan `other`. Lebih dari nol Instance ini mengikuti `other` dalam urutan penyortiran.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| obj | java.lang.Object | Objek untuk dibandingkan dengan instance ini. |

**Returns:**
boolean - **True** jika objek yang ditentukan adalah View yang memiliki nilai Uid yang sama dengan instance ini; jika tidak, **false**.
### forViewScreen(int viewScreen) {#forViewScreen-int-}
```
public static View forViewScreen(int viewScreen)
```


Membuat instance baru dari kelas [View](../../com.aspose.tasks/view).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| viewScreen | int | Tipe layar untuk yang dapat menampilkan tampilan. |

**Returns:**
[View](../../com.aspose.tasks/view) - Constructed view.
### getFilter() {#getFilter--}
```
public final Filter getFilter()
```


Mengambil filter yang digunakan dalam satu tampilan.

**Returns:**
[Filter](../../com.aspose.tasks/filter) - a filter used in a single view.
### getGroup() {#getGroup--}
```
public final Group getGroup()
```


Mengambil grup dari tampilan tunggal.

**Returns:**
[Group](../../com.aspose.tasks/group) - a group of the single view.
### getHighlightFilter() {#getHighlightFilter--}
```
public final boolean getHighlightFilter()
```


Mengambil nilai yang menunjukkan apakah Microsoft Project menyorot filter untuk satu tampilan.

**Returns:**
boolean - nilai yang menunjukkan apakah Microsoft Project menyoroti filter untuk tampilan tunggal.
### getName() {#getName--}
```
public final String getName()
```


Mengambil nama objek View.

**Returns:**
java.lang.String - nama dari objek View.
### getPageInfo() {#getPageInfo--}
```
public final PageInfo getPageInfo()
```


Mendapatkan instance dari kelas `PageInfo`([getPageInfo()](../../com.aspose.tasks/view\\#getPageInfo--)). Mewakili data pengaturan halaman yang terdapat dalam format file mpp.

**Returns:**
[PageInfo](../../com.aspose.tasks/pageinfo) - an instance of the `PageInfo`([getPageInfo()](../../com.aspose.tasks/view\#getPageInfo--)) class.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Mendapatkan induk dari objek View. Hanya-baca [Project](../../com.aspose.tasks/project).

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent of the View object.
### getScreen() {#getScreen--}
```
public final int getScreen()
```


Mendapatkan tipe layar untuk tampilan tunggal. Hanya-baca [ViewScreen](../../com.aspose.tasks/viewscreen).

**Returns:**
int - tipe layar untuk tampilan tunggal.
### getShowInMenu() {#getShowInMenu--}
```
public final boolean getShowInMenu()
```


Mengambil nilai yang menunjukkan apakah Microsoft Project menampilkan nama tampilan tunggal di daftar drop-down View atau Other Views pada Ribbon.

**Returns:**
boolean - nilai yang menunjukkan apakah Microsoft Project menampilkan nama tampilan tunggal di dalam daftar drop-down View atau Other Views pada Ribbon.
### getTable() {#getTable--}
```
public final Table getTable()
```


Mengambil tabel dari tampilan tunggal.

**Returns:**
[Table](../../com.aspose.tasks/table) - a table of the single view.
### getType() {#getType--}
```
public final int getType()
```


Mendapatkan tipe item dalam tampilan tunggal, seperti tugas atau sumber daya. Hanya-baca [ItemType](../../com.aspose.tasks/itemtype).

**Returns:**
int - tipe item dalam tampilan tunggal, seperti tugas atau sumber daya.
### getUid() {#getUid--}
```
public final int getUid()
```


Mendapatkan pengidentifikasi unik dari sebuah tampilan.

**Returns:**
int - pengidentifikasi unik dari sebuah tampilan.
### getVisualObjectsPlacements() {#getVisualObjectsPlacements--}
```
public final List<VisualObjectPlacement> getVisualObjectsPlacements()
```


Mendapatkan koleksi objek yang mewakili penempatan dan tampilan [OleObject](../../com.aspose.tasks/oleobject) dalam tampilan.

**Returns:**
java.util.List&lt;com.aspose.tasks.VisualObjectPlacement&gt; - koleksi objek yang mewakili penempatan dan tampilan [OleObject](../../com.aspose.tasks/oleobject) dalam tampilan.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Mengembalikan nilai kode hash untuk instance kelas [Resource](../../com.aspose.tasks/resource).

**Returns:**
int - mengembalikan nilai kode hash untuk objek ini.
### op_Equality(View a, View b) {#op-Equality-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_Equality(View a, View b)
```


Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | Tampilan pertama. |
| b | [View](../../com.aspose.tasks/view) | Tampilan kedua. |

**Returns:**
boolean - nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan
### op_GreaterThan(View a, View b) {#op-GreaterThan-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_GreaterThan(View a, View b)
```


Mengembalikan nilai yang menunjukkan apakah instance ini lebih besar dari objek yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | Tampilan pertama. |
| b | [View](../../com.aspose.tasks/view) | Tampilan kedua. |

**Returns:**
boolean - nilai yang menunjukkan apakah instance ini lebih besar dari objek yang ditentukan
### op_GreaterThanOrEqual(View a, View b) {#op-GreaterThanOrEqual-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_GreaterThanOrEqual(View a, View b)
```


Mengembalikan nilai yang menunjukkan apakah instance ini lebih besar atau sama dengan objek yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | Tampilan pertama. |
| b | [View](../../com.aspose.tasks/view) | Tampilan kedua. |

**Returns:**
boolean - nilai yang menunjukkan apakah instance ini lebih besar dari atau sama dengan objek yang ditentukan
### op_Inequality(View a, View b) {#op-Inequality-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_Inequality(View a, View b)
```


Mengembalikan nilai yang menunjukkan apakah instance ini tidak sama dengan objek yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | Tampilan pertama. |
| b | [View](../../com.aspose.tasks/view) | Tampilan kedua. |

**Returns:**
boolean - nilai yang menunjukkan apakah instance ini tidak sama dengan objek yang ditentukan
### op_LessThan(View a, View b) {#op-LessThan-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_LessThan(View a, View b)
```


Mengembalikan nilai yang menunjukkan apakah instance ini lebih kecil dari objek yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | Filter pertama. |
| b | [View](../../com.aspose.tasks/view) | Filter kedua. |

**Returns:**
boolean - nilai yang menunjukkan apakah instance ini lebih kecil dari objek yang ditentukan
### op_LessThanOrEqual(View a, View b) {#op-LessThanOrEqual-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_LessThanOrEqual(View a, View b)
```


Mengembalikan nilai yang menunjukkan apakah instance ini lebih kecil atau sama dengan objek yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | Tampilan pertama. |
| b | [View](../../com.aspose.tasks/view) | Tampilan kedua. |

**Returns:**
boolean - nilai yang menunjukkan apakah instance ini lebih kecil dari atau sama dengan objek yang ditentukan
### setFilter(Filter value) {#setFilter-com.aspose.tasks.Filter-}
```
public final void setFilter(Filter value)
```


Menetapkan filter yang digunakan dalam tampilan tunggal.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [Filter](../../com.aspose.tasks/filter) | filter yang digunakan dalam satu tampilan. |

### setGroup(Group value) {#setGroup-com.aspose.tasks.Group-}
```
public final void setGroup(Group value)
```


Menetapkan grup dari tampilan tunggal.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [Group](../../com.aspose.tasks/group) | kelompok dari tampilan tunggal. |

### setHighlightFilter(boolean value) {#setHighlightFilter-boolean-}
```
public final void setHighlightFilter(boolean value)
```


Menetapkan nilai yang menunjukkan apakah Microsoft Project menyoroti filter untuk tampilan tunggal.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah Microsoft Project menyorot filter untuk satu tampilan. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Menetapkan nama dari objek View.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | nama objek View. |

### setShowInMenu(boolean value) {#setShowInMenu-boolean-}
```
public final void setShowInMenu(boolean value)
```


Menetapkan nilai yang menunjukkan apakah Microsoft Project menampilkan nama tampilan tunggal di dalam daftar drop-down View atau Other Views pada Ribbon.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah Microsoft Project menampilkan nama tampilan tunggal di daftar drop-down View atau Other Views di Ribbon. |

### setTable(Table value) {#setTable-com.aspose.tasks.Table-}
```
public final void setTable(Table value)
```


Menetapkan tabel dari tampilan tunggal.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [Table](../../com.aspose.tasks/table) | tabel dari tampilan tunggal. |

