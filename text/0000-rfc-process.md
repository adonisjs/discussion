- Feature Name: RFC Process
- Start Date: 2017-01-03
- RFC PR: (leave this empty)
- Rust Issue: (leave this empty)

# Summary
[summary]: #summary

This RFC recommends the RFC process and formal review process to be added to the adonis/discussion repo.

# Motivation
[motivation]: #motivation

This RFC process is inspired by the RFC process for Ember and Rust which aim to facilitate more open communication of framework progress and new features.
The RFC process is meant as a way to formalize the way new features are recommended, discussed, and added to the Adonis framework.
This is to help make it clearer who is working on what features and what new features are request and needed by the community.
The RFC process also helps aid in making sure that new APIs, tools, and changes are widely accepted by the community and push things forward in a positive direction with broad support.

The RFC process is also a way to help spread the load of maintaining Adonis as it grows and making sure that new features continue to be well understood, documented, and relevant.

This also is a way to better document and have one place for proposed features as now it is spread across DMs, Twitter, many different repo issues, and more.
The RFC process will give a good way of providing direct feedback to smaller parts of new features and get iterative changes to them.

# Detailed design
[design]: #detailed-design

The bulk of this RFC is rendered in the updates to the README as well as a template RFC markdown file.

[Updated Readme](https://github.com/rtablada/discussion/blob/rfc-implementation/README.md)
[Template for RFC](https://github.com/rtablada/discussion/blob/rfc-implementation/0000-template.md)

The RFC process is described below (as copied from the updated README)

---

## When to Follow This Process

RFCs should be created for any "substantial" change to Adonis, Lucid, Ace, 1st Party Packages, or the documentation.
Examples of "substantial" changes might include:

* A new feature that adds, removes, or changes methods or classes: creating a new API surface
* The removal of a feature to a separate package
* The introduction of new conventions
* Changes in project structure
* New 1st Party Packages

Changes that do not require an RFC:

* Refactoring, renaming private variables
* Updates to comments
* Minor version updates to dependencies
* Additions that will only be noticed by core contributors and not addon authors or Adonis developers

If you submit a PR or Issue to an Adonis package repo, you may be requested to submit an RFC or issue to the discussion thread first to ensure consensus.

## Gathering Feedback

Discussion is the main driver for successful Open Source communities.
If you need help composing an RFC, create an Issue within this repo to begin a high-level discussion with the goal of creating a formal RFC.

Also feel free to reach out to community members on the [Adonis Gitter](https://gitter.im/adonisjs/adonis-framework) for help creating and submitting an RFC.

## The Process

To make a major feature change to Adonis, an RFC must be accepted and merged into the discussion repository.
At that point, the RFC may be implemented and included in the framework.

To submit an RFC

* Fork the Discussion Repo http://github.com/adonisjs/discussion
* Copy the `0000-template.md` to `text/0000-my-feature.md` (where `my-feature` is a descriptive short name for your proposal, *don't assign a number yet*)
* Fill in the RFC. Put care into each section (especially the "How We Teach This" section) as RFCs that do not present an attention to feature design will likely be closed or asked to rework.
* Submit a pull request. During this time, the RFC will receive feedback from contributors and community members. At this time, you may be asked to revise and push changes to your RFC.
* Build and iterate on feedback. RFCs that have more feedback and consensus are more likely to be accepted into the final framework.
* Eventually a core team member will flag the pull request as "final comment period". This period will be 7 days for final discussion.
* Significant changes during the "final comment period" may trigger a new 7 day period of commenting.
* Any RFC may be rejected by the core team based on public discussion or conflicts with other features or RFCs. A comment will be made on the pull request detailing the reasons the RFC was rejected, and the associated pull request will then be closed.
* At the end of the "final commend period", an RFC may be accepted by the core contributors and merged into the discussion repository. At this point the RFC will be considered "active" and implementations can be merged into the respective package or core repository.

## RFC Lifecycle

Once an RFC becomes active, the PR will be merged and an implementation issue will be opened, authors may implement it and submit the feature as a pull-request to the respective repo.
RFCs that are in the "active" stage may not be implemented, and implementations of "active" RFCs may not be merged in to the framework.

Modifications to existing "active" RFCs can be made via pull requests to further align RFCs that are still "active" but have not been implemented.

## Implementing RFCs

RFC authors are not required to provide implementation.
Of course: third party packages, example implementations, or proof-of-concepts are welcome and can be linked to in the RFC.
These can be used directly or used to influence the final implementation of a proposed feature.

If you are interested in working on an RFC implementation or know of design decisions that may help in the implementation of the proposed feature, feel free to comment on the associated issue.

## Review Process for RFCs

Each week, the core contributors will attempt to review some of the open RFC pull requests.
Also, community members will attempt to help transfer issues into RFC format.

Each accepted RFC will have a champion who will represent the feature and the progress.

The Adonis RFC process owes its inspiration to the [Ember](https://github.com/emberjs/rfcs) and [Rust](https://github.com/rust-lang/rfcs) RFC process.

# How We Teach This
[how-we-teach-this]: #how-we-teach-this

What names and terminology work best for these concepts and why?
How is this idea best presented—as a continuation of existing patterns, or as a wholly new one?

Would the acceptance of this proposal change how Adonis is taught to new users at any level?
How should this feature be introduced and taught to existing Adonis users?

What additions or changes to the Adonis Docs will be needed for this new feature?
What will users need to know before upgrading their apps to a version that contains this feature?

# Drawbacks
[drawbacks]: #drawbacks

* This may slow down new feature development as RFCs require a 7 day comment period.
* Community involvement may be small at the onset and RFCs will be mostly existing discussions that have traditionally occurred over direct message or in private.
* Core Contributors will still have to follow the full RFC process for new features
* "Surprise Features" will be less likely since public record of RFCs

# Alternatives
[alternatives]: #alternatives

Continuing with the existing discussion issue process though it lacks inline commenting, change tracking, or (easy) ways to see what has been accepted.

# Unresolved questions
[unresolved]: #unresolved-questions

* Do more members need to be added as "Core Contributors" to Adonis or the Discussion Repo?
* Should weekly meetings or times be set to review RFCs?
