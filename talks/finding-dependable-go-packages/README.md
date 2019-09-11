# Finding dependable Go packages (Julie Qiu @JQiu25)

## Intro

https://speakerdeck.com/julieqiu/finding-dependable-go-packages

This talk was about how to find and choose Go packages to use in your projects. Julie suggested a three stage approach.

## Discovery

How to find the package?

- Social media?
- Google search?

## How to evaluate a package

### Popularity

- Does the package have a licence?
- Is the package popular?
  - Downloads / Stars / Forks / Watchers
  - Contributors
  - Dependents

### Quality

- How good is the quality of the code in the package?
  - Documentation (godoc.org)
  - Tests (goreportcard.com)
  - Bugs (staticcheck.io)

### Maintained

- What is the upkeep of the package?
  - Maintainer Activity
  - Commit History
  - Issue Tracker

### Dependencies/usage

- How many indirect dependencies does the package have?
  - What if one of those is deleted?
  - Use godoc.org to see the dependencies

## Maintenance - how well is the package maintained

- Stay up to date with releases of the package
- Contribute to the project
- See <https://golang.org/s/discovery-updates>

Notes: I thought we might be able to pull together some kind of checklist that includes some of the above items, in PR checklists for our Go projects.

At the end of the talk Julie announced that the Go community are working on a new discovery site to help with the above process. The site will display documentation for Go packages with version support and provide features that help developers discover and evaluate Go packages or modules. This should be launched at the end of the year. See https://golang.org/s/discovery-updates
