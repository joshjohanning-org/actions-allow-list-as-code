# Actions Allow List as Code

[![🚀🔐 Deploy Actions allow list](https://github.com/joshjohanning-org/actions-allow-list-as-code/actions/workflows/actions-allow-list.yml/badge.svg)](https://github.com/joshjohanning-org/actions-allow-list-as-code/actions/workflows/actions-allow-list.yml)

## How to request new action(s) to be added

1. Open up the [github-actions-allow-list.yml](./github-actions-allow-list.yml)
2. Add additional action(s), one per line
    - Can add an:
      - entire organization: `azure/*`
      - any action version: `azure/login@*`
      - a specific action version: `azure/login@v1`
      - a specific commit ref (i.e.: branch): `azure/login@main`
      - a specific commit full sha: `azure/login@v5906929b67adab884c91d130ce6a7a3a4205a8dd`
3. Commit changes in a branch
4. Create a pull request
5. Someone from the [actions-approver-team](https://github.com/orgs/joshjohanning-org/teams/actions-approver-team) will review
6. Upon review and a merge of the Pull Request, the changes will be live in a few seconds after the Actions job finishes running 🚀

> [!IMPORTANT]
> Do not remove the `actionsdesk/github-actions-allow-list-as-code-action@*` line otherwise this workflow will fail to initialize (because this Action is blocked) and you will have to manually add it back in.
