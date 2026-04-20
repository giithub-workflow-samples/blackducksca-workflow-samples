# Black Duck SCA Workflow Samples                                                                                                                                                                                                                          

## Table of Contents
- [Overview](#overview)
- [Workflow Samples using Action](#workflow-samples-using-action)
- [Workflow Samples using CLI](#workflow-samples-using-cli)
- [Documentation](#documentation)

## Overview
Live, executable samples using the Black Duck Security Scan Action with Black Duck SCA


## Workflow Samples using Action
| How To? | Details | Workflow  | Results  | Status |
|---------|---------|---------------|--------------|--------------|                                                                                                            
| **Scan repository with build as a pre-step (Recommended)** | This recommended method ensures SAST analysis on compiled code and artifacts through a pre-build step for comprehensive vulnerability detection | [Workflow](https://github.com/giithub-workflow-samples/build-scan/blob/main/.github/workflows/main.yml) |[Results](https://giithub-workflow-samples.github.io/build-scan/execution-logs/) |  |
| **Scan repository in an environment where build is not an option** | This option is less accurate and should be used when you can't build your repository | [Workflow](https://github.com/blackducksca-workflow-samples/buildless-scan/blob/main/.github/workflows/nodejs-npm.yml) | [Results](https://blackducksca-workflow-samples.github.io/buildless-scan/) |  |
| **PR Comments** | For each new vulnerable component that the developer introduces with his/her changes, this integration is capable of adding a comment to the pull request. PR comments enable the developer to quickly view, understand and fix the issue before merging the pull request <br>**Expected Result: FAIL** | [Workflow](https://github.com/blackducksca-workflow-samples/pr-comments/blob/main/.github/workflows/nodejs-npm.yml) | [Results](https://blackducksca-workflow-samples.github.io/pr-comments/) |  |                                                                                     
| **Create Automatic FixPRs** | Fix PR feature automatically creates PRs for vulnerable components found in the scan. This sample shows how you can configure the fix PR feature | [Workflow](https://github.com/blackducksca-workflow-samples/automatic-fixpr/blob/main/.github/workflows/automatic-fixpr.yml) | [Results](https://blackducksca-workflow-samples.github.io/automatic-fixpr/) |  |                                                                            
| **Generate Sarif Reports** | This sample shows how you can create a SARIF file for SCA issues found in the scan | [Workflow](https://github.com/blackducksca-workflow-samples/sarif-generation/blob/main/.github/workflows/nodejs-npm.yml) | [Results](https://blackducksca-workflow-samples.github.io/sarif-generation/) |  |                                                                        
| **Import issues into GitHub Advanced Security** | This sample shows how you can post SCA issues found in the scan to Code Scanning tab in GitHub Advanced Security | [Workflow](https://github.com/blackducksca-workflow-samples/sarif-generation/blob/main/.github/workflows/nodejs-npm.yml) | [Results](https://blackducksca-workflow-samples.github.io/sarif-generation/) |   |
| **Build Break** | The ability to break or not break a build when policy violations are found is configurable. This sample shows you how to configure the build break options. <br>**Expected Result: FAIL** |  [Workflow](https://github.com/blackducksca-workflow-samples/build-break/blob/main/.github/workflows/nodejs-npm.yml) | [Results](https://blackducksca-workflow-samples.github.io/build-break/) |   |                                                                                   
| **Passing Detect tool arguments from Black Duck Sca scans** | To leverage advanced SCA features, you need to pass options to Detect. This sample shows how you can configure Detect options |  [Workflow](https://github.com/blackducksca-workflow-samples/arbitrary-params/blob/main/.github/workflows/nodejs-npm.yml) | [Results](https://blackducksca-workflow-samples.github.io/arbitrary-params/) |   |                                                                           
| **Run scans asynchronously to avoid holding up the pipeline during scanning** | By default, the pipeline is held until the scan finishes. You can configure the workflow in such a way where the pipeline doesn't wait for the scan to finish and returns immediately after kicking off the scan. Note that post scan options are not triggered when you choose to not wait for the scan to finish | [Workflow](https://github.com/blackducksca-workflow-samples/async-mode/blob/main/.github/workflows/nodejs-npm.yml) | [Results](https://blackducksca-workflow-samples.github.io/async-mode/) |  | 
| **Simplified workflow using default configurations for beginners** | Basic workflow demonstrating all Black Duck SCA features with default configurations. Ideal for beginners to explore features quickly | [Workflow](https://github.com/blackducksca-workflow-samples/simplified-example/blob/main/.github/workflows/nodejs-npm.yml) | [Results](https://blackducksca-workflow-samples.github.io/simplified-example/) |   | 
| **Detailed workflow with full configurations for advanced users**  | Comprehensive workflow demonstrating all Black Duck SCA capabilities with full configurations. Ideal for advanced users requiring granular control and customization capabilities | [Workflow](https://github.com/blackducksca-workflow-samples/detailed-example/blob/main/.github/workflows/nodejs-npm.yml) | [Results](https://blackducksca-workflow-samples.github.io/detailed-example/) |   | 


## Workflow Samples using CLI
| How To? | Details | Workflow  | Results  |
|---------|---------|---------------|--------------|
| **Scan repository with build as a pre-step (Recommended)** | This recommended method ensures SAST analysis on compiled code and artifacts through a pre-build step for comprehensive vulnerability detection | [Workflow](https://github.com/blackducksca-workflow-samples/bridgecli/blob/main/.github/workflows/BlackduckSCA_Bridge.yml) | [Results](https://blackducksca-workflow-samples.github.io/bridgecli/) |


## Documentation                                                                                                                                                                                                                         
[Using the Black Duck Security Scan Action with Black Duck SCA Documentation](https://documentation.blackduck.com/bundle/bridge/page/documentation/c_github-blackduck.html)
