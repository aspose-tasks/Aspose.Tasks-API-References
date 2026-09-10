---
title: "Calendar"
second_title: "Referensi API Aspose.Tasks untuk Python via .NET"
description: 
type: docs
weight: 140
url: /id/python-net/aspose.tasks/calendar/
---

## Calendar class

Mewakili kalender yang digunakan dalam sebuah proyek.

Tipe Calendar menampilkan anggota-anggota berikut:
## Properti
| Nama | Deskripsi |
| :- | :- |
| name | Mendapatkan atau mengatur nama kalender. |
| uid | Mendapatkan atau mengatur pengidentifikasi unik kalender. |
| week_days | Mendapatkan WeekDaysCollection untuk kalender ini.<br/>            Kumpulan hari kerja yang mendefinisikan kalender. |
| exceptions | Mendapatkan objek CalendarExceptionCollection.<br/>            Kumpulan pengecualian yang terkait dengan kalender. |
| work_weeks | Mendapatkan objek WorkWeekCollections.<br/>            Kumpulan minggu kerja yang terkait dengan kalender. |
| is_base_calendar | Mendapatkan nilai yang menunjukkan apakah kalender adalah kalender dasar. |
| base_calendar | Mendapatkan atau mengatur kalender dasar yang menjadi dependensi kalender ini.<br/>            Hanya berlaku jika kalender bukan kalender dasar. |
| is_baseline_calendar | Mendapatkan atau mengatur nilai yang menunjukkan apakah kalender adalah kalender baseline. |
| guid | Mendapatkan Guid kalender. |
| primavera_properties | Mendapatkan objek yang berisi properti khusus Primavera untuk kalender yang dibaca dari format Primavera. |
## Methods
| Nama | Deskripsi |
| :- | :- |
| get_start_date_from_finish_and_duration(finish, duration) | Mengembalikan tanggal mulai berdasarkan tanggal selesai yang ditentukan dan durasi. |
| get_start_date_from_finish_and_duration(finish, duration) | Mengembalikan tanggal mulai berdasarkan tanggal selesai dan durasi yang ditentukan. |
| get_working_hours(start, finish) | Mengembalikan WorkUnit - Mulai, Selesai, dan Durasi jam kerja untuk interval tanggal dan waktu yang ditentukan. |
| get_working_hours(dt) | Mengembalikan WorkUnit - Mulai, Selesai, dan Durasi jam kerja untuk interval tanggal dan waktu yang ditentukan. |
| get_finish_date_by_start_and_work(start, work) | Menghitung tanggal ketika jumlah waktu kerja yang ditentukan akan berlalu menurut kalender. |
| get_finish_date_by_start_and_work(start, work) | Menghitung tanggal ketika jumlah waktu kerja yang ditentukan akan berlalu menurut kalender. |
| get_intersection_calendar(calendar1, calendar2) | Mendapatkan instance [ICalendar](/tasks/python-net/aspose.tasks/icalendar/) yang dapat digunakan untuk melakukan perhitungan pada irisan jadwal kerja dari 2 kalender. |
| make_standard_calendar(calendar) | Membuat kalender standar default. |
| make_24_hour_calendar(calendar) | Mengubah Kalender menjadi Kalender 24Jam.<br/>            Kalender 24Jam adalah Kalender di mana setiap hari dalam seminggu bekerja dengan jam kerja 24 jam nonstop. |
| make_night_shift_calendar(calendar) | Mengubah Kalender menjadi Kalender Shift Malam. |
| delete() | Menghapus kalender dari proyek. |
| is_day_working(dt) | Menentukan apakah hari yang ditentukan adalah hari kerja menurut kalender. |
| get_working_hours_time_span(start, finish) | Mengembalikan jumlah jam kerja antara tanggal yang ditentukan. |
| get_task_finish_date_from_duration(task, duration) | Menghitung tanggal dan waktu selesai tugas dari tanggal mulai, bagian-bagian terpisah, dan durasi kerja. |
| get_working_times(dt) | Mengembalikan [WorkingTimeCollection](/tasks/python-net/aspose.tasks/workingtimecollection/) dari waktu kerja untuk tanggal yang ditentukan. |
| get_previous_working_day_end(date) | Menghitung akhir tanggal kerja sebelumnya dari tanggal yang ditentukan. |
| get_next_working_day_start(date) | Menghitung awal hari kerja berikutnya untuk tanggal yang ditentukan. |
| get_work_start(date) | Menghitung awal waktu kerja berikutnya mulai dari tanggal dan waktu yang ditentukan. |
| is_empty() | Mengembalikan apakah kalender tidak memiliki jam kerja yang didefinisikan. |

### Lihat Juga

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

