# E-Course Registration Forecasting and Autoscaling

A plan for using time-series forecasting to scale cloud servers before UiTM's course registration peak, so the registration system stays reachable.

## Problem statement

UiTM students must register for their courses online within a short announced window. Every semester, the e-course registration system becomes slow or inaccessible when many students log in at the same time, and students often cannot even open the registration page. Some students wait up to about three days before they can register successfully. This delays registration, risks losing seats in required courses, and forces students to keep retrying.

## Documents

- [Problem statement](docs/problem-statement.md)
- [Requirements](docs/requirements.md)
- [User stories](docs/user-stories.md)
- [Sprint log](docs/sprint-log.md)
- [Technology notes](docs/technology-notes.md) 

## Project structure

- README.md: project summary and links
- LICENSE: MIT licence
- .gitignore: files Git must not track
- docs/: problem statement, requirements, user stories and sprint log
- src/: place for source code (empty for now)

## Roadmap

- [x] Problem statement, requirements and user stories
- [x] Acceptance criteria and numbered requirements
- [x] Evidence for the problem statement
- [x] Technology notes: machine learning time-series forecasting, with 3 sources
- [x] Outline of the technology explanation

## Status

Work in progress for CSC649 Assignment 1.

## Author

Hafizul Rahman, UiTM