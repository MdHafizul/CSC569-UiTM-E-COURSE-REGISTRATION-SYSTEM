# User Stories

These user stories describe the main users of the forecasting and autoscaling support system.

## US1: Accessible registration page
US1: Supports: FR5, NFR1
As a student, I want the registration page to stay accessible when everyone registers at once, so that I can register on the first day without repeated retries.

Acceptance criteria:
1. During a simulated peak at the forecast peak load, the page loads in under 3 seconds for 95% of requests.
2. At least 95% of registration submissions succeed on the first attempt.

## US2: Forecast before the registration window
US2: Supports: FR2, FR3
As a system administrator, I want a forecast of expected users before the registration window, so that I can plan server capacity in advance.

Acceptance criteria:
1. The dashboard shows an hourly forecast for the next 7 days.
2. Changing the registration start date updates the forecast.

## US3: Scale down after the peak
US3: Supports: FR6, NFR5
As a university IT manager, I want servers to scale down automatically after the peak, so that cloud cost stays low outside registration periods.

Acceptance criteria:
1. Extra instances are removed after load stays below the off-peak level for 60 minutes.
2. Idle capacity outside the registration window is no more than 25% of peak capacity.