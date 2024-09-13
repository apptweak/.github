<!--- Provide a general summary of your changes in the Title above -->
<!-- This is a template, feel free to remove unused sections or add information you think is needed -->

## What are you doing and why
<!--- Describe your changes in detail. Explain the process which led you to decide to make the change as you did -->

## Associated ticket number and/or AirBrake error?
<!--- If this has a related ticket/task, add it here -->
<!--- Also add any AirBrake errors that will be fixed by this -->

## Due Date or Desirable Merge
<!-- If you have an idea of the urgency of the PR or would like to inform the reviewers of when you would like to get answers -->
<!-- Be reasonable and keep in mind that people will not be obligated to answer in your time, but this can be helpful to prioritize reviews -->
<!-- For example: Needs to be merged before 2024-02-29 | I would like to merge this sometime in the next two weeks | This is super urgent and is blocking this other task, please review ASAP -->

## How has this been tested?
<!--- Please describe in detail how you tested your changes. -->
<!--- Include details of your testing environment and the tests you ran to -->
<!--- See how your change affects other areas of the code, etc. -->
<!--- If you did not add automated tests covering your changes, explain why -->

## Anticipated impact
<!--- What do you expect this change will impact? Does some other repo also need to be changed? -->
<!--- Does your change include a database modification? Can it be deployed without downtime? -->
<!--- Does it require a cache version bump? -->

## How do you plan to monitor the change in prod to make sure it's working?
<!--- What logs can you monitor once it's in prod -->
<!--- Which changes do you plan to see in prod that will let you know the change works as expected -->
<!--- Which instrumentation have you included to help monitor and check the changes -->
<!--- What kind of test can you run in prod (if any) to make sure it's working -->

## Checklist
<!--- Go over all the following points, and put an `x` in all the boxes that apply. -->
<!--- If one or more lines do not apply, use ~ to ~strikethrough~ the whole line -->
<!--- If you're unsure about any of these, don't hesitate to ask. We're here to help! -->
- [ ] My code follows the code style of this project.
- [ ] I have run tests locally (manual tests and otherwise).
- [ ] This has been tested on staging.
- [ ] My change requires a change to the documentation.
  - [ ] I have updated the documentation accordingly.
- [ ] My change includes a database modification
  - [ ] I have tested my database modification in staging.
- [ ] My change affects endpoints for console or search-ads integrations. If so:
  - [ ] I am tagging a reviewer to explicitly review the security of this change: (flag reviewer here)
- [ ] My changes require changes in other components/squads/teams
  - [ ] I already did the changes in the other components or notified the responsible people that the changes need to be done
  - [ ] The needed changes are already deployed or ready to be deployed
