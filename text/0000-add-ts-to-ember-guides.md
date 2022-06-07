---
Stage: Accepted
Start Date:
Release Date: Unreleased
Release Versions:
  ember-source: vX.Y.Z
  ember-data: vX.Y.Z
Relevant Team(s): Ember Learn, Ember Typescript, Ember Franework
RFC PR:
---

<!---
Directions for above:

Stage: Leave as is
Start Date: Fill in with today's date, YYYY-MM-DD
Release Date: Leave as is
Release Versions: Leave as is
Relevant Team(s): Fill this in with the [team(s)](README.md#relevant-teams) to which this RFC applies
RFC PR: Fill this in with the URL for the Proposal RFC PR
-->

# <RFC title>

## Summary

Now that Typescript is a supported as a language in Ember, we need to figure
out a way to surface documentation for adoption and usage.

## Motivation

> Why are we doing this? What use cases does it support? What is the expected
outcome?
We need to add documentation in the following forms:
1. Merging [TS guides](https://docs.ember-cli-typescript.com/) into Ember guides
2. Adding TS

## Detailed design

> This is the bulk of the RFC.

> Explain the design in enough detail for somebody
familiar with the framework to understand, and for somebody familiar with the
implementation to implement. This should get into specifics and corner-cases,
and include examples of how the feature is used. Any new terminology should be
defined here.

Outline:
1. List out all sections on the TS docs that can be incorporated into Ember guides.
Pick the hardest section and then include an example of what that page could look
like.
2. Include code samples of a toggle component that can switch between JS and TS,
where the JS part is compiled from TS. Once selected, all examples will be in that
language (default to JS).
3. List out the explanatory texts that can be incorporated into Ember guides

Examples can be toggled between TS and JS, with JS being compiled from TS, so
it reduces maintenance cost.

## How we teach this

> What names and terminology work best for these concepts and why? How is this
idea best presented? As a continuation of existing Ember patterns, or as a
wholly new one?

> Would the acceptance of this proposal mean the Ember guides must be
re-organized or altered? Does it change how Ember is taught to new users
at any level?

> How should this feature be introduced and taught to existing Ember
users?

## Drawbacks

Adding Typescript documentation means added maintenance effort on:
- Keeping documentation up to date for both JS and TS
- Potential learning curve for people who want to make changes to TS examples.
This might be a small risk bc in the past 2 years, there are X commits to modify
examples (TODO: do research)

## Alternatives

> What other designs have been considered? What is the impact of not doing this?

> This section could also include prior art, that is, how other frameworks in the same domain have solved this problem.

## Unresolved questions

> Optional, but suggested for first drafts. What parts of the design are still
TBD?
