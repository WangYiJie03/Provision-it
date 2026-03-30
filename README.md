<h1 align="center">
  <img src="frontend/Icons/pvit90.png" width="150px"/><br/>
  Provision-IT – Backend Service (Team Project Showcase)
</h1>

## My Contributions

This project was developed as part of a team of 5.

My main contributions included:

- Designed and implemented RESTful backend APIs for portfolio aggregation and transaction history queries
- Built PostgreSQL schema and data models to support historical asset valuation tracking and audit-safe updates
- Developed backend service logic using Flask and SQLAlchemy
- Contributed to integration testing and collaborated in Agile team workflows, including pull request reviews and sprint stand-ups

## Project Overview

Provision-IT is a fractional asset ownership platform that allows users to
browse assets, purchase fractions, manage portfolios, and track asset value
history.

The backend service is built with Flask and PostgreSQL, exposing RESTful APIs
to support authentication, asset management, trading, and portfolio operations.

## Detailed Contribution Breakdown

I worked as a backend-focused developer in this client-based Agile project, with responsibilities spanning
database design, API development, and frontend-backend integration.

### Backend & Database Design
- Contributed to early system design decisions around fractional asset modelling, proposing a fixed-unit
  fraction approach (instead of percentage-based ownership) to simplify valuation, aggregation, and
  transaction consistency.
- Designed and implemented the AssetValueHistory table to support historical valuation tracking and
  manual price adjustments by administrators, including audit fields such as timestamp, source,
  adjusted_by, and adjustment_reason.

### API Development & Business Logic
- Implemented RESTful APIs using Flask and SQLAlchemy to support asset valuation history queries and
  administrator price updates.
- Built read-only portfolio APIs for user holdings and transaction history:
  - `GET /users/<user_id>/fractions/owning` to aggregate user holdings by asset, including latest value and
    estimated portfolio value.
  - `GET /users/<user_id>/transactions` with asset filtering and pagination, returning transactions in
    reverse chronological order.
- Implemented backend service logic for valuation calculations, transaction aggregation, and structured
  JSON responses for frontend consumption.

### Frontend Integration & Testing
- Integrated backend APIs with frontend HTML/JavaScript pages to display asset valuation history,
  user holdings, and transaction records.
- Wrote and executed integration tests using pytest to validate API correctness and data consistency.
- Assisted with local environment setup, database initialization, and data import workflows
  (init_db_postgres.py, environment configuration, and troubleshooting).

### Collaboration & Engineering Practices
- Actively participated in Agile workflows including sprint planning, stand-ups, pull requests, and
  code reviews.
- Submitted pull requests with detailed descriptions and responded quickly to feedback, fixing issues
  during integration testing on the same day.
- Contributed to project documentation by adding setup notes, common errors, and troubleshooting
  guidance to improve developer onboarding.


## Tech Stack

- **Backend:** Python, Flask, SQLAlchemy
- **Database:** PostgreSQL
- **Testing:** pytest
- **Tools:** Git, GitHub, Agile workflow

## Repository Note

This repository contains my showcase version of a University of Melbourne client-based Agile team project. The original team delivery repository is available here: [Provision-it Team Repository](https://github.com/Evelyn-0yi/Provision-it)
