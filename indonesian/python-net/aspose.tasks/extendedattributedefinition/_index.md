---
title: "ExtendedAttributeDefinition"
second_title: "Referensi API Aspose.Tasks untuk Python via .NET"
description: 
type: docs
weight: 310
url: /id/python-net/aspose.tasks/extendedattributedefinition/
---

## ExtendedAttributeDefinition class

Mewakili definisi atribut tambahan yang terkait dengan sebuah proyek.

Tipe ExtendedAttributeDefinition menampilkan anggota-anggota berikut:
## Properti
| Nama | Deskripsi |
| :- | :- |
| field_id | Mendapatkan atau mengatur yang sesuai dengan id proyek dari bidang khusus.<br/>            Gunakan representasi string dari sebuah konstanta dari kelas [ExtendedAttributeTask](/tasks/python-net/aspose.tasks/extendedattributetask/) untuk menentukan properti [field_id](/tasks/python-net/aspose.tasks/extendedattributedefinition/). |
| field_name | Mendapatkan nama dari bidang khusus. |
| cf_type | Mendapatkan tipe dari bidang khusus. |
| guid | Mendapatkan atau mengatur Guid dari bidang khusus. |
| element_type | Mendapatkan atau mengatur atribut ekstended yang terkait<br/>            dengan sebuah tugas, sebuah sumber daya, atau sebuah penugasan. |
| max_multi_values | Mendapatkan atau mengatur jumlah maksimum nilai yang dapat Anda atur dalam daftar pilihan. |
| user_def | Mendapatkan atau mengatur nilai yang menunjukkan apakah bidang khusus didefinisikan oleh pengguna. |
| alias | Mendapatkan atau mengatur alias dari bidang khusus. |
| secondary_pid | Mendapatkan atau mengatur PID sekunder dari bidang khusus. |
| auto_roll_down | Mendapatkan atau mengatur nilai yang menunjukkan apakah penurunan otomatis ke penugasan diaktifkan. |
| default_guid | Mendapatkan atau mengatur Guid dari entri tabel pencarian default. |
| lookup_uid | Mendapatkan Guid dari tabel pencarian yang terkait dengan bidang khusus. |
| phonetics_alias | Mendapatkan atau mengatur pengucapan fonetik dari alias bidang khusus. |
| rollup_type | Mendapatkan atau mengatur cara perhitungan rollup. |
| calculation_type | Mendapatkan atau mengatur tipe perhitungan nilai atribut khusus. |
| summary_rows_calculation_type | Mendapatkan atau mengatur tipe perhitungan nilai atribut khusus untuk baris ringkasan. |
| formula | Mendapatkan atau mengatur rumus yang digunakan Microsoft Project untuk mengisi bidang tugas khusus. |
| graphical_indicator | Mendapatkan atau mengatur info indikator grafis yang terkait dengan atribut yang diperluas.<br/>            Berlaku untuk format MPP. |
| restrict_values | Mendapatkan atau mengatur nilai yang menunjukkan apakah nilai bidang khusus dibatasi pada nilai dalam [value_list](/tasks/python-net/aspose.tasks/extendedattributedefinition/). |
| valuelist_sort_order | Mendapatkan atau mengatur cara daftar nilai diurutkan. Nilainya: 0=Menurun, 1=Naik. |
| append_new_values | Mendapatkan atau mengatur nilai yang menunjukkan apakah nilai baru yang ditambahkan ke proyek secara otomatis ditambahkan ke daftar. |
| default | Mendapatkan atau mengatur nilai default dalam daftar. |
| value_list | Mendapatkan List<Value> ValueList. |
| secondary_guid | Mendapatkan atau mengatur GUID sekunder dari atribut yang diperluas. |
| parent_project | Mendapatkan proyek induk untuk instance [ExtendedAttributeDefinition](/tasks/python-net/aspose.tasks/extendedattributedefinition/). |
## Methods
| Nama | Deskripsi |
| :- | :- |
| create_extended_attribute() | Membuat atribut yang diperluas baru dengan ID bidang yang sama dengan nilai ID bidang objek ini. |
| create_extended_attribute(text_value) | Membuat atribut yang diperluas baru dengan ID bidang yang sama dengan nilai ID bidang objek ini dan nilai teks yang ditentukan. |
| create_extended_attribute(numeric_value) | Membuat atribut yang diperluas baru dengan ID bidang yang sama dengan nilai ID bidang objek ini dan nilai numerik yang ditentukan. |
| create_extended_attribute(date_time_value) | Membuat atribut yang diperluas baru dengan ID bidang yang sama dengan nilai ID bidang objek ini dan nilai tanggal yang ditentukan. |
| create_extended_attribute(duration_value) | Membuat atribut yang diperluas baru dengan ID bidang yang sama dengan nilai ID bidang objek ini dan nilai durasi yang ditentukan. |
| create_extended_attribute(flag_value) | Membuat atribut yang diperluas baru dengan ID bidang yang sama dengan nilai ID bidang objek ini dan nilai flag yang ditentukan. |
| create_extended_attribute(lookup_value) | Membuat atribut ekstensi baru yang terhubung dengan item [Value](/tasks/python-net/aspose.tasks/value/) yang ditentukan. |
| create_task_definition(custom_field_type, field_id, alias) | Metode pabrik yang membuat definisi atribut ekstensi sederhana, yang ditampilkan Microsoft Project sebagai "None".<br/>            Memiliki [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) yang bernilai [NONE](/tasks/python-net/aspose.tasks/calculationtype/) dan hanya dapat digunakan dalam Tasks.<br/>            Anda harus menentukan |
| create_task_definition(field_id, alias) | Metode pabrik yang membuat definisi atribut ekstensi sederhana, yang ditampilkan Microsoft Project sebagai "None".<br/>            Memiliki [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) yang bernilai [NONE](/tasks/python-net/aspose.tasks/calculationtype/) dan hanya dapat digunakan dalam Tasks.<br/>            Anda harus menentukan |
| create_resource_definition(custom_field_type, field_id, alias) | Metode pabrik yang membuat definisi atribut ekstensi sederhana, yang ditampilkan Microsoft Project sebagai "None".<br/>            Memiliki [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) yang bernilai [NONE](/tasks/python-net/aspose.tasks/calculationtype/) dan hanya dapat digunakan dalam Resource.<br/>            Anda harus menentukan |
| create_resource_definition(field_id, alias) | Metode pabrik yang membuat definisi atribut ekstensi sederhana, yang ditampilkan Microsoft Project sebagai "None".<br/>            Memiliki [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) yang bernilai [NONE](/tasks/python-net/aspose.tasks/calculationtype/) dan hanya dapat digunakan dalam Resource.<br/>            Anda harus menentukan |
| create_lookup_task_definition(field_id, alias) | Metode pabrik yang membuat definisi atribut ekstensi dengan lookup.<br/>            Memiliki [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) yang bernilai [LOOKUP](/tasks/python-net/aspose.tasks/calculationtype/) dan hanya dapat digunakan dalam Tasks.<br/>            Anda harus menentukan |
| create_lookup_task_definition(custom_field_type, field_id, alias) | Metode pabrik yang membuat definisi atribut ekstensi dengan lookup.<br/>            Memiliki [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) yang bernilai [LOOKUP](/tasks/python-net/aspose.tasks/calculationtype/) dan hanya dapat digunakan dalam Tasks.<br/>            Anda harus menentukan |
| create_lookup_resource_definition(field_id, alias) | Metode pabrik yang membuat definisi atribut ekstensi dengan lookup.<br/>            Memiliki [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) yang bernilai [LOOKUP](/tasks/python-net/aspose.tasks/calculationtype/) dan hanya dapat digunakan dalam Resources.<br/>            Anda harus menentukan |
| create_lookup_resource_definition(custom_field_type, field_id, alias) | Metode pabrik yang membuat definisi atribut ekstensi dengan lookup.<br/>            Memiliki [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) yang bernilai [LOOKUP](/tasks/python-net/aspose.tasks/calculationtype/) dan hanya dapat digunakan dalam Resources.<br/>            Anda harus menentukan |
| add_lookup_value(value) | Menambahkan nilai ke daftar lookup internal. Ini adalah cara yang disarankan untuk manipulasi dengan [value_list](/tasks/python-net/aspose.tasks/extendedattributedefinition/). |
| remove_lookup_value(value) | Menghapus nilai dari daftar lookup internal. Ini adalah cara yang disarankan untuk manipulasi dengan [value_list](/tasks/python-net/aspose.tasks/extendedattributedefinition/). |

### Lihat Juga

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

