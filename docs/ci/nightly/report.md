# Nightly 2026-11-14 — regression

Commit `6a3f44c7f5ff`, triggered by schedule. [Run](https://github.com/yermakoffivan/spinoza/actions/runs/43580063235)

| | this run | |
|---|---|---|
| jobs | 89 | 33 failed |
| job-minutes | 728.9 (+4.6) | |
| e2e coverage | 47.3% (+0.3) | |
| mutation score | 100% (no change) | 7824 killed, 0 lived |
| flaky | 0 (no change) | passed only on retry |
| uncovered mutants | 341 (no change) | records across reported build variants |

Mutation score is killed / (killed + lived). Uncovered mutants are excluded from that score; some are uninstrumented constant expressions.

## Separate system coverage

These suites retain their own Go statement denominators. The browser E2E coverage above is unchanged by these profiles.

| suite | covered / total statements | coverage |
|---|---|---|
| cluster-mode-auth | 4926 / 21386 | 23% |
| cluster-mode-chromium | 3861 / 21386 | 18.1% |
| cluster-mode-firefox | 3865 / 21386 | 18.1% |
| cluster-mode-webkit | 1987 / 21386 | 9.3% |
| mcp-cli | 794 / 21580 | 3.7% |

## New failures

- cluster-mode-release
- e2e / cluster mode / webkit
- install

## Failing

- cluster-mode-release
- e2e / checks-issues-worklist / webkit
- e2e / cluster mode / webkit
- e2e / foundation-security / webkit
- e2e / gitops / chromium
- e2e / gitops / firefox
- e2e / gitops / webkit
- e2e / helm / webkit
- e2e / inspect-compare-rbac-topology / chromium
- e2e / inspect-compare-rbac-topology / firefox
- e2e / inspect-compare-rbac-topology / webkit
- e2e / multicluster-fleet / chromium
- e2e / multicluster-fleet / firefox
- e2e / multicluster-fleet / webkit
- e2e / mutations-protection-history / webkit
- e2e / navigation-interaction / chromium
- e2e / navigation-interaction / firefox
- e2e / navigation-interaction / webkit
- e2e / observability-traffic / webkit
- e2e / outage / webkit
- e2e / resilience-capacity-soak / chromium
- e2e / resilience-capacity-soak / firefox
- e2e / resilience-capacity-soak / webkit
- e2e / resources-live-tables / chromium
- e2e / resources-live-tables / firefox
- e2e / resources-live-tables / webkit
- e2e / streams-terminals-forwards / chromium
- e2e / streams-terminals-forwards / firefox
- e2e / streams-terminals-forwards / webkit
- e2e / visual-accessibility / chromium
- e2e / visual-accessibility / firefox
- e2e / visual-accessibility / webkit
- install

## Jobs

| job | result | minutes |
|---|---|---|
| cluster-mode-release | skipped | 0 |
| e2e / checks-issues-worklist / chromium | success | 8 |
| e2e / checks-issues-worklist / firefox | success | 8.2 |
| e2e / checks-issues-worklist / webkit | failure | 3.8 |
| e2e / cluster mode / chromium | success | 7.3 |
| e2e / cluster mode / firefox | success | 6.9 |
| e2e / cluster mode / webkit | failure | 6.5 |
| e2e / cluster-mode-auth | success | 12.1 |
| e2e / distribution-desktop-install | success | 0.1 |
| e2e / e2e-coverage | success | 0.3 |
| e2e / foundation-security / chromium | success | 4.2 |
| e2e / foundation-security / firefox | success | 4.4 |
| e2e / foundation-security / webkit | failure | 3.9 |
| e2e / gitops / chromium | failure | 12.4 |
| e2e / gitops / firefox | failure | 12.3 |
| e2e / gitops / webkit | failure | 12.9 |
| e2e / helm / chromium | success | 4.8 |
| e2e / helm / firefox | success | 5.2 |
| e2e / helm / webkit | failure | 5 |
| e2e / inspect-compare-rbac-topology / chromium | failure | 7.5 |
| e2e / inspect-compare-rbac-topology / firefox | failure | 7.9 |
| e2e / inspect-compare-rbac-topology / webkit | failure | 8.2 |
| e2e / mcp-cli | success | 3.3 |
| e2e / multicluster-fleet / chromium | failure | 7.7 |
| e2e / multicluster-fleet / firefox | failure | 7.9 |
| e2e / multicluster-fleet / webkit | failure | 8 |
| e2e / mutations-protection-history / chromium | success | 4.2 |
| e2e / mutations-protection-history / firefox | success | 5.7 |
| e2e / mutations-protection-history / webkit | failure | 5.3 |
| e2e / navigation-interaction / chromium | failure | 7.8 |
| e2e / navigation-interaction / firefox | failure | 7.9 |
| e2e / navigation-interaction / webkit | failure | 7.9 |
| e2e / observability-traffic / chromium | success | 3.6 |
| e2e / observability-traffic / firefox | success | 4.5 |
| e2e / observability-traffic / webkit | failure | 4.7 |
| e2e / outage / chromium | success | 4.2 |
| e2e / outage / firefox | success | 3.8 |
| e2e / outage / webkit | failure | 3.5 |
| e2e / resilience-capacity-soak / chromium | failure | 7.7 |
| e2e / resilience-capacity-soak / firefox | failure | 8.3 |
| e2e / resilience-capacity-soak / webkit | failure | 8 |
| e2e / resources-live-tables / chromium | failure | 12.5 |
| e2e / resources-live-tables / firefox | failure | 7.9 |
| e2e / resources-live-tables / webkit | failure | 8.3 |
| e2e / select | success | 0.1 |
| e2e / streams-terminals-forwards / chromium | failure | 8 |
| e2e / streams-terminals-forwards / firefox | failure | 8.9 |
| e2e / streams-terminals-forwards / webkit | failure | 5.4 |
| e2e / suite-contract | success | 0.3 |
| e2e / visual-accessibility / chromium | failure | 7.5 |
| e2e / visual-accessibility / firefox | failure | 5.2 |
| e2e / visual-accessibility / webkit | failure | 8.1 |
| fuzz / fuzz (., FuzzServingCheckPublicURL) | success | 12.6 |
| fuzz / fuzz (./internal/access, FuzzDecisionAggregation) | success | 11.4 |
| fuzz / fuzz (./internal/auth, FuzzRoleAuthorization) | success | 10.4 |
| fuzz / fuzz (./internal/charts, FuzzChartIndex) | success | 10.4 |
| fuzz / fuzz (./internal/charts, FuzzFetchableRepositoryURL) | success | 10.4 |
| fuzz / fuzz (./internal/checks, FuzzParseRules) | success | 11.3 |
| fuzz / fuzz (./internal/issues, FuzzCursor) | success | 10.5 |
| fuzz / fuzz (./internal/mcp, FuzzProtocol) | success | 11.3 |
| fuzz / fuzz (./internal/mcp, FuzzStdioFraming) | success | 11.3 |
| fuzz / fuzz (./internal/store, FuzzHistoryLimit) | success | 10.8 |
| fuzz / fuzz (./internal/store, FuzzTimelineCellsRoundTrip) | success | 10.7 |
| install | skipped | 0 |
| mutation / mutation (checks-a-e) | success | 11 |
| mutation / mutation (checks-f-j) | success | 14 |
| mutation / mutation (checks-k-o) | success | 10.3 |
| mutation / mutation (checks-p-r) | success | 11.2 |
| mutation / mutation (checks-s-t) | success | 7 |
| mutation / mutation (checks-u-z) | success | 4.6 |
| mutation / mutation (cmd) | success | 1.2 |
| mutation / mutation (internal-a-d) | success | 14.2 |
| mutation / mutation (internal-e-l) | success | 24.7 |
| mutation / mutation (internal-m-r) | success | 12.9 |
| mutation / mutation (internal-s-z) | success | 6.6 |
| mutation / mutation (resources-a-f) | success | 4.4 |
| mutation / mutation (resources-g-l) | success | 1.2 |
| mutation / mutation (resources-m-r) | success | 12.4 |
| mutation / mutation (resources-s-z) | success | 4.1 |
| mutation / mutation (root-default) | success | 5.3 |
| mutation / mutation (root-desktop) | success | 6.2 |
| mutation / mutation (server-a-c) | success | 24.9 |
| mutation / mutation (server-d-e) | success | 6.7 |
| mutation / mutation (server-f) | success | 18.4 |
| mutation / mutation (server-g-l) | success | 30.4 |
| mutation / mutation (server-m-r) | success | 12.3 |
| mutation / mutation (server-s-z) | success | 29.8 |
| mutation / mutation-total | success | 0.2 |
| repeat | success | 5.7 |
