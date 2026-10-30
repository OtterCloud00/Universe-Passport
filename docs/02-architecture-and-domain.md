# Architecture and Domain Model

## Architecture direction
The project should be built as a Blazor Web App in .NET 10, with a clear separation between:
- UI layer
- domain / business logic
- persistence layer
- authentication layer

## Suggested app structure
- `UniversePassport.Web` – Blazor UI
- `UniversePassport.Application` – business services and use cases
- `UniversePassport.Domain` – entities and domain logic
- `UniversePassport.Infrastructure` – EF Core, data access, auth integration
- `UniversePassport.Tests` – unit and integration tests

## Core domain entities
### Course
A large learning unit or event journey.

### Module
A section inside a course or a learning track.

### Lesson
A single learning item: session, talk, workshop, or micro-learning unit.

### UserProgress
Tracks the current progress of a user for a specific module, lesson, or course.

### Achievement
A potential digital reward unlocked after a user meets a condition.

### Badge
A collectible or visual reward shown to the user after unlocking one or more achievements.

### Challenge
A task or quest, such as "Attend 3 sessions" or "Complete a workshop".

### Speaker
A speaker or presenter.

### EventUpdate
A live announcement or important update within the event.

## Example relationships
- User -> many UserProgress
- Course -> many Modules
- Module -> many Lessons
- Lesson -> many Speakers
- User -> many Achievements
- User -> many Challenges
- User -> many SavedSessions

## Data model philosophy
The app should model the experience as a progression system instead of a plain event calendar.

This means the app is not only storing agenda items but also:
- what a user has viewed
- what they have completed
- what they have unlocked
- what they are recommended to do next

## Blazor fit
Blazor is a good fit because the app is essentially a stateful, interactive learning dashboard:
- module cards
- progress bars
- challenge status
- personal passport
- event announcements
- filters and recommendations

## Recommended default data layer
- EF Core
- SQLite for local dev or PostgreSQL for production-like dev
- migrations for schema evolution

## Recommended auth pattern
- Identity for app users
- GitHub OAuth for a GitHub-native experience

## Recommended next-step principle
Build the domain model first, then the UI, then the data layer. This keeps the app coherent and avoids over-building components before the actual data model is ready.
