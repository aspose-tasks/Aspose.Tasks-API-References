---
title: "TimeDelta"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Représente une différence entre deux horodatages."
type: docs
weight: 317
url: /fr/java/com.aspose.tasks/timedelta/
---

**Inheritance:**
java.lang.Object
```
public class TimeDelta
```

Représente une différence entre deux horodatages.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [TimeDelta(int hours, int minutes, int seconds)](#TimeDelta-int-int-int-) | Initialise une nouvelle instance de TimeDelta avec le nombre spécifié d'heures, de minutes et de secondes. |
| [TimeDelta(int days, int hours, int minutes, int seconds, int milliseconds)](#TimeDelta-int-int-int-int-int-) | Initialise une nouvelle instance de TimeDelta avec le nombre spécifié de jours, d'heures, de minutes, de secondes et de millisecondes. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [add(TimeDelta other)](#add-com.aspose.tasks.TimeDelta-) | Renvoie un nouvel objet TimeDelta dont la valeur est la somme de cette instance et d'une autre. |
| [clone()](#clone--) | \{@inheritDoc\} |
| [compare(TimeDelta t1, TimeDelta t2)](#compare-com.aspose.tasks.TimeDelta-com.aspose.tasks.TimeDelta-) | Compare deux valeurs TimeDelta et renvoie un entier indiquant si la première valeur est plus courte, égale ou plus longue que la deuxième valeur. |
| [compareTo(TimeDelta other)](#compareTo-com.aspose.tasks.TimeDelta-) | Compare cette instance à un objet TimeDelta spécifié et renvoie un entier indiquant si cette instance est plus courte, égale ou plus longue que l'objet TimeSpan. |
| [equals(TimeDelta other)](#equals-com.aspose.tasks.TimeDelta-) | Indique si un certain intervalle de temps `other` est égal à celui-ci. |
| [equals(TimeDelta t1, TimeDelta t2)](#equals-com.aspose.tasks.TimeDelta-com.aspose.tasks.TimeDelta-) | Vérifie l'égalité de deux instances. |
| [equals(Object other)](#equals-java.lang.Object-) | \{@inheritDoc\} |
| [fromDays(double value)](#fromDays-double-) | Renvoie un TimeDelta qui représente un nombre spécifié de jours (arrondi à la milliseconde la plus proche). |
| [fromHours(double value)](#fromHours-double-) | Renvoie un TimeDelta qui représente un nombre spécifié d'heures (arrondi à la milliseconde la plus proche). |
| [fromMilliseconds(double value)](#fromMilliseconds-double-) | Renvoie un TimeDelta qui représente un nombre spécifié de millisecondes (arrondi à la milliseconde la plus proche). |
| [fromMinutes(double value)](#fromMinutes-double-) | Renvoie un TimeDelta qui représente un nombre spécifié de minutes (arrondi à la milliseconde la plus proche). |
| [fromSeconds(double value)](#fromSeconds-double-) | Renvoie un TimeDelta qui représente un nombre spécifié de secondes (arrondi à la milliseconde la plus proche). |
| [getDays()](#getDays--) | Renvoie le composant jours de l'intervalle de temps, représenté par cette instance. |
| [getHours()](#getHours--) | Renvoie le composant heures de l'intervalle de temps, représenté par cette instance. |
| [getMilliseconds()](#getMilliseconds--) | Renvoie le composant millisecondes de l'intervalle de temps, représenté par cette instance. |
| [getMinutes()](#getMinutes--) | Renvoie le composant minutes de l'intervalle de temps, représenté par cette instance. |
| [getSeconds()](#getSeconds--) | Renvoie le composant secondes de l'intervalle de temps, représenté par cette instance. |
| [getTotalDays()](#getTotalDays--) | Renvoie la valeur de l'instance actuelle exprimée en jours entiers et fractionnaires. |
| [getTotalHours()](#getTotalHours--) | Renvoie la valeur de l'instance actuelle exprimée en heures entières et fractionnaires. |
| [getTotalMilliseconds()](#getTotalMilliseconds--) | Renvoie la valeur de l'instance actuelle exprimée en millisecondes entières et fractionnaires. |
| [getTotalMinutes()](#getTotalMinutes--) | Renvoie la valeur de l'instance actuelle exprimée en minutes entières et fractionnaires. |
| [getTotalSeconds()](#getTotalSeconds--) | Renvoie la valeur de l'instance actuelle exprimée en secondes entières et fractionnaires. |
| [hashCode()](#hashCode--) | \{@inheritDoc\} |
| [negate()](#negate--) | Renvoie un nouveau `TimeDelta` dont la valeur est la valeur négative de cette instance. |
| [parse(String s)](#parse-java.lang.String-) | Convertit la représentation sous forme de chaîne d'un intervalle de temps en son équivalent `TimeDelta`. |
| [subtract(TimeDelta other)](#subtract-com.aspose.tasks.TimeDelta-) | Renvoie un nouvel objet TimeDelta dont la valeur est la différence entre cette instance et les instances `other`. |
| [toString()](#toString--) | \{@inheritDoc\} |
| [tryParse(String s, TimeDelta[] result)](#tryParse-java.lang.String-com.aspose.tasks.TimeDelta---) | Convertit la représentation sous forme de chaîne d'un intervalle de temps en son équivalent TimeDelta et renvoie une valeur indiquant si la conversion a réussi. |
### TimeDelta(int hours, int minutes, int seconds) {#TimeDelta-int-int-int-}
```
public TimeDelta(int hours, int minutes, int seconds)
```


Initialise une nouvelle instance de TimeDelta avec le nombre spécifié d'heures, de minutes et de secondes.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| heures | int | nombre d'heures. |
| minutes | int | nombre de minutes. |
| secondes | int | nombre de secondes. |

### TimeDelta(int days, int hours, int minutes, int seconds, int milliseconds) {#TimeDelta-int-int-int-int-int-}
```
public TimeDelta(int days, int hours, int minutes, int seconds, int milliseconds)
```


Initialise une nouvelle instance de TimeDelta avec le nombre spécifié de jours, d'heures, de minutes, de secondes et de millisecondes.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| jours | int | nombre de jours. |
| heures | int | nombre d'heures. |
| minutes | int | nombre de minutes. |
| secondes | int | nombre de secondes. |
| millisecondes | int | nombre de millisecondes. |

### add(TimeDelta other) {#add-com.aspose.tasks.TimeDelta-}
```
public TimeDelta add(TimeDelta other)
```


Renvoie un nouvel objet TimeDelta dont la valeur est la somme de cette instance et d'une autre.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| other | [TimeDelta](../../com.aspose.tasks/timedelta) | l'instance à additionner. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - a new object that represents the value of this instance plus value of other instance.
### clone() {#clone--}
```
public Object clone()
```




**Returns:**
java.lang.Object - \{@inheritDoc\}
### compare(TimeDelta t1, TimeDelta t2) {#compare-com.aspose.tasks.TimeDelta-com.aspose.tasks.TimeDelta-}
```
public static int compare(TimeDelta t1, TimeDelta t2)
```


Compare deux valeurs TimeDelta et renvoie un entier indiquant si la première valeur est plus courte, égale ou plus longue que la deuxième valeur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| t1 | [TimeDelta](../../com.aspose.tasks/timedelta) | le premier intervalle de temps à comparer. |
| t2 | [TimeDelta](../../com.aspose.tasks/timedelta) | le deuxième intervalle de temps à comparer. |

**Returns:**
int - \-1 si `t1` est plus court que `t2`, 0 si `t1` est égal à `t2` et 1 si `t1` est plus long que `t2`.
### compareTo(TimeDelta other) {#compareTo-com.aspose.tasks.TimeDelta-}
```
public int compareTo(TimeDelta other)
```


Compare cette instance à un objet TimeDelta spécifié et renvoie un entier indiquant si cette instance est plus courte, égale ou plus longue que l'objet TimeSpan.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| other | [TimeDelta](../../com.aspose.tasks/timedelta) | une instance à comparer. |

**Returns:**
int - \-1 si cette instance est plus courte que `other`, 0 si cette instance est égale à `other` et 1 si cette instance est plus longue que `other`.
### equals(TimeDelta other) {#equals-com.aspose.tasks.TimeDelta-}
```
public boolean equals(TimeDelta other)
```


Indique si un certain intervalle de temps `other` est égal à celui-ci.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| other | [TimeDelta](../../com.aspose.tasks/timedelta) | intervalle de temps à comparer. |

**Returns:**
booléen - `true` si les intervalles sont égaux ; `false` sinon.
### equals(TimeDelta t1, TimeDelta t2) {#equals-com.aspose.tasks.TimeDelta-com.aspose.tasks.TimeDelta-}
```
public static boolean equals(TimeDelta t1, TimeDelta t2)
```


Vérifie l'égalité de deux instances.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| t1 | [TimeDelta](../../com.aspose.tasks/timedelta) | première instance. |
| t2 | [TimeDelta](../../com.aspose.tasks/timedelta) | deuxième instance. |

**Returns:**
booléen - `true` si les instances sont égales ; `false` sinon.
### equals(Object other) {#equals-java.lang.Object-}
```
public boolean equals(Object other)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| autre | java.lang.Object | \{@inheritDoc\} |

**Returns:**
booléen - \{@inheritDoc\}
### fromDays(double value) {#fromDays-double-}
```
public static TimeDelta fromDays(double value)
```


Renvoie un TimeDelta qui représente un nombre spécifié de jours (arrondi à la milliseconde la plus proche).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double | un nombre de jours. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### fromHours(double value) {#fromHours-double-}
```
public static TimeDelta fromHours(double value)
```


Renvoie un TimeDelta qui représente un nombre spécifié d'heures (arrondi à la milliseconde la plus proche).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double | un nombre d'heures. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### fromMilliseconds(double value) {#fromMilliseconds-double-}
```
public static TimeDelta fromMilliseconds(double value)
```


Renvoie un TimeDelta qui représente un nombre spécifié de millisecondes (arrondi à la milliseconde la plus proche).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double | un nombre de millisecondes. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### fromMinutes(double value) {#fromMinutes-double-}
```
public static TimeDelta fromMinutes(double value)
```


Renvoie un TimeDelta qui représente un nombre spécifié de minutes (arrondi à la milliseconde la plus proche).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double | un nombre de minutes. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### fromSeconds(double value) {#fromSeconds-double-}
```
public static TimeDelta fromSeconds(double value)
```


Renvoie un TimeDelta qui représente un nombre spécifié de secondes (arrondi à la milliseconde la plus proche).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double | un nombre de secondes. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### getDays() {#getDays--}
```
public int getDays()
```


Renvoie le composant jours de l'intervalle de temps, représenté par cette instance.

**Returns:**
int - le composant jours de l'intervalle de temps. Peut être positif ou négatif.
### getHours() {#getHours--}
```
public int getHours()
```


Renvoie le composant heures de l'intervalle de temps, représenté par cette instance.

**Returns:**
int - le composant heures de l'intervalle de temps, compris entre -23 et 23.
### getMilliseconds() {#getMilliseconds--}
```
public int getMilliseconds()
```


Renvoie le composant millisecondes de l'intervalle de temps, représenté par cette instance.

**Returns:**
int - le composant millisecondes de l'intervalle de temps, compris entre -999 et 999.
### getMinutes() {#getMinutes--}
```
public int getMinutes()
```


Renvoie le composant minutes de l'intervalle de temps, représenté par cette instance.

**Returns:**
int - le composant minutes de l'intervalle de temps compris entre -59 et 59.
### getSeconds() {#getSeconds--}
```
public int getSeconds()
```


Renvoie le composant secondes de l'intervalle de temps, représenté par cette instance.

**Returns:**
int - le composant secondes de l'intervalle de temps compris entre -59 et 59.
### getTotalDays() {#getTotalDays--}
```
public double getTotalDays()
```


Renvoie la valeur de l'instance actuelle exprimée en jours entiers et fractionnaires.

**Returns:**
double - le nombre total de jours représenté par cette instance.
### getTotalHours() {#getTotalHours--}
```
public double getTotalHours()
```


Renvoie la valeur de l'instance actuelle exprimée en heures entières et fractionnaires.

**Returns:**
double - le nombre total d'heures représenté par cette instance.
### getTotalMilliseconds() {#getTotalMilliseconds--}
```
public double getTotalMilliseconds()
```


Renvoie la valeur de l'instance actuelle exprimée en millisecondes entières et fractionnaires.

**Returns:**
double - le nombre total de millisecondes représenté par cette instance.
### getTotalMinutes() {#getTotalMinutes--}
```
public double getTotalMinutes()
```


Renvoie la valeur de l'instance actuelle exprimée en minutes entières et fractionnaires.

**Returns:**
double - le nombre total de minutes représenté par cette instance.
### getTotalSeconds() {#getTotalSeconds--}
```
public double getTotalSeconds()
```


Renvoie la valeur de l'instance actuelle exprimée en secondes entières et fractionnaires.

**Returns:**
double - le nombre total de secondes représenté par cette instance.
### hashCode() {#hashCode--}
```
public int hashCode()
```




**Returns:**
int - \{@inheritDoc\}
### negate() {#negate--}
```
public TimeDelta negate()
```


Renvoie un nouveau `TimeDelta` dont la valeur est la valeur négative de cette instance.

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - A new object with the same numeric value as this instance, but with the opposite sign.
### parse(String s) {#parse-java.lang.String-}
```
public static TimeDelta parse(String s)
```


Convertit la représentation sous forme de chaîne d'un intervalle de temps en son équivalent `TimeDelta`.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| s | java.lang.String | une chaîne qui spécifie l'intervalle de temps à convertir. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - a time interval that corresponds to `s`.
### subtract(TimeDelta other) {#subtract-com.aspose.tasks.TimeDelta-}
```
public TimeDelta subtract(TimeDelta other)
```


Renvoie un nouvel objet TimeDelta dont la valeur est la différence entre cette instance et les instances `other`.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| other | [TimeDelta](../../com.aspose.tasks/timedelta) | l'instance à soustraire. |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - a new object that represents the value of this instance minus value of other instance.
### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String - \{@inheritDoc\}
### tryParse(String s, TimeDelta[] result) {#tryParse-java.lang.String-com.aspose.tasks.TimeDelta---}
```
public static boolean tryParse(String s, TimeDelta[] result)
```


Convertit la représentation sous forme de chaîne d'un intervalle de temps en son équivalent TimeDelta et renvoie une valeur indiquant si la conversion a réussi.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| s | java.lang.String | une chaîne qui spécifie l'intervalle de temps à convertir. |
| result | [TimeDelta\[\]](../../com.aspose.tasks/timedelta) | ce tableau doit contenir au moins un élément. Lorsque cette méthode retourne, `result[0]` contient un objet qui représente l'intervalle de temps spécifié par `s`, ou un intervalle de temps de longueur zéro si la conversion a échoué. |

**Returns:**
boolean - `true` si s a été converti avec succès ; sinon, `false`.
