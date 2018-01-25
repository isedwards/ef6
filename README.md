This repository aims to provide a well-documented example of using Entity Framework 6 and LinQ for use in custom user controls for the Climsoft project developed in VisualBasic.NET

Initial tasks
- Develop examples simultaneously for a station selector and an element selector (connecting to db.stations and db.obselement)

Ability to perform following filters:
- equals "67774010"
- IN {"67774010", "67775050"}
- date greater #01/01/2001#

In addition, the ability to provide a extra customised columns from the select (e.g. the concatenation of id and name)

Further tasks
- Switch to stationelement. Only return those stations that can have data for the currently selected element(s), or only those elements available at the currently selected station(s)

NOTES:
- [IQueryable vs IEnumerable](https://stackoverflow.com/a/2876655/)
