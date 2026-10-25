---
title: "Aspose::Tasks::Project::GetPageCount μέθοδος"
linktitle: "GetPageCount"
articleTitle: "GetPageCount"
second_title: "Aspose.Tasks για C++"
description: "Επιστρέφει τον αριθμό σελίδων για το έργο που θα αποδοθεί χρησιμοποιώντας την προεπιλεγμένη Timescale (Days)."
type: docs
weight: 1090
url: /el/cpp/aspose.tasks/project/getpagecount/
---

## GetPageCount (1 of 7) {#getpagecount_1}

Επιστρέφει τον αριθμό σελίδων για το έργο που θα αποδοθεί χρησιμοποιώντας την προεπιλεγμένη Timescale (Days).

**Returns:** Page count to be rendered.

```cpp
GetPageCount()
```

---

## GetPageCount (2 of 7) {#getpagecount_2}

Επιστρέφει τον αριθμό σελίδων για το έργο που θα αποδοθεί χρησιμοποιώντας τις δοσμένες SaveOptions .

**Returns:** a page count to be rendered.

```cpp
GetPageCount(const System::SharedPtr< Saving::SaveOptions > & saveOptions)
```

| Παράμετρος | Περιγραφή |
| --- | --- |
| saveOptions | Οι επιλογές αποθήκευσης για λήψη του αριθμού σελίδων. |

---

## GetPageCount (3 of 7) {#getpagecount_3}

Επιστρέφει τον αριθμό σελίδων για το έργο που θα αποδοθεί χρησιμοποιώντας τις δοσμένες Timescale και PageSize .

**Returns:** Page count to be rendered.

```cpp
GetPageCount(Visualization::PageSize pageSize, Visualization::Timescale scale)
```

| Παράμετρος | Περιγραφή |
| --- | --- |
| pageSize | Το μέγεθος για λήψη του αριθμού σελίδων. |
| scale | Η κλίμακα για την οποία θέλετε να λάβετε τον αριθμό σελίδων. |

---

## GetPageCount (4 of 7) {#getpagecount_4}

Επιστρέφει τον αριθμό σελίδων για το έργο που θα αποδοθεί χρησιμοποιώντας το δεδομένο Timescale, το PresentationFormat και το εύρος ημερομηνιών.

**Returns:** Page count to be rendered.

```cpp
GetPageCount(Visualization::PageSize pageSize, Visualization::Timescale scale, System::DateTime startDate, System::DateTime endDate)
```

| Παράμετρος | Περιγραφή |
| --- | --- |
| pageSize | Το μέγεθος για λήψη του αριθμού σελίδων. |
| scale | Η κλίμακα για την οποία θέλετε να λάβετε τον αριθμό σελίδων. |
| startDate | Η ημερομηνία έναρξης για την οποία θέλετε να λάβετε τον αριθμό σελίδων. |
| endDate | Η ημερομηνία λήξης για την οποία θέλετε να λάβετε τον αριθμό σελίδων. |

---

## GetPageCount (5 of 7) {#getpagecount_5}

Επιστρέφει τον αριθμό σελίδων για το έργο που θα αποδοθεί χρησιμοποιώντας το προεπιλεγμένο Timescale (Ημέρες) και το δεδομένο PresentationFormat.

**Returns:** Page count to be rendered.

```cpp
GetPageCount(Visualization::PresentationFormat format)
```

| Παράμετρος | Περιγραφή |
| --- | --- |
| μορφή | Η μορφή για την οποία θέλετε να λάβετε τον αριθμό σελίδων. |

---

## GetPageCount (6 of 7) {#getpagecount_6}

Επιστρέφει τον αριθμό σελίδων για το έργο που θα αποδοθεί χρησιμοποιώντας το δεδομένο Timescale και το PresentationFormat.

**Returns:** a page count to be rendered.

```cpp
GetPageCount(Visualization::PresentationFormat format, Visualization::Timescale scale)
```

| Παράμετρος | Περιγραφή |
| --- | --- |
| μορφή | Η μορφή για την οποία θέλετε να λάβετε τον αριθμό σελίδων. |
| scale | Η κλίμακα για την οποία θέλετε να λάβετε τον αριθμό σελίδων. |

---

## GetPageCount (7 of 7) {#getpagecount_7}

Επιστρέφει τον αριθμό σελίδων για το έργο που θα αποδοθεί χρησιμοποιώντας το δεδομένο Timescale.

**Returns:** Page count to be rendered.

```cpp
GetPageCount(Visualization::Timescale scale)
```

| Παράμετρος | Περιγραφή |
| --- | --- |
| scale | Η κλίμακα για την οποία θέλετε να λάβετε τον αριθμό σελίδων. |

