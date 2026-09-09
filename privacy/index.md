# Community OS Privacy Policy

Last updated: 2026-09-09

Community OS is a Reddit Devvit app that helps subreddit moderators understand community health, recognize contributors, manage recurring community programs, rescue unanswered posts, and generate weekly community intelligence.

## Data Community OS processes

Community OS processes only the Reddit information needed to provide its features.

For contribution tracking, it may store:

- Reddit username
- Reddit post or comment ID
- whether the contribution was a post or comment
- limited scoring input used for contributor recognition
- contribution timestamp
- rolling contributor counters and point totals

For the unanswered-post queue, it may temporarily store:

- Reddit post ID
- post title
- permalink
- creation time

Community OS also stores app settings, recurring-program definitions, health snapshots, and duplicate-run markers.

## Data Community OS does not store

Community OS does not intentionally store:

- comment bodies
- post bodies
- email addresses
- real names
- profile images
- Reddit user flair
- external account data
- advertising profiles
- sensitive-trait inferences

## How data is used

Stored data is used only to operate Community OS features, including:

- calculating directional community-health signals
- identifying unanswered posts
- measuring contributor activity and return
- generating contributor-recognition rankings
- generating moderator recommendations
- operating recurring programs
- generating weekly community-intelligence reports
- preventing duplicate automated posts

Community OS does not use Reddit data for advertising, model training, or sale of user data.

## Storage

In the current version, Community OS stores Reddit data only in installation-scoped Devvit Redis.

Community OS does not send Reddit user data to an external database, analytics service, advertising service, or third-party API.

## Retention

Contribution-event metadata is retained for no more than 30 days.

Derived contributor profiles are rebuilt from the remaining rolling data as older events expire.

Operational app settings and configuration data may remain for as long as the app installation exists.

## Deleted Reddit content

When Community OS receives supported Reddit post or comment deletion events, it removes the corresponding contribution event from its stored dataset and rebuilds the affected contributor profile.

## Moderator privacy purge

Moderators can use the Community OS privacy purge control to remove tracked Community OS contributor metadata for a Reddit username.

Community OS also performs a rotating account-availability check and removes tracked contributor data for accounts detected as unavailable.

## Data sharing

Community OS does not sell Reddit data.

Community OS does not share stored Reddit user data with advertisers or external data brokers.

Data remains within the Reddit Devvit environment for the installed app in the current version.

## Public dashboard information

Community OS includes a public read-only dashboard view. Information intentionally displayed by the app, such as aggregate community-health metrics or contributor-recognition information, may therefore be visible to Reddit users viewing that dashboard or an explicitly published Community OS report.

Moderator controls remain restricted to moderators.

## Security and access

Community OS uses Reddit moderator verification for mutation endpoints and Redis transaction and duplicate-lock protections for relevant operations.

No software can guarantee absolute security, but Community OS is designed to minimize the amount of Reddit user data it stores and the length of time contribution-event data is retained.

## Changes to this policy

This policy may be updated when Community OS features or data practices change. The date at the top of this document will be updated when material changes are made.

## Contact

For questions, privacy requests, or support related to Community OS, contact the developer on Reddit:

`u/weknowthe_`

Community OS is an independent Devvit app and is not an official Reddit product.
