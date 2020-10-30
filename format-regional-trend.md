# Regional trend data

## Data update
- Every Monday at 5 pm (UTC).

## Data format

**Reference file:** andamento-settimanale-dati-regionali.csv<br>
**Reference file with latest data:**: andamento-settimanale-dati-regionali-latest.csv<br>

| Field name                  | Description (ITA)                       | Description                            | Format                       | Example             |
|-----------------------------|-----------------------------------|----------------------------------------|-------------------------------|---------------------|
| **settimana**                        | primo giorno della settimana di riferimento. La settimana inizia il lunedì.            | first day of the reference week. Week starts on Monday.                   | YYYY-MM-DD HH:MM:SS | 2020-06-01 00:00:00 |
| **denominazione_regione**                       | denominazione della Regione | name of the Region           |  string     |         Abruzzo         |
| **codice_regione**              | codice della regione (ISTAT 2019) | code of the region (ISTAT 2019)                        | number      | 13            |
| **lat**       | latitudine       | latitude                     | WGS84             | 42.4564388275            |
| **long**                         | longitudine    | longitude         | WGS84                         | 13.871007974999998          |
| **notifiche_inviate**  | numero di notifiche inviate nella settimana di riferimento*    | number of notifications sent in the reference week*     | number                         | 3         |
| **utenti_positivi**      | numero di utenti positivi che hanno caricato le proprie chiavi nella settimana di riferimento*   | number of positive users who uploaded their keys in the reference week*   | number                        | 3                   |
|
These data are also available in a json format.
<br>

\*If this value is negative (-1), the number of notifications or positive users is less than or equal to 5.

### Note
Please note:
* The number of positive users is the number of users who have uploaded their keys.

* The number of notifications is the number of notifications of possible risk exposure generated by the application. The detection is partial since all notifications for iOS devices are detected and only a third of those sent by Android that have the necessary technology available to detect them safely.

* Latitude and longitude are calculated as the average of the latitudes and longitudes of the provincial capitals of that region.