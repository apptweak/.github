<!--- Provide a general summary of your changes in the Title above -->
<!-- This is a template, feel free to remove unused sections or add information you think is needed -->

### Linked PRs
<!-- (Optional) Please list any related PRs here:
- PR #123 (Title and link)
- PR #456 (Title and link)
-->

## What does this PR do?
<!--- Describe your changes in detail. Explain the process which led you to decide to make the change as you did -->

<!--
**Before and After Screenshots:**
- **Before:** ![before](link-to-before-screenshot)
- **After:** ![after](link-to-after-screenshot)
-->

## Why is this change necessary?
<!-- (Optional) Describe the reasoning behind this change. Explain the motivation, the problem it addresses, or the benefits it provides.
This section helps reviewers understand the broader context and importance of the changes. -->

## Associated ticket number and/or AirBrake error?
<!--- If this has a related ticket/task, add it here -->
<!--- Also add any AirBrake errors that will be fixed by this -->

## Due Date or Desirable Merge
<!-- If you have an idea of the urgency of the PR or would like to inform the reviewers of when you would like to get answers -->
<!-- Be reasonable and keep in mind that people will not be obligated to answer in your time, but this can be helpful to prioritize reviews -->

<!-- ASAP -->
<!-- Not urgent -->
<!-- Next week -->
<!-- Specific date: [Specify Date] -->

## Checklist
<!--- Go over all the following points, and put an `x` in all the boxes that apply. -->
<!--- If one or more lines do not apply, use ~ to ~strikethrough~ the whole line -->
<!--- If you're unsure about any of these, don't hesitate to ask. We're here to help! -->
- [ ] My code follows the code style of this project.
- [ ] I have added/updated unit tests.
- [ ] This has been tested locally (manual).
- [ ] This has been tested on staging (manual).
- [ ] My change touches on some of the following areas: **authorizing access to integration data** (consoles, search ads, MMP), **authentication** (including serving or consuming OAuth endpoints), **cryptography and security** (including generation of secure tokens). If so:
  - [ ] I am tagging a senior reviewer to specifically review the security of this change: (flag reviewer here)
- [ ] My changes require changes in other components/squads/teams
  - [ ] I already did the changes in the other components or notified the responsible people that the changes need to be done
  - [ ] The needed changes are already deployed or ready to be deployed

### Checklist for DataPi-specific changes
- [ ] I can assess the usage of my change
  - [ ] I added mixpanel events to track the usage of my change
