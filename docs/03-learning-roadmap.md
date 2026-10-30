# Learning Roadmap and Coaching Plan

## Guidance model
This project should be developed as a guided learning journey, similar in spirit to Microsoft Learn:
- each step has a clear objective
- each step produces a visible result
- each step builds on the previous one
- errors are treated as part of the learning process

## Phase 1 — Project bootstrap
Goals:
- create the .NET 10 solution
- create the Blazor Web App project
- verify the app launches locally
- understand the default project structure

Deliverables:
- working app shell
- navigation layout
- initial pages

## Phase 2 — Domain model and app concepts
Goals:
- define the core entities of the product
- describe the learning and event model clearly
- decide how progress, badge and challenge data will be represented

Core concepts:
- `Course`
- `Module`
- `Lesson`
- `UserProgress`
- `Achievement`
- `Badge`
- `Challenge`
- `Speaker`
- `EventUpdate`

Deliverables:
- domain model definition
- initial DTOs or entities
- data model conventions

## Phase 3 — Core UI pages
Goals:
- build the primary experience
- create the landing page and main navigation
- create agenda, passport, challenges and speaker pages

Deliverables:
- working screens for the main journey
- reusable cards, layouts and components
- readable event UX

## Phase 4 — Learning flow logic
Goals:
- model progress as a learning system
- allow a user to complete sessions or modules
- unlock achievements dynamically

Examples:
- attend a session
- complete a challenge
- finish a module
- unlock a badge

Deliverables:
- progress state logic
- achievement checks
- badge display and unlocking UI

## Phase 5 — Persistence with EF Core
Goals:
- map entities to a relational database
- create migrations
- seed demo data

Deliverables:
- working database access layer
- initial seed data for event content
- persistence for user progress

## Phase 6 — Authentication and personalization
Goals:
- add identity support
- allow per-user personalization
- bind progress and saved sessions to the logged-in user

Deliverables:
- login flow
- auth setup
- user-specific states

## Phase 7 — Polish, quality and demo readiness
Goals:
- refine the UI
- improve responsiveness
- verify the app flows are understandable
- prepare final demo narrative

Deliverables:
- stable demo flow
- clean design
- confident presentation story

## Demo flow for the final presentation
1. user lands on homepage
2. explores agenda
3. saves a session
4. sees progress update
5. completes a challenge
6. unlocks a badge
7. reaches summary Passport view

## Learning principle
The app will be developed in small, testable steps. We do not aim for a gigantic single build; we aim for a working, understandable learning experience that can be expanded iteratively.
