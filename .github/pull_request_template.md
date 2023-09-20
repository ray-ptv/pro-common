## Jira Ticket
[{{ .ticket }}](https://plutotv.atlassian.net/browse/{{ .ticket }})
## What does the PR do?
{{ .description }}
- [ ] Increment Chart Version

## Publishing test charts
<details><summary>Details</summary>
<p>
Adding a `/publish` comment to an approved pull request will generate test
charts for any helm chart that has changes in the pull request.  The helm charts
will be published with the version listed in the helm chart with the Jira
ticket suffixed like `1.2.3-PRO-1234`.  

If the chart doesn't publish after triggering,
1. be sure your branch name follows the branch naming standards.
2. check the github action run for errors.
</p>
</details>
