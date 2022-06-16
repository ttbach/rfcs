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

# Add Typescript to Ember Guides

## Summary

Now that Typescript is a supported language in Ember, we need to figure out a way to surface documentation for adoption and usage.

## Motivation

Currently, the only documentation we have for Typescript in Ember exists in a [separate site](https://docs.ember-cli-typescript.com/). This is not ideal because
it's hard to find the TS doc because it's not linked anywhere and also not ideal to have separate sites for Ember resources.

## Detailed design

> Explain the design in enough detail for somebody
familiar with the framework to understand, and for somebody familiar with the
implementation to implement. This should get into specifics and corner-cases,
and include examples of how the feature is used. Any new terminology should be
defined here.

At a high level, we need to incorporate explanatory information from https://docs.ember-cli-typescript.com/ in the Ember guides.

Outline:
1. Draw out proposal for what [the component state and actions page](https://guides.emberjs.com/release/components/component-state-and-actions/) would look like with the changes
2. Include code samples of a toggle component that can switch between JS and TS, where the JS part is compiled from TS. Once selected, all examples will be in that
language (default to JS). Example: https://firebase.google.com/docs/firestore/manage-data/add-data. Alternatively, if we want a less pronounced experience, we
can add a TS checkbox instead of a TS tab.
3. List out the explanatory texts that can be incorporated into Ember guides
4. Examples can be toggled between TS and JS, with JS being compiled from TS, so
it reduces maintenance cost.

## How we teach this

Not sure if this section is necessary

## Drawbacks

Adding Typescript documentation means added maintenance effort on:
- Keeping documentation up to date for both JS and TS
- Potential learning curve for people who want to make changes to TS examples.

In the past year, there have been 11 commits that modify
code samples.

Commit list:
1. 5/25/22 https://github.com/ember-learn/guides-source/pull/1708 - tutorial update
2. 4/8/22 https://github.com/ember-learn/guides-source/pull/1821 - fix ember data call code sample
3. 12/6/21 https://github.com/ember-learn/guides-source/pull/1758 - fix looping example
4. 12/4/21 https://github.com/ember-learn/guides-source/pull/1751 - fix backing class
5. 11/5/21 https://github.com/ember-learn/guides-source/pull/1747 - make code more accessible
6. 11/4/21 https://github.com/ember-learn/guides-source/pull/1734 - remove willTransition references
7. 9/1/21 https://github.com/ember-learn/guides-source/pull/1729 - remove @id from built in Ember components
8. 8/31/21 https://github.com/ember-learn/guides-source/pull/1725 - add class based examples
9. 8/31/21 https://github.com/ember-learn/guides-source/pull/1724 - update class based examples
10. 8/31/21 https://github.com/ember-learn/guides-source/pull/1715 - injection in native classes
11. 7/21/21 https://github.com/ember-learn/guides-source/pull/1705 - fix glimmer code

## Alternatives

> What other designs have been considered? What is the impact of not doing this?

> This section could also include prior art, that is, how other frameworks in the same domain have solved this problem.

## Unresolved questions

> Optional, but suggested for first drafts. What parts of the design are still
TBD?
