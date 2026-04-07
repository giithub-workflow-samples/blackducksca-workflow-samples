# Black Duck SCA — GitHub Actions Workflow Samples

> Executable GitHub Actions workflow examples for Black Duck Software Composition Analysis (SCA).

## Examples

| Example | Description |
|---|---|
| [build-scan](https://github.com/giithub-workflow-samples/build-scan) | Full build scan — installs dependencies then runs Black Duck SCA scan |
| [buildless-scan](https://github.com/giithub-workflow-samples/buildless-scan) | Buildless scan — runs scan without a build step |
| [simplified-example](https://github.com/giithub-workflow-samples/simplified-example) | Minimal configuration to get started quickly |
| [sarif-generation](https://github.com/giithub-workflow-samples/sarif-generation) | Exports scan results in SARIF format for the GitHub Security tab |
| [pr-comments](https://github.com/giithub-workflow-samples/pr-comments) | Posts scan results as pull request review comments |
| [build-break](https://github.com/giithub-workflow-samples/build-break) | Fails the pipeline when vulnerabilities exceed policy thresholds |
| [automatic-fixpr](https://github.com/giithub-workflow-samples/automatic-fixpr) | Automatically creates PRs to remediate vulnerable dependencies |
| [detailed-example](https://github.com/giithub-workflow-samples/detailed-example) | Comprehensive workflow with all available parameters documented |
| [arbitrary-params](https://github.com/giithub-workflow-samples/arbitrary-params) | Demonstrates passing custom parameters to the Black Duck scan |
| [async-mode](https://github.com/giithub-workflow-samples/async-mode) | Runs the scan asynchronously without blocking the pipeline |

## Prerequisites

- A Black Duck instance (SaaS or on-prem)
- GitHub repository with the following secrets configured:
  - `BLACKDUCK_URL` — URL of your Black Duck instance
  - `BLACKDUCK_API_TOKEN` — API token with scan permissions

## Navigation

[← Back to GitHub Workflow Samples](https://github.com/giithub-workflow-samples)
