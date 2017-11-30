## hijri

hijri is a small helper library to convert a Hijri date to a Gregorian date according to Ummul Qura calendar.

It just exports one function `HijriToGregorian` which takes a Hijri `year`, `month`
and a `day` and return the equivalent Gregorian date based on based on Ummul Qura [موقع تقويم أم القرى](http://www.ummulqura.org.sa/) calendar.

Please note the Islamic (Hijri) calendar system is a lunar calendar based on observation. 
The observation aspect of the calendar means that a new month can only be declared based on human observations of the moon, 
something which can obviously vary and is unsuited to computer calculation.

# Install

```go 
go get github.com/younisshah/hijri
```


# Usage

```go
gregorianDate, err := hijri.HijriToGregorian(1439, 3, 12)
// ... err handling
// gregorianDate.String() -> 2017-11-30 00:00:00 +0000 UTC
```

# License

MIT