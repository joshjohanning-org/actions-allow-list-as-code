# Actions Allow List as Code

[![🚀🔐 Deploy Actions allow list](https://github.com/joshjohanning-org/actions-allow-list-as-code/actions/workflows/actions-allow-list.yml/badge.svg)](https://github.com/joshjohanning-org/actions-allow-list-as-code/actions/workflows/actions-allow-list.yml)

## How to request new action(s) to be added

1. Open up the [github-actions-allow-list.yml](./github-actions-allow-list.yml)
2. Add additional action(s), one per line
    - Can add an entire organization with `azure/*`, any action version `azure/login@*`, or a specific action version `azure/login@v1`
3. Commit changes in a branch
4. Create a pull request
5. Someone from the [actions-approver-team](https://github.com/orgs/joshjohanning-org/teams/actions-approver-team) will review
6. Upon review and a merge of the Pull Request, the changes will be live in a few seconds after the Actions job finishes running
