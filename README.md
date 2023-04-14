# Saarani (सारणी)

The main data is stored in this repo.

If you want to know more about Covid Saarani and how to fetch data,
see the [documentation](https://github.com/covid-saarani/documentation).

---

The latest data can be accessed using `latest.json`, which is a symlink.

Daily datewise data is stored in the `Daily` folder. The file is updated
hourly as the last fetched timestamps change, and can also get newer data.
So for a full list of intraday changes you might need to consult `git log`
for the file.

The pushing of data is done using a GitHub action, invoking a dedicated
program - the [लिपिक](https://github.com/covid-saarani/lipik).

---

## Note about some discrepancies

Had missed many 12-14 age group vaccination stats till Oct 2022 (Situation
improved and life went back to normal, so didn't really pay attention...
Apologies). This happened due to change / addition in PDF format and API keys
for vaccination, which I did not account in time.

Also, from Oct 2022 till 11th April 2023, there was a parsing error for 18+ 3rd
dose delta *if the primary source was MoHFW*. For data with primary source as
MyGov, which is most of the data, there would *not* be any problems.

***All other data can be relied upon.***

---
