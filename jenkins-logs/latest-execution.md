# Jenkins Execution Log

## Build Information
- **Job Name:** `MBP_Github_Polaris_Async_Mode_Scan/main`
- **Build Number:** #2
- **Build Status:** 🟢 **SUCCESS**
- **Duration:** 1 min 32 sec and counting
- **Timestamp:** 2025-11-13 20:31:04 UTC

---

## Console Output

```
Branch indexing
Connecting to https://api.github.com using madhusud@blackduck.com/****** (Github_Username_PAT)
Obtained nodejs-npm/Jenkinsfile from e9bdb3eb4eec4cd752a0420ac526ae347f64b99e
Loading library blackduck-logs-publisher@main
Attempting to resolve main from remote references...
 > git --version # timeout=10
 > git --version # 'git version 2.39.5 (Apple Git-154)'
using GIT_ASKPASS to set credentials Github_Username_PAT
 > git ls-remote -h -- https://github.com/integrations-garage/blackduck-logs-publisher # timeout=10
Found match: refs/heads/main revision e969196a63b1be83b84541b022f7aa52928bd5e5
The recommended git tool is: NONE
using credential Github_Username_PAT
 > git rev-parse --resolve-git-dir /Users/madhusud/.jenkins/workspace/hub_Polaris_Async_Mode_Scan_main@libs/a0dda568bac7bbb4a171f59ba3f2660c21c69edc6356524e9ae8bb4500c12bbb/.git # timeout=10
Fetching changes from the remote Git repository
 > git config remote.origin.url https://github.com/integrations-garage/blackduck-logs-publisher # timeout=10
Fetching without tags
Fetching upstream changes from https://github.com/integrations-garage/blackduck-logs-publisher
 > git --version # timeout=10
 > git --version # 'git version 2.39.5 (Apple Git-154)'
using GIT_ASKPASS to set credentials Github_Username_PAT
 > git fetch --no-tags --force --progress -- https://github.com/integrations-garage/blackduck-logs-publisher +refs/heads/*:refs/remotes/origin/* # timeout=10
Checking out Revision e969196a63b1be83b84541b022f7aa52928bd5e5 (main)
 > git config core.sparsecheckout # timeout=10
 > git checkout -f e969196a63b1be83b84541b022f7aa52928bd5e5 # timeout=10
Commit message: "Phase 3 - 2"
 > git rev-list --no-walk e969196a63b1be83b84541b022f7aa52928bd5e5 # timeout=10
[Pipeline] Start of Pipeline
[Pipeline] node
Running on mac-sh in /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main@2
[Pipeline] {
[Pipeline] stage
[Pipeline] { (Declarative: Checkout SCM)
[Pipeline] checkout
The recommended git tool is: NONE
using credential Github_Username_PAT
Cloning the remote Git repository
Cloning with configured refspecs honoured and without tags
Cloning repository https://github.com/polaris-jenkins-samples/async-mode.git
 > git init /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main@2 # timeout=10
Fetching upstream changes from https://github.com/polaris-jenkins-samples/async-mode.git
 > git --version # timeout=10
 > git --version # 'git version 2.39.5 (Apple Git-154)'
using GIT_ASKPASS to set credentials Github_Username_PAT
 > git fetch --no-tags --force --progress -- https://github.com/polaris-jenkins-samples/async-mode.git +refs/heads/main:refs/remotes/origin/main # timeout=10
Avoid second fetch
Checking out Revision e9bdb3eb4eec4cd752a0420ac526ae347f64b99e (main)
Commit message: "Jenkins log upload - Build #2"
First time build. Skipping changelog.
 > git config remote.origin.url https://github.com/polaris-jenkins-samples/async-mode.git # timeout=10
 > git config --add remote.origin.fetch +refs/heads/main:refs/remotes/origin/main # timeout=10
 > git config core.sparsecheckout # timeout=10
 > git checkout -f e9bdb3eb4eec4cd752a0420ac526ae347f64b99e # timeout=10
[Pipeline] }
[Pipeline] // stage
[Pipeline] withEnv
[Pipeline] {
[Pipeline] stage
[Pipeline] { (Build)
[Pipeline] script
[Pipeline] {
[Pipeline] echo
JOB_NAME: MBP_Github_Polaris_Async_Mode_Scan/main
[Pipeline] dir
Running in /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main@2/nodejs-npm
[Pipeline] {
[Pipeline] sh
+ node --version
v22.16.0
[Pipeline] sh
+ npm --version
10.9.2
[Pipeline] sh
+ npm install
npm warn deprecated fsevents@1.2.9: fsevents 1 will break on node v14+ and could be using insecure binaries. Upgrade to fsevents 2.
npm warn deprecated set-value@2.0.0: Critical bug fixed in v3.0.1, please upgrade to the latest version.
npm warn deprecated mixin-deep@1.3.1: Critical bug fixed in v2.0.1, please upgrade to the latest version.
npm warn deprecated ini@1.3.5: Please update to ini >=1.3.6 to avoid a prototype pollution issue
npm warn deprecated set-value@0.4.3: Critical bug fixed in v3.0.1, please upgrade to the latest version.
npm warn deprecated path-is-absolute@2.0.0: This package is no longer relevant as Node.js 0.12 is unmaintained.
npm warn deprecated urix@0.1.0: Please see https://github.com/lydell/urix#deprecated
npm warn deprecated har-validator@5.1.3: this library is no longer supported
npm warn deprecated to-iso-string@0.0.2: to-iso-string has been deprecated, use @segment/to-iso-string instead.
npm warn deprecated cryptiles@2.0.5: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated resolve-url@0.2.1: https://github.com/lydell/resolve-url#deprecated
npm warn deprecated bcrypt-nodejs@0.0.3: bcrypt-nodejs is no longer actively maintained. Please use bcrypt or bcryptjs. See https://github.com/kelektiv/node.bcrypt.js/wiki/bcrypt-vs-brypt.js to learn more about these two options
npm warn deprecated cryptiles@0.2.2: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated source-map-url@0.4.0: See https://github.com/lydell/source-map-url#deprecated
npm warn deprecated boom@0.4.2: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated debug@3.2.6: Debug versions >=3.2.0 <3.2.7 || >=4 <4.3.1 have a low-severity ReDos regression when used in a Node.js environment. It is recommended you upgrade to 3.2.7 or 4.3.1. (https://github.com/visionmedia/debug/issues/797)
npm warn deprecated debug@3.2.6: Debug versions >=3.2.0 <3.2.7 || >=4 <4.3.1 have a low-severity ReDos regression when used in a Node.js environment. It is recommended you upgrade to 3.2.7 or 4.3.1. (https://github.com/visionmedia/debug/issues/797)
npm warn deprecated debug@3.2.6: Debug versions >=3.2.0 <3.2.7 || >=4 <4.3.1 have a low-severity ReDos regression when used in a Node.js environment. It is recommended you upgrade to 3.2.7 or 4.3.1. (https://github.com/visionmedia/debug/issues/797)
npm warn deprecated debug@3.2.6: Debug versions >=3.2.0 <3.2.7 || >=4 <4.3.1 have a low-severity ReDos regression when used in a Node.js environment. It is recommended you upgrade to 3.2.7 or 4.3.1. (https://github.com/visionmedia/debug/issues/797)
npm warn deprecated chokidar@2.1.6: Chokidar 2 does not receive security updates since 2019. Upgrade to chokidar 3 with 15x fewer dependencies
npm warn deprecated sntp@0.2.4: This module moved to @hapi/sntp. Please make sure to switch over as this distribution is no longer supported and may contain bugs and critical security issues.
npm warn deprecated boom@2.10.1: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated minimatch@0.3.0: Please update to minimatch 3.0.2 or higher to avoid a RegExp DoS issue
npm warn deprecated chokidar@2.1.8: Chokidar 2 does not receive security updates since 2019. Upgrade to chokidar 3 with 15x fewer dependencies
npm warn deprecated sntp@1.0.9: This module moved to @hapi/sntp. Please make sure to switch over as this distribution is no longer supported and may contain bugs and critical security issues.
npm warn deprecated querystring@0.2.0: The querystring API is considered Legacy. new code should use the URLSearchParams API instead.
npm warn deprecated request@2.36.0: request has been deprecated, see https://github.com/request/request/issues/3142
npm warn deprecated mkdirp@0.3.0: Legacy versions of mkdirp are no longer supported. Please update to mkdirp 1.x. (Note that the API surface has changed to use Promises in 1.x.)
npm warn deprecated tough-cookie@2.2.2: ReDoS vulnerability parsing Set-Cookie https://nodesecurity.io/advisories/130
npm warn deprecated hoek@0.9.1: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated node-uuid@1.4.8: Use uuid module instead
npm warn deprecated node-uuid@1.4.8: Use uuid module instead
npm warn deprecated uuid@3.3.2: Please upgrade  to version 7 or higher.  Older versions may use Math.random() in certain circumstances, which is known to be problematic.  See https://v8.dev/blog/math-random for details.
npm warn deprecated source-map-resolve@0.5.2: See https://github.com/lydell/source-map-resolve#deprecated
npm warn deprecated har-validator@2.0.6: this library is no longer supported
npm warn deprecated mkdirp@0.5.1: Legacy versions of mkdirp are no longer supported. Please update to mkdirp 1.x. (Note that the API surface has changed to use Promises in 1.x.)
npm warn deprecated hoek@2.16.3: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated request@2.79.0: request has been deprecated, see https://github.com/request/request/issues/3142
npm warn deprecated request@2.88.0: request has been deprecated, see https://github.com/request/request/issues/3142
npm warn deprecated request@2.67.0: request has been deprecated, see https://github.com/request/request/issues/3142
npm warn deprecated readdir-scoped-modules@1.0.2: This functionality has been moved to @npmcli/fs
npm warn deprecated hawk@1.0.0: This module moved to @hapi/hawk. Please make sure to switch over as this distribution is no longer supported and may contain bugs and critical security issues.
npm warn deprecated hawk@3.1.3: This module moved to @hapi/hawk. Please make sure to switch over as this distribution is no longer supported and may contain bugs and critical security issues.
npm warn deprecated jade@0.26.3: Jade has been renamed to pug, please install the latest version of pug instead of jade
npm warn deprecated swig@1.4.2: This package is no longer maintained
npm warn deprecated bson@1.0.9: Fixed a critical issue with BSON serialization documented in CVE-2019-2391, see https://bit.ly/2KcpXdo for more details
npm warn deprecated nodeunit@0.9.5: you are strongly encouraged to use other testing options

added 962 packages, and audited 1412 packages in 12s

32 packages are looking for funding
  run `npm fund` for details

137 vulnerabilities (9 low, 35 moderate, 57 high, 36 critical)

To address issues that do not require attention, run:
  npm audit fix

To address all issues possible (including breaking changes), run:
  npm audit fix --force

Some issues need review, and may require choosing
a different dependency.

Run `npm audit` for details.
[Pipeline] }
[Pipeline] // dir
[Pipeline] }
[Pipeline] // script
[Pipeline] }
[Pipeline] // stage
[Pipeline] stage
[Pipeline] { (polaris-async-mode-scan)
[Pipeline] script
[Pipeline] {
[Pipeline] dir
Running in /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main@2/nodejs-npm
[Pipeline] {
[Pipeline] security_scan
**************************** START EXECUTION OF BLACK DUCK SECURITY SCAN ****************************
[Security Scan] INFO: Jenkins Job name: MBP_Github_Polaris_Async_Mode_Scan
-------------------------------- Connection to node --------------------------------
[Security Scan] INFO: Jenkins job is running on agent node remotely
-------------------------- Parameter Validation Initiated --------------------------
[Security Scan] INFO:  --- product = [POLARIS]
[Security Scan] INFO: Parameters for polaris:
[Security Scan] INFO:  --- polaris_waitForScan = false
[Security Scan] INFO:  --- polaris_server_url = https://poc.polaris.blackduck.com
[Security Scan] INFO:  --- polaris_assessment_types = SAST,SCA
[Security Scan] INFO:  --- polaris_access_token = ******************************************************************************
------------------------------------------------------------------------------------
[Security Scan] INFO: Parameters for additional configuration:
[Security Scan] INFO:  --- network_ssl_trustAll = false
[Security Scan] INFO:  --- network_airgap = false
[Security Scan] INFO: Polaris parameters are validated successfully
[Security Scan] INFO: Bridge download parameters are validated successfully
[Security Scan] INFO: Bridge download is not required. Found installed in: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm
------------------------------------------------------------------------------------
[Security Scan] INFO: Bridge CLI version is - 3.9.2
[Security Scan] INFO: Jenkins Job name: MBP_Github_Polaris_Async_Mode_Scan
[Security Scan] INFO: Polaris Application Name: async-mode
[Security Scan] INFO: Polaris Project Name: async-mode
[Security Scan] INFO: Polaris Branch Name: main
[Security Scan] INFO: Jenkins Job name: MBP_Github_Polaris_Async_Mode_Scan
[Security Scan] INFO: Executable command line arguments: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm/bridge-cli --stage polaris --input /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main@2/polaris_input2297059410956767203.json --out .bridge/output/scan_info_out.json

******************************* START EXECUTION OF BRIDGE CLI *******************************
2025-11-13 20:29:58.5117 IST [Bridge CLI] INFO: Using cache directory: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm
2025-11-13 20:29:58.5167 IST [Bridge CLI] INFO: Found version "3.0.371" in registry for workflow "polaris", trying to load it from local cache
2025-11-13 20:29:59.8423 IST [Bridge CLI] INFO: Input Resources:
2025-11-13 20:29:59.8424 IST [Bridge CLI] INFO: resource = value [source]
2025-11-13 20:29:59.8424 IST [Bridge CLI] INFO: ------------------------------------------------------------
2025-11-13 20:29:59.8424 IST [Bridge CLI] INFO: network.airgap = false [polaris_input2297059410956767203.json]
2025-11-13 20:29:59.8424 IST [Bridge CLI] INFO: network.ssl.trustAll = false [polaris_input2297059410956767203.json]
2025-11-13 20:29:59.8424 IST [Bridge CLI] INFO: polaris.accesstoken = ***************************************** [polaris_input2297059410956767203.json]
2025-11-13 20:29:59.8424 IST [Bridge CLI] INFO: polaris.application.name = async-mode [polaris_input2297059410956767203.json]
2025-11-13 20:29:59.8424 IST [Bridge CLI] INFO: polaris.assessment.types = [SAST SCA] [polaris_input2297059410956767203.json]
2025-11-13 20:29:59.8425 IST [Bridge CLI] INFO: polaris.branch.name = main [polaris_input2297059410956767203.json]
2025-11-13 20:29:59.8425 IST [Bridge CLI] INFO: polaris.project.name = async-mode [polaris_input2297059410956767203.json]
2025-11-13 20:29:59.8425 IST [Bridge CLI] INFO: polaris.serverUrl = https://poc.polaris.blackduck.com [polaris_input2297059410956767203.json]
2025-11-13 20:29:59.8425 IST [Bridge CLI] INFO: polaris.waitForScan = false [polaris_input2297059410956767203.json]
2025-11-13 20:29:59.8425 IST [Bridge CLI] INFO: ------------------------------------------------------------
2025-11-13 20:29:59.8425 IST [Bridge CLI] INFO: Starting adapters for stage polaris
2025-11-13 20:29:59.8444 IST [Bridge CLI] INFO: Starting Adapter: Polaris Status Provider
2025-11-13 20:29:59.8444 IST [Bridge CLI] INFO: Starting Adapter: Polaris Initializer
2025-11-13 20:29:59.8444 IST [Bridge CLI] INFO: Starting Adapter: Polaris SCM Discovery
2025-11-13 20:29:59.8444 IST [Bridge CLI] INFO: Starting Adapter: Polaris Controller
2025-11-13 20:29:59.9135 IST [Polaris SCM Discovery] INFO: Adapter finished
2025-11-13 20:29:59.9170 IST [Bridge CLI] INFO: Starting Adapter: Set Polaris Assessment Mode to CI
2025-11-13 20:29:59.9171 IST [Set Polaris Assessment Mode to CI] INFO: Provided value for resource 'polaris.assessment.mode'
2025-11-13 20:29:59.9172 IST [Set Polaris Assessment Mode to CI] INFO: Adapter finished
2025-11-13 20:29:59.9203 IST [Bridge CLI] INFO: Starting Adapter: Create Polaris Project & Branch By Default
2025-11-13 20:29:59.9204 IST [Create Polaris Project & Branch By Default] INFO: Provided value for resource 'polaris.onboarding'
2025-11-13 20:29:59.9204 IST [Create Polaris Project & Branch By Default] INFO: Adapter finished
2025-11-13 20:30:02.3863 IST [Polaris Initializer] INFO: Successfully created test for "SAST(sastFull)" assessment. The short test ID is "VUQO9R1"
2025-11-13 20:30:02.3952 IST [Polaris Initializer] INFO: Successfully created test for "SCA(scaPackage)" assessment. The short test ID is "K6VIXW1"
2025-11-13 20:30:02.4022 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.id'
2025-11-13 20:30:02.4024 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.id'
2025-11-13 20:30:02.4025 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.shortId'
2025-11-13 20:30:02.4027 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.shortId'
2025-11-13 20:30:02.4029 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.streamId'
2025-11-13 20:30:02.4032 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.project.id'
2025-11-13 20:30:02.4033 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.branch.id'
2025-11-13 20:30:02.4034 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.portfolioid'
2025-11-13 20:30:02.4035 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.tenant.id'
2025-11-13 20:30:02.4036 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.application.id'
2025-11-13 20:30:02.4039 IST [Polaris Initializer] INFO: Adapter finished
2025-11-13 20:30:02.4136 IST [Bridge CLI] INFO: Starting Adapter: Check pull request
2025-11-13 20:30:02.4481 IST [Check pull request] INFO: Provided value for resource 'environment.scan.pull'
2025-11-13 20:30:02.4482 IST [Check pull request] INFO: Adapter finished
2025-11-13 20:30:02.4923 IST [Polaris Controller] INFO: Running for "sast" assessment with scan type "sastFull"
2025-11-13 20:30:02.4927 IST [Polaris Controller] INFO: fetching recommended "coverity" tool info...
2025-11-13 20:30:03.2662 IST [Polaris Controller] INFO: checking "coverity" tool installation inside bridge home directory: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0
2025-11-13 20:30:03.2662 IST [Polaris Controller] INFO: Checking tool version for "cov_thin_client" in "/Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0"
2025-11-13 20:30:03.2663 IST [Polaris Controller] INFO: Running command:/Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/coverity --version
2025-11-13 20:30:03.2866 IST [Polaris Controller] INFO: Got tool version for "cov_thin_client": 2025.9.0
2025-11-13 20:30:03.5903 IST [Polaris Controller] INFO: "coverity" tool is already installed...
2025-11-13 20:30:03.5903 IST [Polaris Controller] INFO: fetching recommended "Sigma" tool info...
2025-11-13 20:30:03.9038 IST [Polaris Controller] INFO: checking "Sigma" tool installation inside bridge home directory: /Users/madhusud/.blackduck/bridge/tools/sigma/2025.10.0
2025-11-13 20:30:03.9039 IST [Polaris Controller] INFO: Checking tool version for "sigma" in "/Users/madhusud/.blackduck/bridge/tools/sigma/2025.10.0"
2025-11-13 20:30:03.9039 IST [Polaris Controller] INFO: Running command:/Users/madhusud/.blackduck/bridge/tools/sigma/2025.10.0/sigma --version
2025-11-13 20:30:03.9389 IST [Polaris Controller] INFO: Got tool version for "sigma": 2025.10.0
2025-11-13 20:30:04.2377 IST [Polaris Controller] INFO: "Sigma" tool is already installed...
2025-11-13 20:30:04.2377 IST [Polaris Controller] INFO: Running for "sca" assessment with scan type "scaPackage"
2025-11-13 20:30:04.2377 IST [Polaris Controller] INFO: fetching recommended "detect" tool info...
2025-11-13 20:30:04.5887 IST [Polaris Controller] INFO: checking "detect" tool installation inside bridge home directory: /Users/madhusud/.blackduck/bridge/tools/blackduck-detect/10.4.0
2025-11-13 20:30:04.5888 IST [Polaris Controller] INFO: Running command:/Library/Java/JavaVirtualMachines/jdk-21.jdk/Contents/Home/bin/java -version
2025-11-13 20:30:04.6217 IST [Polaris Controller] INFO: Checking tool version for "detect" in "/Users/madhusud/.blackduck/bridge/tools/blackduck-detect/10.4.0"
2025-11-13 20:30:04.6240 IST [Polaris Controller] INFO: Got tool version for "detect": 10.4.0
2025-11-13 20:30:04.9228 IST [Polaris Controller] INFO: "detect" tool is already installed...
2025-11-13 20:30:04.9228 IST [Polaris Controller] INFO: Scan is configured to run asynchronously, Bridge will not wait for the scan to complete.
2025-11-13 20:30:04.9293 IST [Polaris Controller] INFO: Provided value for resource 'coverity.id'
2025-11-13 20:30:04.9294 IST [Polaris Controller] INFO: Provided value for resource 'sigma.id'
2025-11-13 20:30:04.9295 IST [Polaris Controller] INFO: Provided value for resource 'detect.id'
2025-11-13 20:30:04.9296 IST [Bridge CLI] INFO: Starting adapters for stage polaris-sast
2025-11-13 20:30:04.9296 IST [Bridge CLI] INFO: Starting adapters for stage polaris-sca-package
2025-11-13 20:30:04.9296 IST [Bridge CLI] INFO: Starting adapters for stage polaris-artifacts-uploader
2025-11-13 20:30:04.9303 IST [Bridge CLI] INFO: Starting Adapter: Polaris SCA Package Manager Scan
2025-11-13 20:30:04.9303 IST [Bridge CLI] INFO: Starting Adapter: Polaris Coverity Capture
2025-11-13 20:30:04.9303 IST [Bridge CLI] INFO: Starting Adapter: Polaris Artifacts Uploader
2025-11-13 20:30:04.9305 IST [Polaris Controller] INFO: Adapter finished
2025-11-13 20:30:04.9440 IST [Bridge CLI] INFO: Starting Adapter: Default Adapter for execution path
2025-11-13 20:30:04.9443 IST [Default Adapter for execution path] INFO: Provided value for resource 'coverity.execution.path'
2025-11-13 20:30:04.9444 IST [Default Adapter for execution path] INFO: Adapter finished
2025-11-13 20:30:04.9493 IST [Bridge CLI] INFO: Starting Adapter: Default Adapter for execution path
2025-11-13 20:30:04.9494 IST [Default Adapter for execution path] INFO: Provided value for resource 'sigma.execution.path'
2025-11-13 20:30:04.9495 IST [Default Adapter for execution path] INFO: Adapter finished
2025-11-13 20:30:04.9908 IST [Polaris Coverity Capture] INFO: Identified workflow: Polaris
2025-11-13 20:30:04.9913 IST [Polaris Coverity Capture] INFO: command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/coverity capture --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir -o analyze.location=connect
2025-11-13 20:30:05.0460 IST [Polaris Coverity Capture] INFO: coverity 2025.9.0 covcli-2025.9-push-12
2025-11-13 20:30:05.0460 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CACHE_API_TOKEN_FILE=/var/folders/wm/gkd75sk54h57yqd0_j95gp2r0000gn/T/polaris_coverity_cache2028491458/.authKey
2025-11-13 20:30:05.0461 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CACHE_KEY=673c666f-5f9a-4514-b30a-9817bd0c02b1
2025-11-13 20:30:05.0461 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CACHE_URL=https://poc.polaris.blackduck.com/api/cache
2025-11-13 20:30:05.0461 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CLI_CAPTURE_ZIP_ARCHIVE=/Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/idir.zip
2025-11-13 20:30:05.0461 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CLI_POLARIS_CLIENT=true
2025-11-13 20:30:05.0463 IST [Polaris Coverity Capture] INFO: Detected that stdout is not connected to a terminal.  Defaulting ticker mode to 'none'.
2025-11-13 20:30:05.0464 IST [Polaris Coverity Capture] INFO: If this is not correct, explicitly set the ticker mode to the desired value using the '--ticker-mode' option.
2025-11-13 20:30:05.0473 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir create
2025-11-13 20:30:05.0728 IST [Polaris Coverity Capture] INFO: Using lightweight capture with thin client.
2025-11-13 20:30:05.0730 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-internal-manage-cache check
2025-11-13 20:30:05.9004 IST [Polaris Coverity Capture] INFO: Caching is enabled.
2025-11-13 20:30:05.9019 IST [Polaris Coverity Capture] INFO: Telemetry is enabled
2025-11-13 20:30:06.3687 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir list-capture-diagnostics
2025-11-13 20:30:06.3822 IST [Polaris Coverity Capture] INFO: Executing action no-op: nothing to do for initialization
2025-11-13 20:30:06.8498 IST [Polaris Coverity Capture] INFO: Executing action Delete compiler configurations for intermediate directory '/Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir'
2025-11-13 20:30:06.8498 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler gcc --comptype clangcc --template
2025-11-13 20:30:07.0857 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler cc --comptype gcc --template
2025-11-13 20:30:07.3162 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler c++ --comptype g++ --template
2025-11-13 20:30:07.5451 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler clang --comptype clangcc --template
2025-11-13 20:30:07.7849 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler java --comptype java --template
2025-11-13 20:30:08.0367 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler go --comptype go --template
2025-11-13 20:30:08.2753 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler ccache --comptype prefix --template
2025-11-13 20:30:08.5148 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler kotlinc --comptype kotlinc --template
2025-11-13 20:30:08.7508 IST [Polaris Coverity Capture] WARNING: Template config template-java-config-0 already exists for java and will be reused. 
2025-11-13 20:30:08.7508 IST [Polaris Coverity Capture] WARNING: Template config template-apt-config-0 already exists for apt and will be reused. 
2025-11-13 20:30:08.7508 IST [Polaris Coverity Capture] WARNING: Template config template-javaw-config-0 already exists for javaw and will be reused. 
2025-11-13 20:30:08.7558 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --dart
2025-11-13 20:30:09.0012 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --javascript
2025-11-13 20:30:09.2484 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --php
2025-11-13 20:30:09.4896 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --python
2025-11-13 20:30:09.7429 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --ruby
2025-11-13 20:30:09.9794 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --comptype capture-config-files --file-regex $capture-config-files$ --template
2025-11-13 20:30:09.9969 IST [Polaris Coverity Capture] WARNING: Configuration already exists for file regex $capture-config-files$
2025-11-13 20:30:09.9969 IST [Polaris Coverity Capture] INFO:           and it will not be updated.
2025-11-13 20:30:10.4555 IST [Polaris Coverity Capture] INFO: Executing action no-op: no compilers need to be unconfigured
2025-11-13 20:30:10.8708 IST [Polaris Coverity Capture] INFO: Executing action no-op: compiler configurations loaded
2025-11-13 20:30:11.4160 IST [Polaris Coverity Capture] INFO: Executing action Emit files using buildless capture: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-internal-capture-files --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --ticker-mode none --append-log --capture-list-file /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/capture-file-list-564853495 --record-with-source
2025-11-13 20:30:11.4286 IST [Polaris Coverity Capture] INFO: Buildless capture started.
2025-11-13 20:30:11.4381 IST [Polaris Coverity Capture] INFO: Emitting 84 Files.
2025-11-13 20:30:11.8831 IST [Polaris Coverity Capture] INFO: Buildless capture completed.
2025-11-13 20:30:11.8849 IST [Polaris Coverity Capture] INFO: Executing action No unwanted TUs to delete
2025-11-13 20:30:11.8849 IST [Polaris Coverity Capture] INFO: Executing action Action cleanup: Unwanted TUs action cleanup
2025-11-13 20:30:11.8851 IST [Polaris Coverity Capture] INFO: Executing action deleteResidualTUs /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir
2025-11-13 20:30:11.8854 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir list-capture-diagnostics
2025-11-13 20:30:11.9043 IST [Polaris Coverity Capture] INFO: Executing action Invalidate capture results
2025-11-13 20:30:11.9043 IST [Polaris Coverity Capture] INFO: Executing action Invoke cov-run-sigma: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-run-sigma --project-dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main@2/nodejs-npm --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir --coverity-config /var/folders/wm/gkd75sk54h57yqd0_j95gp2r0000gn/T/cov-run-sigma-config-2507234818/coverity.yaml --sigma-binary-path /Users/madhusud/.blackduck/bridge/tools/sigma/2025.10.0/sigma --enable-telemetry
2025-11-13 20:30:11.9206 IST [Polaris Coverity Capture] INFO: cov-run-sigma version 2025.9.0 on Darwin 24.6.0 arm64
2025-11-13 20:30:11.9207 IST [Polaris Coverity Capture] INFO: Internal version numbers: 477d3c5ddd p-2025.9-push-57
2025-11-13 20:30:11.9207 IST [Polaris Coverity Capture] INFO: 
2025-11-13 20:30:13.5069 IST [Polaris Coverity Capture] INFO: Executing action Action cleanup: Coverity configuration for Sigma
2025-11-13 20:30:13.9990 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir list-capture-diagnostics
2025-11-13 20:30:14.0550 IST [Polaris Coverity Capture] INFO: Capture summary:
2025-11-13 20:30:14.0550 IST [Polaris Coverity Capture] INFO:     SUCCEEDED: 87
2025-11-13 20:30:14.0550 IST [Polaris Coverity Capture] INFO:     INCOMPLETE: 0
2025-11-13 20:30:14.0551 IST [Polaris Coverity Capture] INFO:     FAILED: 0
2025-11-13 20:30:14.0551 IST [Polaris Coverity Capture] INFO:     IGNORED: 3
2025-11-13 20:30:14.0551 IST [Polaris Coverity Capture] INFO:     FILES CAPTURED: 87
2025-11-13 20:30:14.0551 IST [Polaris Coverity Capture] INFO:     LINES OF CODE: 32920
2025-11-13 20:30:14.0572 IST [Polaris Coverity Capture] INFO: Capture phase took 8.152s.
2025-11-13 20:30:14.0573 IST [Polaris Coverity Capture] WARNING: !! SOURCES FOR UNSUPPORTED LANGUAGES WERE DETECTED !!
2025-11-13 20:30:14.0573 IST [Polaris Coverity Capture] WARNING: 
2025-11-13 20:30:14.0573 IST [Polaris Coverity Capture] WARNING: Source files for the following languages were detected, but these languages are not supported on Mac OS ARM:
2025-11-13 20:30:14.0573 IST [Polaris Coverity Capture] WARNING:   * C#
2025-11-13 20:30:14.0573 IST [Polaris Coverity Capture] WARNING: In order to analyze these files, please analyze the project on an operating system and architecture where they are supported.
2025-11-13 20:30:14.0808 IST [Polaris Coverity Capture] INFO: To analyze your project, type '/Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/coverity analyze --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir -o analyze.location=connect'.
2025-11-13 20:30:14.0827 IST [Polaris Coverity Capture] INFO: Coverity Capture completed successfully
2025-11-13 20:30:14.0897 IST [Polaris Coverity Capture] INFO: Provided value for resource 'coverity.completed'
2025-11-13 20:30:14.0898 IST [Polaris Coverity Capture] INFO: Provided value for resource 'coverity.idir.output'
2025-11-13 20:30:14.0900 IST [Polaris Coverity Capture] INFO: Provided value for resource 'polaris.test.sast.tests.sastFull.artifacts.path'
2025-11-13 20:30:14.0902 IST [Polaris Coverity Capture] INFO: Adapter finished
2025-11-13 20:30:14.0921 IST [Bridge CLI] INFO: Starting Adapter: Default Adapter for execution path
2025-11-13 20:30:14.0922 IST [Default Adapter for execution path] INFO: Provided value for resource 'detect.execution.path'
2025-11-13 20:30:14.0922 IST [Default Adapter for execution path] INFO: Adapter finished
2025-11-13 20:30:14.1152 IST [Polaris SCA Package Manager Scan] INFO: Running command /Library/Java/JavaVirtualMachines/jdk-21.jdk/Contents/Home/bin/java -jar /Users/madhusud/.blackduck/bridge/tools/blackduck-detect/10.4.0/detect-10.4.0.jar --detect.cleanup=false --detect.bdio.file.name=scan --detect.bdio.output.path=/Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main@2/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/bdio/blackduck_artifact --detect.output.path=/Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main@2/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect --detect.tools=DETECTOR --detect.component.location.analysis.enabled=true --blackduck.offline.mode=true --blackduck.offline.mode.force.bdio=true
2025-11-13 20:30:14.0000 IST [Polaris SCA Package Manager Scan][main] WARNING: --- Detect-Self-Updater:  Self-Update feature is disabled because of the following reasons:
2025-11-13 20:30:14.0000 IST [Polaris SCA Package Manager Scan][main] WARNING: --- Detect-Self-Updater:  Detect in offline mode is incompatible with the Self-Update feature.
2025-11-13 20:30:14.0000 IST [Polaris SCA Package Manager Scan][main] WARNING: --- Detect-Self-Updater:  Black Duck URL is required for the Self-Update feature.
2025-11-13 20:30:14.8512 IST [Polaris SCA Package Manager Scan] INFO: ______     _            _
2025-11-13 20:30:14.8512 IST [Polaris SCA Package Manager Scan] INFO: |  _  \   | |          | |
2025-11-13 20:30:14.8513 IST [Polaris SCA Package Manager Scan] INFO: | | | |___| |_ ___  ___| |_
2025-11-13 20:30:14.8513 IST [Polaris SCA Package Manager Scan] INFO: | | | / _ \ __/ _ \/ __| __|
2025-11-13 20:30:14.8513 IST [Polaris SCA Package Manager Scan] INFO: | |/ /  __/ ||  __/ (__| |_
2025-11-13 20:30:14.8513 IST [Polaris SCA Package Manager Scan] INFO: |___/ \___|\__\___|\___|\__|
2025-11-13 20:30:14.8513 IST [Polaris SCA Package Manager Scan] INFO: 
2025-11-13 20:30:14.9738 IST [Polaris SCA Package Manager Scan] INFO: 
2025-11-13 20:30:14.9739 IST [Polaris SCA Package Manager Scan] INFO: Detect Version: 10.4.0
2025-11-13 20:30:14.9739 IST [Polaris SCA Package Manager Scan] INFO: 
2025-11-13 20:30:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 20:30:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Current property values:
2025-11-13 20:30:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- --property = value [notes]
2025-11-13 20:30:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ------------------------------------------------------------
2025-11-13 20:30:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- blackduck.offline.mode = true [cmd] 
2025-11-13 20:30:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- blackduck.offline.mode.force.bdio = true [cmd] 
2025-11-13 20:30:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.bdio.file.name = scan [cmd] 
2025-11-13 20:30:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.bdio.output.path = /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main@2/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/bdio/blackduck_artifact [cmd] 
2025-11-13 20:30:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.cleanup = false [cmd] 
2025-11-13 20:30:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.component.location.analysis.enabled = true [cmd] 
2025-11-13 20:30:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.excluded.directories = /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main@2/nodejs-npm/.bridge [env] 
2025-11-13 20:30:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.output.path = /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main@2/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect [cmd] 
2025-11-13 20:30:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.tools = DETECTOR [cmd] 
2025-11-13 20:30:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ------------------------------------------------------------
2025-11-13 20:30:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 20:30:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Detect build date: 2025-04-24
2025-11-13 20:30:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Source directory: /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main@2/nodejs-npm
2025-11-13 20:30:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Output directory: /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main@2/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect
2025-11-13 20:30:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Run directory: /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main@2/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-15-00-14-935
2025-11-13 20:30:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 20:30:15.0000 IST [Polaris SCA Package Manager Scan][main] WARNING: --- Correlated Scanning is not available for Rapid/Stateless scan mode or offline scanning. A correlation ID will not be set.
2025-11-13 20:30:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 20:30:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Docker tool will not be run.
2025-11-13 20:30:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 20:30:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Bazel tool will not be run.
2025-11-13 20:30:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 20:30:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Will include the Detectors tool.
2025-11-13 20:30:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Searching for detectors.
2025-11-13 20:30:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Evaluating detectors. This may take a while.
2025-11-13 20:30:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ======================================================================================================
2025-11-13 20:30:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Detector Report
2025-11-13 20:30:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ======================================================================================================
2025-11-13 20:30:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 	/Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main@2/nodejs-npm (depth 0)
2025-11-13 20:30:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 		NPM Package Lock: SUCCESS
2025-11-13 20:30:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 			Found file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main@2/nodejs-npm/package-lock.json
2025-11-13 20:30:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 			Found file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main@2/nodejs-npm/package.json
2025-11-13 20:30:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 20:30:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Detectors actions finished.
2025-11-13 20:30:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 20:30:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Project name: owasp-nodejs-goat
2025-11-13 20:30:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Project version: 1.3.0
2025-11-13 20:30:16.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 20:30:16.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Signature Scanner tool will not be run.
2025-11-13 20:30:16.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 20:30:16.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Vulnerability Impact Analysis tool will not be run.
2025-11-13 20:30:16.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 20:30:16.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- IaC Scanner tool will not be run.
2025-11-13 20:30:17.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 20:30:17.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ##################################################################################################
2025-11-13 20:30:17.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #                                                                                                #
2025-11-13 20:30:17.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  Product Notice                                                                                #
2025-11-13 20:30:17.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  © 2024 Black Duck Software, Inc.                                                              #
2025-11-13 20:30:17.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  This Black Duck Component Locator and all associated documentation are proprietary            #
2025-11-13 20:30:17.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  to Black Duck Software, Inc. and may only be used pursuant to the terms and conditions of a   #
2025-11-13 20:30:17.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  written license agreement with Black Duck Software, Inc. All other use, reproduction,         #
2025-11-13 20:30:17.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  modification, or distribution of the Black Duck Component Locator or the associated           #
2025-11-13 20:30:17.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  documentation is strictly prohibited.                                                         #
2025-11-13 20:30:17.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #                                                                                                #
2025-11-13 20:30:17.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ##################################################################################################
2025-11-13 20:30:17.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Running Component Locator v1.1.12 on /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main@2/nodejs-npm
2025-11-13 20:30:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Component Location Analysis file saved at: /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main@2/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-15-00-14-935/scan/components-with-locations.json
2025-11-13 20:30:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 20:30:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 20:30:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 20:30:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Creating status file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main@2/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-15-00-14-935/status/status.json
2025-11-13 20:30:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 20:30:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Skipping cleanup, it is disabled.
2025-11-13 20:30:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 20:30:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 20:30:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ======== Detect Result ========
2025-11-13 20:30:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 20:30:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Component Location Analysis File: /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main@2/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-15-00-14-935/scan/components-with-locations.json
2025-11-13 20:30:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 20:30:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ======== Detect Status ========
2025-11-13 20:30:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 20:30:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- NPM: SUCCESS
2025-11-13 20:30:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Overall Status: SUCCESS - Detect exited successfully.
2025-11-13 20:30:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 20:30:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ===============================
2025-11-13 20:30:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 20:30:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Detect duration: 00h 00m 44s 728ms
2025-11-13 20:30:59.1759 IST [Polaris SCA Package Manager Scan] INFO: Provided value for resource 'detect.completed'
2025-11-13 20:30:59.1761 IST [Polaris SCA Package Manager Scan] INFO: Provided value for resource 'polaris.test.sca.tests.scaPackage.artifacts.path'
2025-11-13 20:30:59.1762 IST [Polaris SCA Package Manager Scan] INFO: Adapter finished
2025-11-13 20:30:59.2008 IST [Polaris Artifacts Uploader] INFO: uploading artifact for "SAST(sastFull)" assessment with id "d0a6ab8f-ecc1-49bd-a4cd-121b49745763"
2025-11-13 20:30:59.2011 IST [Polaris Artifacts Uploader] INFO: uploading artifact for "SCA(scaPackage)" assessment with id "40984352-521c-4054-849a-7832bfa10e4e"
2025-11-13 20:31:00.5671 IST [Polaris Artifacts Uploader] INFO: Uploading artifact /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/idir.zip for "SAST(sastFull)" assessment
2025-11-13 20:31:00.5677 IST [Polaris Artifacts Uploader] INFO: Uploading artifact /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main@2/nodejs-npm/.bridge/polaris_sca_package_manager_scan/blackduck-sca-artifacts.zip for "SCA(scaPackage)" assessment
2025-11-13 20:31:01.0199 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact:   7%  16384/208045
2025-11-13 20:31:01.0315 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact:   4%  16384/383867
2025-11-13 20:31:01.2433 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact:  39%  81920/208045
2025-11-13 20:31:01.2463 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact:  70%  147456/208045
2025-11-13 20:31:01.2472 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact:  29%  114688/383867
2025-11-13 20:31:01.7607 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact: 100%  208045/208045
2025-11-13 20:31:01.7680 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact:  55%  212992/383867
2025-11-13 20:31:01.7704 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact:  81%  311296/383867
2025-11-13 20:31:01.9938 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact: 100%  383867/383867
2025-11-13 20:31:02.2651 IST [Polaris Artifacts Uploader] INFO: successfully uploaded artifact "/Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main@2/nodejs-npm/.bridge/polaris_sca_package_manager_scan/blackduck-sca-artifacts.zip"
2025-11-13 20:31:02.5091 IST [Polaris Artifacts Uploader] INFO: successfully uploaded artifact "/Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Polaris_Async_Mode_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/idir.zip"
2025-11-13 20:31:02.7778 IST [Polaris Artifacts Uploader] INFO: successfully resumed "SCA(scaPackage)" assessment with id "40984352-521c-4054-849a-7832bfa10e4e"
2025-11-13 20:31:03.0853 IST [Polaris Artifacts Uploader] INFO: successfully resumed "SAST(sastFull)" assessment with id "d0a6ab8f-ecc1-49bd-a4cd-121b49745763"
2025-11-13 20:31:03.1169 IST [Polaris Artifacts Uploader] INFO: Provided value for resource 'polaris.test.sast.tests.sastFull.artifacts.uploadSuccessful'
2025-11-13 20:31:03.1174 IST [Polaris Artifacts Uploader] INFO: Provided value for resource 'polaris.test.sca.tests.scaPackage.artifacts.uploadSuccessful'
2025-11-13 20:31:03.1181 IST [Polaris Artifacts Uploader] INFO: Adapter finished
2025-11-13 20:31:03.1845 IST [Polaris Status Provider] INFO: Results for test "SAST(sastFull)" with ID "d0a6ab8f-ecc1-49bd-a4cd-121b49745763" will be available at https://poc.polaris.blackduck.com/portfolio/portfolios/edf596d3-b54f-4a6b-9e5c-209f2e526c67/portfolio-items/f6f40d05-1268-4824-a147-bd35b7506448/projects/e684c68e-3360-40f9-8953-62fcc9d0e027/tests/d0a6ab8f-ecc1-49bd-a4cd-121b49745763/detected-issues after successful completion of scan
2025-11-13 20:31:03.1851 IST [Polaris Status Provider] INFO: Results for test "SCA(scaPackage)" with ID "40984352-521c-4054-849a-7832bfa10e4e" will be available at https://poc.polaris.blackduck.com/portfolio/portfolios/edf596d3-b54f-4a6b-9e5c-209f2e526c67/portfolio-items/f6f40d05-1268-4824-a147-bd35b7506448/projects/e684c68e-3360-40f9-8953-62fcc9d0e027/tests/40984352-521c-4054-849a-7832bfa10e4e/detected-issues after successful completion of scan
2025-11-13 20:31:03.1851 IST [Polaris Status Provider] INFO: "SAST(sastFull)" test with ID "VUQO9R1" & "SCA(scaPackage)" test with ID "K6VIXW1" are queued, you can track the status of the tests at https://poc.polaris.blackduck.com/scans/tests
2025-11-13 20:31:03.1851 IST [Polaris Status Provider] INFO: Polaris issues view for project "async-mode", branch "main" will be available at https://poc.polaris.blackduck.com/portfolio/portfolios/edf596d3-b54f-4a6b-9e5c-209f2e526c67/portfolio-items/f6f40d05-1268-4824-a147-bd35b7506448/projects/e684c68e-3360-40f9-8953-62fcc9d0e027/issues?branchId=7e8ffa23-8d7b-46ec-9991-911babeaca87 after successful completion of scan
2025-11-13 20:31:03.1950 IST [Polaris Status Provider] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.summary.url'
2025-11-13 20:31:03.1953 IST [Polaris Status Provider] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.summary.url'
2025-11-13 20:31:03.1955 IST [Polaris Status Provider] INFO: Provided value for resource 'polaris.project.issues.url'
2025-11-13 20:31:03.1958 IST [Polaris Status Provider] INFO: Adapter finished
******************************* END EXECUTION OF BRIDGE CLI *******************************
[Security Scan] INFO: Retrieving the issue count from the scan results
[Security Scan] INFO: Total issues found: 0
[Security Scan] INFO: Security Scan execution is successful
**************************** END EXECUTION OF BLACK DUCK SECURITY SCAN ****************************
[Pipeline] }
[Pipeline] // dir
[Pipeline] }
[Pipeline] // script
[Pipeline] }
[Pipeline] // stage
[Pipeline] stage
[Pipeline] { (Declarative: Post Actions)
[Pipeline] echo
Black Duck Logs Publisher - Starting log upload process
[Pipeline] echo
Configuration: [githubOrg:polaris-jenkins-samples, repoName:async-mode, credentialsId:github-pat-logs-publisher, maxRetries:3, retentionCount:5, jobNamePrefixes:[MBP_Github_, MBP_, Github_, Pipeline_, Job_, Build_]]
[Pipeline] echo
Job Name: MBP_Github_Polaris_Async_Mode_Scan/main
[Pipeline] echo
Build Number: 2
[Pipeline] echo
GitHub Organization: polaris-jenkins-samples
[Pipeline] withCredentials
Masking supported pattern matches of $GITHUB_TOKEN
[Pipeline] {
[Pipeline] echo
Using configured repository name: async-mode
[Pipeline] echo
Target repository: polaris-jenkins-samples/async-mode
[Pipeline] echo
LogProcessor: captureJenkinsLogs called
```

---

*Log generated by Black Duck Logs Publisher*