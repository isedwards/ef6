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
- Array vs List
- [IQueryable vs IEnumerable](https://stackoverflow.com/a/2876655/), including notes on paging with [Take](https://msdn.microsoft.com/en-us/library/bb300906.aspx?f=255&MSPPError=-2147217396) and [Skip](https://msdn.microsoft.com/en-us/library/bb357513.aspx) (see also [diagram](https://stackoverflow.com/a/40013006/)). Testing that an [object implements an interface](https://stackoverflow.com/questions/1360267/test-if-an-object-implements-an-interface) doesn't guarented that [extension methods will be available](https://stackoverflow.com/questions/48475363/missingmemberexception-when-using-callbyname).
- DataSource vs BindingSource
- Interfaces (vs Duck Typing and ABCs)
- "[Unable to convert MySQL date/time value to System.DateTime](https://stackoverflow.com/a/5758638/)"

- Replace `Chr(34) &` string concatenation with escaped quotes (`"""`), StringBuilder and String.Format. Also check whether using [+ or &](https://stackoverflow.com/questions/734600/the-difference-between-and-for-joining-strings-in-vb-net) for concatenation.
