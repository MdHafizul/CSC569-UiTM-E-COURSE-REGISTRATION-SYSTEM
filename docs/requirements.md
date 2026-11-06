# Requirements

In this document, the system means the forecasting and autoscaling support system that sits beside the existing registration portal.

## Functional requirements
- The system shall collect concurrent-user and request-count data from the registration portal at intervals of no more than 5 minutes.
- The system shall forecast the expected number of concurrent users for each hour of the next 7 days.
- The system shall accept the registration window start and end dates as input to the forecast.
- The system shall convert the forecast into a recommended number of server instances.
- The system shall start additional server instances at least 30 minutes before a forecast peak.
- The system shall remove extra server instances when actual load stays below the off-peak level for 60 minutes.
- The system shall display forecast load and actual load on one administrator dashboard.
- The system shall alert administrators when actual load exceeds the forecast by more than 20%.

## Non-functional requirements
- Performance: The registration page shall load in under 3 seconds for 95% of requests at the forecast peak load.
- Accuracy: The forecast shall have a mean absolute percentage error (MAPE) of 20% or less on a held-out test period.
- Availability: The registration portal shall be available at least 99.5% of the time during the registration window.
- Security and privacy: The system shall use only anonymised traffic counts (no student personal data), and all data in transit shall use TLS 1.2 or higher.
- Cost: Idle capacity outside the registration window shall be no more than 25% of peak capacity.