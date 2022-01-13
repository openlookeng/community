# OpenLookeng Community Command Help



All of the projects in OpenEuler Community are maintained by Bot. That means the developers can comment below every Pull Request or Issue to trigger Bot Commands. The Commands including as follows:

| Command                 | Example                                                      | Description                                                  | Who Can Use                                                  |
| ----------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| /check-cla              | /check-cla                                                   | Forces rechecking of the CLA status of a Pull Request. If the Pull Request author has already signed CLA, the label `openlookeng-cla/yes` will be added in the Pull Request, If not, the label `openlookeng-cla/no` will be added. | Anyone                                                       |
| /lgtm [cancel]          | /lgtm<br />/lgtm cancel                                      | Adds or removes the `lgtm` label which is typically used to gate merging. | Collaborators on the repository. `/lgtm cancel` can be used additionally by the Pull Request author. |
| /approve [cancel]       | /approve<br/>/approve cancel                                 | Adds or removes the `approved` label which is typically used to gate merging. | Collaborators on the repository.                             |
| /assign [[@]...]        | /assign<br />/assign @openlookeng-bot                        | Assigns assignee(s) to the PR or issue.                      | Anyone can use the command, but the target user(s) must be an org member, a repo collaborator, or should have previously commented on the issue or PR. If no target user is specified, that means will be assigned to yourself. |
| /unassigne              | /unassign <br />/unassign @openlookeng-bot                   | Unassigns assignee(s) to the PR or issue.                    | Anyone can use the command, but the target user(s) must be an org member, a repo collaborator, or should have previously commented on the issue or PR. If no target user is specified, that means will be unassigned to yourself. |
| /[add\|rm]-collaborator | /add-collaborator<br />/rm-collaborator<br />/add collaborator   @openlookeng-bot<br />/rm-collaborator @openlookeng-bot | assigns or unassigns collaborator(s) to the issue            | Anyone can use the command, but the target user(s) must be the repo's member. If no target user is specified, that means will be unassigned to yourself. |
| /check-milestone        | /check-milestone                                             | Check whether the issue is set a milestone, remove or add needs-milestone label | Anyone                                                       |
| /check-issue            | /check-milestone                                             | Check whether the Pull Request is associated with at least an issue, remove or add needs-issue label | Anyone                                                       |
| /remove-needs-issue     | /remove-needs-issue                                          | remove the needs-issue label                                 | Members of the project can use the `/remove-needs-issue`command |
| /check-ci               | /check-ci                                                    | Forces rechecking the CI status and adding CI label if possible. | Anyone                                                       |
| /test ?                 | /test ?                                                      | List available test job(s) for a trusted PR.                 | Anyone                                                       |
| /retest                 | /retest                                                      | Rerun test jobs that have failed.                            | Anyone                                                       |
| /test [\|all]           | /test all<br />/test pull-bazel-test                         | Manually starts a/all test job(s). Lists all possible job(s) when no jobs/an invalid job are specified. | Anyone                                                       |
| /ok-to-test             | /ok-to-test                                                  | Marks a PR as `trusted` and starts tests.                    | Members of the trusted organization for the repo.            |

