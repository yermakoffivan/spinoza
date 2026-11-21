# Nightly 2026-11-21 — regression

Commit `bf36dd3be4cd`, triggered by schedule. [Run](https://github.com/yermakoffivan/spinoza/actions/runs/44892819509)

| | this run | |
|---|---|---|
| jobs | 89 | 33 failed |
| job-minutes | 704 (-33.6) | |
| e2e coverage | 47% (-0.1) | |
| mutation score | 100% (no change) | 7824 killed, 0 lived |
| flaky | 0 (no change) | passed only on retry |
| uncovered mutants | 341 (no change) | records across reported build variants |

Mutation score is killed / (killed + lived). Uncovered mutants are excluded from that score; some are uninstrumented constant expressions.

## Separate system coverage

These suites retain their own Go statement denominators. The browser E2E coverage above is unchanged by these profiles.

| suite | covered / total statements | coverage |
|---|---|---|
| cluster-mode-auth | 4926 / 21386 | 23% |
| cluster-mode-chromium | 3864 / 21386 | 18.1% |
| cluster-mode-firefox | 3862 / 21386 | 18.1% |
| cluster-mode-webkit | 1987 / 21386 | 9.3% |
| mcp-cli | 794 / 21580 | 3.7% |

## New failures

- cluster-mode-release
- e2e / cluster mode / webkit
- install

## Fixed since the last run

- install / windows arm64, binary and PATH

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
| e2e / checks-issues-worklist / chromium | success | 7.9 |
| e2e / checks-issues-worklist / firefox | success | 8.6 |
| e2e / checks-issues-worklist / webkit | failure | 5.3 |
| e2e / cluster mode / chromium | success | 6.8 |
| e2e / cluster mode / firefox | success | 7.3 |
| e2e / cluster mode / webkit | failure | 7.3 |
| e2e / cluster-mode-auth | success | 11 |
| e2e / distribution-desktop-install | success | 0.1 |
| e2e / e2e-coverage | success | 0.4 |
| e2e / foundation-security / chromium | success | 3.8 |
| e2e / foundation-security / firefox | success | 4.2 |
| e2e / foundation-security / webkit | failure | 5 |
| e2e / gitops / chromium | failure | 7.7 |
| e2e / gitops / firefox | failure | 7.8 |
| e2e / gitops / webkit | failure | 8.3 |
| e2e / helm / chromium | success | 4 |
| e2e / helm / firefox | success | 4.8 |
| e2e / helm / webkit | failure | 4.6 |
| e2e / inspect-compare-rbac-topology / chromium | failure | 7.7 |
| e2e / inspect-compare-rbac-topology / firefox | failure | 8.2 |
| e2e / inspect-compare-rbac-topology / webkit | failure | 7.9 |
| e2e / mcp-cli | success | 3.3 |
| e2e / multicluster-fleet / chromium | failure | 8 |
| e2e / multicluster-fleet / firefox | failure | 8.2 |
| e2e / multicluster-fleet / webkit | failure | 8 |
| e2e / mutations-protection-history / chromium | success | 5 |
| e2e / mutations-protection-history / firefox | success | 4.7 |
| e2e / mutations-protection-history / webkit | failure | 5.7 |
| e2e / navigation-interaction / chromium | failure | 7.6 |
| e2e / navigation-interaction / firefox | failure | 7.7 |
| e2e / navigation-interaction / webkit | failure | 7.8 |
| e2e / observability-traffic / chromium | success | 3.2 |
| e2e / observability-traffic / firefox | success | 4 |
| e2e / observability-traffic / webkit | failure | 4.1 |
| e2e / outage / chromium | success | 4.2 |
| e2e / outage / firefox | success | 3.9 |
| e2e / outage / webkit | failure | 4 |
| e2e / resilience-capacity-soak / chromium | failure | 7.5 |
| e2e / resilience-capacity-soak / firefox | failure | 8 |
| e2e / resilience-capacity-soak / webkit | failure | 7.8 |
| e2e / resources-live-tables / chromium | failure | 7.6 |
| e2e / resources-live-tables / firefox | failure | 7.9 |
| e2e / resources-live-tables / webkit | failure | 8.1 |
| e2e / select | success | 0.2 |
| e2e / streams-terminals-forwards / chromium | failure | 8.1 |
| e2e / streams-terminals-forwards / firefox | failure | 8.7 |
| e2e / streams-terminals-forwards / webkit | failure | 5.2 |
| e2e / suite-contract | success | 0.4 |
| e2e / visual-accessibility / chromium | failure | 7.4 |
| e2e / visual-accessibility / firefox | failure | 4.9 |
| e2e / visual-accessibility / webkit | failure | 8.4 |
| fuzz / fuzz (., FuzzServingCheckPublicURL) | success | 10.3 |
| fuzz / fuzz (./internal/access, FuzzDecisionAggregation) | success | 10.7 |
| fuzz / fuzz (./internal/auth, FuzzRoleAuthorization) | success | 10.3 |
| fuzz / fuzz (./internal/charts, FuzzChartIndex) | success | 10.3 |
| fuzz / fuzz (./internal/charts, FuzzFetchableRepositoryURL) | success | 10.3 |
| fuzz / fuzz (./internal/checks, FuzzParseRules) | success | 10.4 |
| fuzz / fuzz (./internal/issues, FuzzCursor) | success | 10.4 |
| fuzz / fuzz (./internal/mcp, FuzzProtocol) | success | 10.5 |
| fuzz / fuzz (./internal/mcp, FuzzStdioFraming) | success | 10.4 |
| fuzz / fuzz (./internal/store, FuzzHistoryLimit) | success | 10.3 |
| fuzz / fuzz (./internal/store, FuzzTimelineCellsRoundTrip) | success | 10.3 |
| install | skipped | 0 |
| mutation / mutation (checks-a-e) | success | 15.2 |
| mutation / mutation (checks-f-j) | success | 12.5 |
| mutation / mutation (checks-k-o) | success | 10.2 |
| mutation / mutation (checks-p-r) | success | 9.2 |
| mutation / mutation (checks-s-t) | success | 6.4 |
| mutation / mutation (checks-u-z) | success | 4.5 |
| mutation / mutation (cmd) | success | 0.8 |
| mutation / mutation (internal-a-d) | success | 17.6 |
| mutation / mutation (internal-e-l) | success | 31.2 |
| mutation / mutation (internal-m-r) | success | 13.9 |
| mutation / mutation (internal-s-z) | success | 8.1 |
| mutation / mutation (resources-a-f) | success | 4.4 |
| mutation / mutation (resources-g-l) | success | 1.1 |
| mutation / mutation (resources-m-r) | success | 12.1 |
| mutation / mutation (resources-s-z) | success | 3.6 |
| mutation / mutation (root-default) | success | 5.6 |
| mutation / mutation (root-desktop) | success | 5.4 |
| mutation / mutation (server-a-c) | success | 17.6 |
| mutation / mutation (server-d-e) | success | 5.7 |
| mutation / mutation (server-f) | success | 18.9 |
| mutation / mutation (server-g-l) | success | 29.7 |
| mutation / mutation (server-m-r) | success | 8 |
| mutation / mutation (server-s-z) | success | 36 |
| mutation / mutation-total | success | 0.2 |
| repeat | success | 3.6 |
