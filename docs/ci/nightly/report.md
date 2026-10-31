# Nightly 2026-10-31 — regression

Commit `6a3f44c7f5ff`, triggered by schedule. [Run](https://github.com/yermakoffivan/spinoza/actions/runs/41186013735)

| | this run | |
|---|---|---|
| jobs | 89 | 2 failed |
| job-minutes | 784.5 (+60.2) | |
| e2e coverage | 64.3% (+17.3) | |
| mutation score | 100% (no change) | 7824 killed, 0 lived |
| flaky | 2 (+2) | passed only on retry |
| uncovered mutants | 341 (no change) | records across reported build variants |

Mutation score is killed / (killed + lived). Uncovered mutants are excluded from that score; some are uninstrumented constant expressions.

## Separate system coverage

These suites retain their own Go statement denominators. The browser E2E coverage above is unchanged by these profiles.

| suite | covered / total statements | coverage |
|---|---|---|
| cluster-mode-auth | 4926 / 21386 | 23% |
| cluster-mode-chromium | 3859 / 21386 | 18% |
| cluster-mode-firefox | 3862 / 21386 | 18.1% |
| cluster-mode-webkit | 3861 / 21386 | 18.1% |
| mcp-cli | 794 / 21580 | 3.7% |

## New failures

- cluster-mode-release
- install

## Fixed since the last run

- e2e / checks-issues-worklist / webkit
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

## Failing

- cluster-mode-release
- install

## Flaky

| test | file | project | attempts |
|---|---|---|---|
| at the supported floor › the chrome a person steers with is all on screen | specs-full/viewport.spec.ts:63 | webkit | 2 |
| forward notifications can be filtered, followed, and cleared | specs/portforward.spec.ts:380 | webkit | 2 |

## Jobs

| job | result | minutes |
|---|---|---|
| cluster-mode-release | skipped | 0 |
| e2e / checks-issues-worklist / chromium | success | 7.7 |
| e2e / checks-issues-worklist / firefox | success | 7.6 |
| e2e / checks-issues-worklist / webkit | success | 8.3 |
| e2e / cluster mode / chromium | success | 6.5 |
| e2e / cluster mode / firefox | success | 7.6 |
| e2e / cluster mode / webkit | success | 7.8 |
| e2e / cluster-mode-auth | success | 11 |
| e2e / distribution-desktop-install | success | 0.1 |
| e2e / e2e-coverage | success | 0.3 |
| e2e / foundation-security / chromium | success | 4 |
| e2e / foundation-security / firefox | success | 3.7 |
| e2e / foundation-security / webkit | success | 4.4 |
| e2e / gitops / chromium | success | 10.1 |
| e2e / gitops / firefox | success | 10.1 |
| e2e / gitops / webkit | success | 11 |
| e2e / helm / chromium | success | 5.1 |
| e2e / helm / firefox | success | 5 |
| e2e / helm / webkit | success | 4.4 |
| e2e / inspect-compare-rbac-topology / chromium | success | 9.4 |
| e2e / inspect-compare-rbac-topology / firefox | success | 11 |
| e2e / inspect-compare-rbac-topology / webkit | success | 10 |
| e2e / mcp-cli | success | 3.5 |
| e2e / multicluster-fleet / chromium | success | 9.1 |
| e2e / multicluster-fleet / firefox | success | 10.7 |
| e2e / multicluster-fleet / webkit | success | 9.3 |
| e2e / mutations-protection-history / chromium | success | 5.1 |
| e2e / mutations-protection-history / firefox | success | 4.6 |
| e2e / mutations-protection-history / webkit | success | 4.6 |
| e2e / navigation-interaction / chromium | success | 11.3 |
| e2e / navigation-interaction / firefox | success | 11 |
| e2e / navigation-interaction / webkit | success | 11.6 |
| e2e / observability-traffic / chromium | success | 3.8 |
| e2e / observability-traffic / firefox | success | 3.5 |
| e2e / observability-traffic / webkit | success | 4.6 |
| e2e / outage / chromium | success | 4 |
| e2e / outage / firefox | success | 4.3 |
| e2e / outage / webkit | success | 4.2 |
| e2e / resilience-capacity-soak / chromium | success | 8.3 |
| e2e / resilience-capacity-soak / firefox | success | 9.2 |
| e2e / resilience-capacity-soak / webkit | success | 9.1 |
| e2e / resources-live-tables / chromium | success | 9.3 |
| e2e / resources-live-tables / firefox | success | 8.7 |
| e2e / resources-live-tables / webkit | success | 9.4 |
| e2e / select | success | 0.2 |
| e2e / streams-terminals-forwards / chromium | success | 5.6 |
| e2e / streams-terminals-forwards / firefox | success | 5.3 |
| e2e / streams-terminals-forwards / webkit | success | 6.5 |
| e2e / suite-contract | success | 0.4 |
| e2e / visual-accessibility / chromium | success | 14.9 |
| e2e / visual-accessibility / firefox | success | 14.6 |
| e2e / visual-accessibility / webkit | success | 15.5 |
| fuzz / fuzz (., FuzzServingCheckPublicURL) | success | 12.4 |
| fuzz / fuzz (./internal/access, FuzzDecisionAggregation) | success | 11.8 |
| fuzz / fuzz (./internal/auth, FuzzRoleAuthorization) | success | 10.2 |
| fuzz / fuzz (./internal/charts, FuzzChartIndex) | success | 10.2 |
| fuzz / fuzz (./internal/charts, FuzzFetchableRepositoryURL) | success | 10.2 |
| fuzz / fuzz (./internal/checks, FuzzParseRules) | success | 10.9 |
| fuzz / fuzz (./internal/issues, FuzzCursor) | success | 10.4 |
| fuzz / fuzz (./internal/mcp, FuzzProtocol) | success | 11.6 |
| fuzz / fuzz (./internal/mcp, FuzzStdioFraming) | success | 11 |
| fuzz / fuzz (./internal/store, FuzzHistoryLimit) | success | 10.8 |
| fuzz / fuzz (./internal/store, FuzzTimelineCellsRoundTrip) | success | 10.5 |
| install | skipped | 0 |
| mutation / mutation (checks-a-e) | success | 10.3 |
| mutation / mutation (checks-f-j) | success | 17.7 |
| mutation / mutation (checks-k-o) | success | 10.2 |
| mutation / mutation (checks-p-r) | success | 13.7 |
| mutation / mutation (checks-s-t) | success | 10 |
| mutation / mutation (checks-u-z) | success | 4.4 |
| mutation / mutation (cmd) | success | 0.8 |
| mutation / mutation (internal-a-d) | success | 18.7 |
| mutation / mutation (internal-e-l) | success | 26.7 |
| mutation / mutation (internal-m-r) | success | 12.7 |
| mutation / mutation (internal-s-z) | success | 7.5 |
| mutation / mutation (resources-a-f) | success | 5.4 |
| mutation / mutation (resources-g-l) | success | 1 |
| mutation / mutation (resources-m-r) | success | 14.2 |
| mutation / mutation (resources-s-z) | success | 3.9 |
| mutation / mutation (root-default) | success | 6.1 |
| mutation / mutation (root-desktop) | success | 5.3 |
| mutation / mutation (server-a-c) | success | 24.8 |
| mutation / mutation (server-d-e) | success | 7.2 |
| mutation / mutation (server-f) | success | 23.4 |
| mutation / mutation (server-g-l) | success | 32.9 |
| mutation / mutation (server-m-r) | success | 8.5 |
| mutation / mutation (server-s-z) | success | 24.9 |
| mutation / mutation-total | success | 0.2 |
| repeat | success | 6.7 |
