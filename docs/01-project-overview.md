# Project Overview

## Project name
GitHub Universe 2026 — Universe Passport

## Current direction
This project has been re-oriented to a .NET 10 + Blazor Web App architecture.
The app is no longer planned as a Next.js event app; it is now intended to behave more like a guided learning platform inspired by Microsoft Learn.

## Vision
Universe Passport is a personalized event companion for GitHub Universe 2026. It helps attendees navigate the event program, track their learning journey, unlock digital badges, complete challenge quests, and stay informed with live announcements.

## Product idea
The application should feel like an event passport plus a learning path:
- a user follows the agenda as if it were a curriculum
- sessions are treated as learning modules
- completion and progress drive the experience
- achievements and badges create motivation
- event updates keep the user informed

## Core value proposition
- event discovery with a structured learning path
- progress tracking and achievement unlocking
- personalized experience for attendees
- strong GitHub identity and event branding
- feasible MVP in a modern .NET stack

## Final MVP scope
- Agenda with filters and search
- Saved sessions / favorites
- Passport with completion state and badges
- Challenge board with points
- Speaker spotlight
- Live updates / announcements

## User experience principle
The app should not feel like a generic scheduler. It should feel like a guided learning journey that rewards engagement and participation.

## Recommended stack
- Frontend: Blazor Web App
- Runtime: .NET 10
- Language: C#
- Styling: Tailwind CSS or custom CSS
- Persistence: EF Core + SQL Server or PostgreSQL
- Authentication: GitHub OAuth or Identity
- Hosting: Azure App Service or Azure Static Web Apps + App Service

## Key pages
- `/` — landing page and event countdown
- `/agenda` — schedule and filters
- `/passport` — personal progress and earned badges
- `/challenges` — quests and leaderboard
- `/speakers` — speaker spotlight
- `/updates` — live announcements
- `/profile` — saved items and stats

## Pitch statement
Universe Passport is a personalized learning and event companion for GitHub Universe 2026. It helps attendees follow the program, complete quests, unlock digital badges, and stay in sync with the event in a guided, motivating experience.

## Note on legacy documents
The repository previously contained a Next.js-oriented proposal. That document remains as historical context, but the active project direction is the .NET 10 + Blazor version described here.
