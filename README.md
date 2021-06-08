## OPS-DEV Alerts
| Hstack Alerts |
|---|
| Couchbase Alerts|

| :memo: Alert Name | :mag_right: What it does? | :bell: Severity | :clock9: Run period |
|---|---|---|---|
| Couchbase  data read failure  | Couchbase reported data read failure on instance for certain bucket bucket | :warning: Warning | 1m |
| Couchbase data read failure | Couchbase reported data read failure on instance for certain bucket bucket | :fire: Critical | 5m |
| Couchbase data write failure  | Couchbase reported data write failure on instance for certain bucket bucket | :fire: Critical | 5m |
| Couchbase data write failure | Couchbase reported data write failure on instance for certain bucket bucket | :warning: Warning | 1m |
| Couchbase item commit failure | Couchbase reported item commit failure on instance for certain bucket | :warning: Warning | 1m |
| Couchbase item commit failure | Couchbase reported item commit failure on instance for certain bucket | :fire: Critical | 5m |
| Couchbase misses | Couchbase reported {{ $value }} misses on {{ $labels.bucket }} in the last 5 minutes | :warning: Warning | 2m |
| Couchbase misses | Couchbase reported {{ $value }} misses on {{ $labels.bucket }} in the last 5 minutes | :fire: Critical | 5m |
| Couchbase unrecoverable OOMs | Couchbase reported {{ $value }} unrecoverable OOMs on {{ $labels.hostname }} for bucket {{ $labels.bucket }} | :fire: Critical | 5s |
| Couchbase used memory | Couchbase uses more than 80% memory on instance for a certain bucket | :fire: Critical | 5m |
| Couchbase used memory s| Couchbase uses more than 90% memory on instance for a certain bucket  | :warning: Warning  | 5m |
| Couchbase GC time | {{ $labels.hostname }} had GC running for more than 60 seconds in the last 5 minutes on couchbase JVM | :fire: Critical | 5m |
| Couchbase cluster disruption | Multiple couchbase nodes are down | :fire: Critical | 1m |
| Couchbase exporter down | Couchbase down on instance {{ $labels.instance }} | :warning: Warning | 1m |
| Couchbase exporter down | Couchbase down on instance {{ $labels.instance }} | :fire: Critical | 10m |
| Couchbase heap usage | {{ $labels.hostname }} had > 90% (current: {{ $value }}) heap usage for couchbase in the last 5 minutes | :fire: Critical | 5m |
| Couchbase incorrect target count | Expected 5 Couchbase, but found {{ $value }} | :fire: Critical | 1m |
