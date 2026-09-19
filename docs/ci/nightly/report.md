# Nightly 2026-09-19 — regression

Commit `a29317eb60e0`, triggered by schedule. [Run](https://github.com/yermakoffivan/spinoza/actions/runs/35429528378)

| | this run | |
|---|---|---|
| jobs | 89 | 2 failed |
| job-minutes | 782.4 (-12) | |
| e2e coverage | 60.3% (no change) | |
| mutation score | 100% (no change) | 7783 killed, 0 lived |
| flaky | 0 (no change) | passed only on retry |

## New failures

- cluster-mode-release
- install

## Failing

- cluster-mode-release
- install

## Jobs

| job | result | minutes |
|---|---|---|
| cluster-mode-release | skipped | 0 |
| e2e / checks-issues-worklist / chromium | success | 5.6 |
| e2e / checks-issues-worklist / firefox | success | 5.3 |
| e2e / checks-issues-worklist / webkit | success | 6.2 |
| e2e / cluster mode / chromium | success | 6.2 |
| e2e / cluster mode / firefox | success | 6.6 |
| e2e / cluster mode / webkit | success | 7.1 |
| e2e / cluster-mode-auth | success | 10.3 |
| e2e / distribution-desktop-install | success | 0.2 |
| e2e / e2e-coverage | success | 0.3 |
| e2e / foundation-security / chromium | success | 4.6 |
| e2e / foundation-security / firefox | success | 4.9 |
| e2e / foundation-security / webkit | success | 4.1 |
| e2e / gitops / chromium | success | 7.7 |
| e2e / gitops / firefox | success | 8.1 |
| e2e / gitops / webkit | success | 8.4 |
| e2e / helm / chromium | success | 5 |
| e2e / helm / firefox | success | 4.9 |
| e2e / helm / webkit | success | 5.2 |
| e2e / inspect-compare-rbac-topology / chromium | success | 9 |
| e2e / inspect-compare-rbac-topology / firefox | success | 9 |
| e2e / inspect-compare-rbac-topology / webkit | success | 9.2 |
| e2e / mcp-cli | success | 3.1 |
| e2e / multicluster-fleet / chromium | success | 9 |
| e2e / multicluster-fleet / firefox | success | 9.9 |
| e2e / multicluster-fleet / webkit | success | 8.8 |
| e2e / mutations-protection-history / chromium | success | 5.2 |
| e2e / mutations-protection-history / firefox | success | 5.6 |
| e2e / mutations-protection-history / webkit | success | 6.3 |
| e2e / navigation-interaction / chromium | success | 10.3 |
| e2e / navigation-interaction / firefox | success | 10.9 |
| e2e / navigation-interaction / webkit | success | 11.2 |
| e2e / observability-traffic / chromium | success | 5.1 |
| e2e / observability-traffic / firefox | success | 4.4 |
| e2e / observability-traffic / webkit | success | 4.8 |
| e2e / outage / chromium | success | 4.9 |
| e2e / outage / firefox | success | 5 |
| e2e / outage / webkit | success | 5 |
| e2e / resilience-capacity-soak / chromium | success | 7.7 |
| e2e / resilience-capacity-soak / firefox | success | 7.7 |
| e2e / resilience-capacity-soak / webkit | success | 8.5 |
| e2e / resources-live-tables / chromium | success | 8.3 |
| e2e / resources-live-tables / firefox | success | 9 |
| e2e / resources-live-tables / webkit | success | 8.8 |
| e2e / select | success | 0.2 |
| e2e / streams-terminals-forwards / chromium | success | 5.3 |
| e2e / streams-terminals-forwards / firefox | success | 4.8 |
| e2e / streams-terminals-forwards / webkit | success | 5.4 |
| e2e / suite-contract | success | 0.4 |
| e2e / visual-accessibility / chromium | success | 13.3 |
| e2e / visual-accessibility / firefox | success | 13.3 |
| e2e / visual-accessibility / webkit | success | 13.5 |
| fuzz / fuzz (., FuzzServingCheckPublicURL) | success | 12.6 |
| fuzz / fuzz (./internal/access, FuzzDecisionAggregation) | success | 11.2 |
| fuzz / fuzz (./internal/auth, FuzzRoleAuthorization) | success | 10.7 |
| fuzz / fuzz (./internal/charts, FuzzChartIndex) | success | 10.5 |
| fuzz / fuzz (./internal/charts, FuzzFetchableRepositoryURL) | success | 10.5 |
| fuzz / fuzz (./internal/checks, FuzzParseRules) | success | 11.3 |
| fuzz / fuzz (./internal/issues, FuzzCursor) | success | 10.6 |
| fuzz / fuzz (./internal/mcp, FuzzProtocol) | success | 11.7 |
| fuzz / fuzz (./internal/mcp, FuzzStdioFraming) | success | 11.5 |
| fuzz / fuzz (./internal/store, FuzzHistoryLimit) | success | 10.9 |
| fuzz / fuzz (./internal/store, FuzzTimelineCellsRoundTrip) | success | 10.7 |
| install | skipped | 0 |
| mutation / mutation (checks-a-e) | success | 14.6 |
| mutation / mutation (checks-f-j) | success | 17.2 |
| mutation / mutation (checks-k-o) | success | 8 |
| mutation / mutation (checks-p-r) | success | 13.1 |
| mutation / mutation (checks-s-t) | success | 10 |
| mutation / mutation (checks-u-z) | success | 6.3 |
| mutation / mutation (cmd) | success | 2.5 |
| mutation / mutation (internal-a-d) | success | 17 |
| mutation / mutation (internal-e-l) | success | 35.3 |
| mutation / mutation (internal-m-r) | success | 10.9 |
| mutation / mutation (internal-s-z) | success | 9.2 |
| mutation / mutation (resources-a-f) | success | 4.4 |
| mutation / mutation (resources-g-l) | success | 2 |
| mutation / mutation (resources-m-r) | success | 14.7 |
| mutation / mutation (resources-s-z) | success | 5.1 |
| mutation / mutation (root-default) | success | 6.8 |
| mutation / mutation (root-desktop) | success | 6.9 |
| mutation / mutation (server-a-c) | success | 24.4 |
| mutation / mutation (server-d-e) | success | 6 |
| mutation / mutation (server-f) | success | 22.1 |
| mutation / mutation (server-g-l) | success | 28.3 |
| mutation / mutation (server-m-r) | success | 12 |
| mutation / mutation (server-s-z) | success | 32.7 |
| mutation / mutation-total | success | 0.2 |
| repeat | success | 6.9 |
