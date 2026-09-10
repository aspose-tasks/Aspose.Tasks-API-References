---
title: "CalendarException"
second_title: "Aspose.Tasks för Python via .NET API-referens"
description: 
type: docs
weight: 160
url: /sv/python-net/aspose.tasks/calendarexception/
---

## CalendarException class

Representerar exceptionella tidsperioder i en kalender.

CalendarException-typen visar följande medlemmar:
## Konstruktörer
| Namn | Beskrivning |
| :- | :- |
| CalendarException() | Initierar en ny instans av klassen [CalendarException](/tasks/python-net/aspose.tasks/calendarexception/). |
## Egenskaper
| Namn | Beskrivning |
| :- | :- |
| entered_by_occurrences | Hämtar eller anger ett värde som indikerar om återkommande intervallet definieras genom att ange ett antal förekomster.<br/>            False anger att intervallet definieras genom att ange ett slutdatum. |
| from_date | Hämtar eller anger början av undantagstiden. |
| to_date | Hämtar eller anger slutet av undantagstiden. |
| förekomster | Hämtar eller anger antalet förekomster som kalenderundantaget är giltigt för. |
| name | Hämtar eller anger namnet på undantaget. |
| type | Hämtar eller anger undantagstypen. |
| period | Hämtar eller anger återkommande period för undantaget. |
| days_of_week | Hämtar DayTypeCollection för detta objekt.<br/>            Veckodagarna då undantaget är giltigt. |
| month_item | Hämtar eller anger månadselementet för vilket ett undantagsåterkommande är schemalagt. |
| month_position | Hämtar eller anger positionen för ett månadselement inom en månad. |
| månad | Hämtar eller anger månaden för vilket ett undantagsåterkommande är schemalagt. |
| month_day | Hämtar eller anger dagen i en månad då ett undantagsåterkommande är schemalagt. |
| day_working | Hämtar eller anger ett värde som indikerar om det angivna datumet eller dagtypen är arbetsdag. |
| working_times | Hämtar eller anger WorkingTimeCollection-objektet.<br/>            Samlingen av arbetstider som definierar den arbetade tiden på veckodagen. |
| parent_calendar | Hämtar den överordnade kalendern för detta objekt. |
## Methods
| Namn | Beskrivning |
| :- | :- |
| delete() | Tar bort Exception-instansen från föräldrakalenderns CalendarExceptionCollection-objekt. |
| check_exception(dt) | Returnerar true om den angivna instansen av datetime‑strukturen är undantagsdagen. |
| get_working_time() | Returnerar arbetstiden för ett kalenderundantag. |
| get_exception_dates() | Returnerar datum då kalenderundantaget är tillämpligt. |

### Se även

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

