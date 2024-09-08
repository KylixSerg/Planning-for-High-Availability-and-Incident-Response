# API Service

| Category     | SLI                                                            | SLO                                                                                                         |
|--------------|----------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------|
| Availability | System is up 3.65 days at max per year or 14.4 minutes per day | 99%                                                                                                         |
| Latency      | Less than 100ms latency for 90% of incoming requests           | 90% of requests below 100ms                                                                                 |
| Error Budget | Less than 20% of requests are allowed to fail                  | Error budget is defined at 20%. This means that 20% of the requests can fail and still be within the budget |
| Throughput   | Minimum of 5RPS for the system to be healthy                   | 5 RPS indicates the application is functioning                                                              |
