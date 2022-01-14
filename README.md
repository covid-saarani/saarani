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
