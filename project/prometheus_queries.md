## Availability SLI
### The percentage of successful requests over the last 5m
(increase(flask_http_request_total{status="200"}[5m])) / on() group_right() (sum(increase(flask_http_request_total[5m])))

## Latency SLI
### 90% of requests finish in these times
increase(
  flask_http_request_duration_seconds_bucket{status="200",le="0.1"}[5m]
)
 / ignoring (le)
increase(
  flask_http_request_duration_seconds_count{status="200"}[5m]
)

## Throughput
### Successful requests per second
rate(flask_http_request_duration_seconds_count{status="200"}[5m])

## Error Budget - Remaining Error Budget
### The error budget is 20%
sum(flask_http_request_total{status!="200"})  / on() group_right() (sum(flask_http_request_total))

