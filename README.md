# testing-in-go

Tutorial repo for Testing in Go talk.

## Logs

Three different types of log entries.

#### Lagacy

```
Wed Aug 28 18:30:10 +0000 2014: Something went a little wrong :)
```

  * Plain text
  * Assume `Info`
  * time.Parse layout: `time.RubyDate`

#### Live

```
3:04PM,INF,not sure what's up here?
```

  * CSV?
  * Assume today
  * `INF`, `ERR` and `WRN`
  * time.Parse layout: `time.Kitchen`

#### New

```
{"when":"2014-08-26T18:30:01.000000002Z","type":"Info","message":"This is the log message"}
```

  * JSON format
  * `Info`, `Error` or `Warning`
  * time.Parse layout: `time.RFC3339Nano`
