<!--
Copyright The Shipwright Contributors

SPDX-License-Identifier: Apache-2.0
-->

# Contributing Guidelines

Welcome to Shipwright, we are glad you want to contribute to the project!
This document contains general guidelines for submitting contributions.
Each component of Shipwright will have its own specific guidelines.

## Contributing prerequisites (CLA/DCO)

The project enforces [Developer Certificate of Origin (DCO)](https://wiki.linuxfoundation.org/dco).
By submitting pull requests submitters acknowledge they grant the
[Apache License v2](./LICENSE) to the code and that they are eligible to grant this license for all commits submitted in their pull requests.

## Getting Started

All contributors must abide by our [Code of Conduct](/CODE_OF_CONDUCT.md).

The core code for Shipwright is located in the following repositories:

* [build](https://github.com/shipwright-io/build) - the Build APIs and associated controller to run builds.
* [cli](https://github.com/shipwright-io/cli) - the `shp` command line for Shipwright builds
* [operator](https://github.com/shipwright-io/operator) - an operator to install Shipwright components on Kubernetes via OLM.

Technical documentation is spread across the code repositories, and is consolidated in the [website](https://github.com/shipwright-io/website) repository.
Content in `website` is published to [shipwright.io](https://shipwright.io)

## Creating new Issues

We recommend to open an issue for the following scenarios:

- Asking for help or questions. (_Use the **discussion** or **help_wanted** label_)
- Reporting a bug. (_Use the **kind/bug** label_)
- Requesting a new feature. (_Use the **kind/feature** label_)

Use the following checklist to determine where you should create an issue:

- If the issue is related to how a Build or BuildRun behaves, or related to Build strategies, create an issue in [build](https://github.com/shipwright-io/build).
- If the issue is related to the command line, create an issue in [cli](https://github.com/shipwright-io/cli).
- If the issue is related to how the operator installs Shipwright on a cluster, create an issue in [operator](https://github.com/shipwright-io/operator).
- If the issue is related to the shipwright.io website, create an issue in [website](https://github.com/shipwright-io/website).

If you are not sure, create an issue in the [community](https://github.com/shipwright-io/community) repository, and the Shipwright maintainers will route it to the correct location.

If feature request is sufficiently broad or significant, the community may ask you to submit a SHIP enhancement proposal.
Please refer to the [SHIP guidelines](/ships/README.md) to learn how to submit a SHIP proposal.

## Writing Pull Requests

Contributions can be submitted by creating a pull request on Github.
We recommend you do the following to ensure the maintainers can collaborate on your contribution:

- Fork the project into your personal Github account.
- Create a new feature branch for your contribution from the latest `main` branch commit.
- Make your changes, ensuring that tests are passing.
- Commit your code changes locally, with a clear commit message and a Developer Certificate of
  Origin [(DCO)](https://wiki.linuxfoundation.org/dco) sign-off footer. You can do this by using
  the `-s` flag when committing changes with git, or amending your commit message after the fact:

  ```sh
  git commit --amend -s
  ```

- Push your code changes to GitHub, then [create a pull request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request)
  with a clear title for the community review. Most Shipwright repositories use templates to
  generate pull request descriptions. If so, please fill out all sections so your change is
  easier to discuss and accept. Finally, please reference the appropriate GitHub issue if your change
  provides a fix or implements a feature.

**NOTE**: All commits must have a DCO sign-off in order for your change to be accepted. See more information on DCO signing [here](https://github.com/apps/dco).

## Code review process

Once your pull request is submitted, a Shipwright maintainer should be assigned to review your changes.

The code review should cover:

- Ensure all related tests (unit, integration and e2e) are passing.
- Ensure the code style is compliant with the [coding conventions](https://github.com/kubernetes/community/blob/master/contributors/guide/coding-conventions.md)
- Ensure the code is properly documented, e.g. enough comments where needed.
- Ensure the code is adding the necessary test cases (unit, integration or e2e) if needed.

Contributors are expected to respond to feedback from reviewers in a constructive manner.
Reviewers are expected to respond to new submissions in a timely fashion, with clear language if changes are requested.

Once the pull request is approved and marked "lgtm", it will get merged.

## Community Meetings Participation

We run the community meetings every Monday at 13:00 UTC time.
For each upcoming meeting we generate a new issue where we layout the topics to discuss.
See our [previous meetings](https://github.com/shipwright-io/build/issues?q=is%3Aissue+label%3Acommunity+is%3Aclosed) outcomes.
Please request an invite in our Slack [channel](https://kubernetes.slack.com/archives/C019ZRGUEJC) or join the [shipwright-dev mailing list](https://lists.shipwright.io/admin/lists/shipwright-users.lists.shipwright.io/).

All meetings are also published on our [public calendar](https://calendar.google.com/calendar/embed?src=shipwright-admin%40lists.shipwright.io&ctz=America%2FNew_York).

## Contact Information

- [Slack channel](https://kubernetes.slack.com/archives/C019ZRGUEJC)
- End-user email list: [shipwright-users@lists.shipwright.io](https://lists.shipwright.io/admin/lists/shipwright-users.lists.shipwright.io/)
- Developer email list: [shipwright-dev@lists.shipwright.io](https://lists.shipwright.io/admin/lists/shipwright-dev.lists.shipwright.io/)
