# API Query Building Assignment
---

## USGS Earthquake Queries

### Query 1: [Magnitude 2.5-3.0]
**URL:**
```
https://earthquake.usgs.gov/fdsnws/event/1/query?format=geojson&minmagnitude=2.5&maxmagnitude=3.0
```

**Parameters used:**
- `format`: [Ensures the results are in json data]
- `minmagnitude=2.5`: [Takes all earthquakes with a magnitude of 2.5 or greater]
- `maxmagnitude=3.0`: [Takes all earthquakes with a magnitude of 3.0 or less]

**Result:** [Returned 507 earthquakes with a magnitude of 2.5-3.0]

---

### Query 2: [All earthquakes on May 22 2025]
**URL:**
```
[https://earthquake.usgs.gov/fdsnws/event/1/query?format=geojson&starttime=2025-05-22&endtime=2025-05-23]
```

**Parameters used:**
- `format`: [Ensures the results are in json data]
- `starttime=2025-05-22`: [Sets the minimum start time to May 22 2025]
- `endtime=2025-05-23`: [Sets the maximum start time to May 23 2025]

**Result:** [There were 303 earthquakes on May 22 2025]

---

### Query 3: [How many earthquakes with a magnitude of at least 5.0 have there been today]
**URL:**
```
[https://earthquake.usgs.gov/fdsnws/event/1/query?format=geojson&minmagnitude=5.0&starttime=2026-02-06]
```

**Parameters used:**
- `format`: [Ensures the results are in json data]
- `minmagnitude=5.0`: [Returns all earthquakes with a magnitude of at least 5.0]
- `starttime=2026-02-06`: [Returns all earthquakes on February 6 2026]

**Result:** [There have been 3 magnitude 5+ earthquakes today]

---

## Open Library Queries

### Query 4: [Return all books written by H. P. Lovecraft in english]
**URL:**
```
[https://openlibrary.org/search.json?author=h+p+lovecraft&language=eng]
```

**Parameters used:**
- `author=h+p+lovecraft`: [Returns all books written by H. P. Lovecraft]
- `language=eng`: [Returns all books written in english]

**Result:** [There are 1788 books written by H. P. Lovecraft in english] 


### Query 5: [How many history books have been made by Quan Millz?]
**URL:**
```
[https://openlibrary.org/search.json?author=quan+millz&subject=history]
```

**Parameters used:**
- `author=quan+millz`: [Return all books written by Quan Millz]
- `subject=history`: [Returns all books written about history]

**Result:** [There are 0 history books written by Quan Millz]

### Query 6: [How many Resident Evill books are in english?]
**URL:**
```
[https://openlibrary.org/search.json?q=resident+evil&language=eng]
```

**Parameters used:**
- `q=resident+evil`: [Returns all books about Resident Evil]
- `language=eng`: [Returns all books written in english]

**Result:** [There are 189 Resident Evil books written in english]