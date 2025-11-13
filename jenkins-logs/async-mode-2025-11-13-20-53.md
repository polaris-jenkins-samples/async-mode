# Jenkins Execution Log

## Build Information
- **Job Name:** `MBP_Github_Polaris_Async_Mode/main`
- **Build Number:** #3
- **Build Status:** 🟢 **SUCCESS**
- **Duration:** 1 min 44 sec and counting
- **Timestamp:** 2025-11-13 20:53:33 UTC

---

## Console Output

```
Started by user admin
Connecting to https://api.github.com using madhusud@blackduck.com/****** (Github_Username_PAT)
Obtained nodejs-npm/Jenkinsfile from a57b014b8efb3d2319c21f3fd58ce8143002a501
Loading library blackduck-logs-publisher@main
Attempting to resolve main from remote references...
 > git --version # timeout=10
 > git --version # 'git version 2.39.5 (Apple Git-154)'
using GIT_ASKPASS to set credentials Github_Username_PAT
 > git ls-remote -h -- https://github.com/integrations-garage/blackduck-logs-publisher # timeout=10
Found match: refs/heads/main revision e969196a63b1be83b84541b022f7aa52928bd5e5
The recommended git tool is: NONE
using credential Github_Username_PAT
 > git rev-parse --resolve-git-dir /Users/madhusud/.jenkins/workspace/P_Github_Polaris_Async_Mode_main@libs/a0dda568bac7bbb4a171f59ba3f2660c21c69edc6356524e9ae8bb4500c12bbb/.git # timeout=10
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
Running on mac-sh in /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Async_Mode_main
[Pipeline] {
[Pipeline] stage
[Pipeline] { (Declarative: Checkout SCM)
[Pipeline] checkout
The recommended git tool is: NONE
using credential Github_Username_PAT
Fetching changes from the remote Git repository
Fetching without tags
 > git rev-parse --resolve-git-dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Async_Mode_main/.git # timeout=10
 > git config remote.origin.url https://github.com/polaris-jenkins-samples/async-mode.git # timeout=10
Fetching upstream changes from https://github.com/polaris-jenkins-samples/async-mode.git
 > git --version # timeout=10
 > git --version # 'git version 2.39.5 (Apple Git-154)'
using GIT_ASKPASS to set credentials Github_Username_PAT
 > git fetch --no-tags --force --progress -- https://github.com/polaris-jenkins-samples/async-mode.git +refs/heads/main:refs/remotes/origin/main # timeout=10
Checking out Revision a57b014b8efb3d2319c21f3fd58ce8143002a501 (main)
Commit message: "Delete jenkins-logs directory"
 > git config core.sparsecheckout # timeout=10
 > git checkout -f a57b014b8efb3d2319c21f3fd58ce8143002a501 # timeout=10
 > git rev-list --no-walk 59c5fbc5f13c2102e91e526325d2a90f70cbb2a8 # timeout=10
[Pipeline] }
[Pipeline] // stage
[Pipeline] withEnv
[Pipeline] {
[Pipeline] stage
[Pipeline] { (Build)
[Pipeline] script
[Pipeline] {
[Pipeline] echo
JOB_NAME: MBP_Github_Polaris_Async_Mode/main
[Pipeline] dir
Running in /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Async_Mode_main/nodejs-npm
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

up to date, audited 1412 packages in 20s

32 packages are looking for funding
  run `npm fund` for details

136 vulnerabilities (9 low, 35 moderate, 57 high, 35 critical)

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
Running in /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Async_Mode_main/nodejs-npm
[Pipeline] {
[Pipeline] security_scan
**************************** START EXECUTION OF BLACK DUCK SECURITY SCAN ****************************
[Security Scan] INFO: Jenkins Job name: MBP_Github_Polaris_Async_Mode
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
[Security Scan] INFO: Jenkins Job name: MBP_Github_Polaris_Async_Mode
[Security Scan] INFO: Polaris Application Name: async-mode
[Security Scan] INFO: Polaris Project Name: async-mode
[Security Scan] INFO: Polaris Branch Name: main
[Security Scan] INFO: Jenkins Job name: MBP_Github_Polaris_Async_Mode
[Security Scan] INFO: Executable command line arguments: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm/bridge-cli --stage polaris --input /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Async_Mode_main/polaris_input5617043213963479501.json --out .bridge/output/scan_info_out.json

******************************* START EXECUTION OF BRIDGE CLI *******************************
2025-11-13 20:52:24.7834 IST [Bridge CLI] INFO: Using cache directory: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm
2025-11-13 20:52:24.7917 IST [Bridge CLI] INFO: Found version "3.0.371" in registry for workflow "polaris", trying to load it from local cache
2025-11-13 20:52:26.0661 IST [Bridge CLI] INFO: Input Resources:
2025-11-13 20:52:26.0662 IST [Bridge CLI] INFO: resource = value [source]
2025-11-13 20:52:26.0662 IST [Bridge CLI] INFO: ------------------------------------------------------------
2025-11-13 20:52:26.0662 IST [Bridge CLI] INFO: network.airgap = false [polaris_input5617043213963479501.json]
2025-11-13 20:52:26.0662 IST [Bridge CLI] INFO: network.ssl.trustAll = false [polaris_input5617043213963479501.json]
2025-11-13 20:52:26.0690 IST [Bridge CLI] INFO: polaris.accesstoken = ***************************************** [polaris_input5617043213963479501.json]
2025-11-13 20:52:26.0690 IST [Bridge CLI] INFO: polaris.application.name = async-mode [polaris_input5617043213963479501.json]
2025-11-13 20:52:26.0690 IST [Bridge CLI] INFO: polaris.assessment.types = [SAST SCA] [polaris_input5617043213963479501.json]
2025-11-13 20:52:26.0690 IST [Bridge CLI] INFO: polaris.branch.name = main [polaris_input5617043213963479501.json]
2025-11-13 20:52:26.0690 IST [Bridge CLI] INFO: polaris.project.name = async-mode [polaris_input5617043213963479501.json]
2025-11-13 20:52:26.0691 IST [Bridge CLI] INFO: polaris.serverUrl = https://poc.polaris.blackduck.com [polaris_input5617043213963479501.json]
2025-11-13 20:52:26.0691 IST [Bridge CLI] INFO: polaris.waitForScan = false [polaris_input5617043213963479501.json]
2025-11-13 20:52:26.0691 IST [Bridge CLI] INFO: ------------------------------------------------------------
2025-11-13 20:52:26.0691 IST [Bridge CLI] INFO: Starting adapters for stage polaris
2025-11-13 20:52:26.0715 IST [Bridge CLI] INFO: Starting Adapter: Polaris Status Provider
2025-11-13 20:52:26.0715 IST [Bridge CLI] INFO: Starting Adapter: Polaris SCM Discovery
2025-11-13 20:52:26.0715 IST [Bridge CLI] INFO: Starting Adapter: Polaris Initializer
2025-11-13 20:52:26.0715 IST [Bridge CLI] INFO: Starting Adapter: Polaris Controller
2025-11-13 20:52:26.1448 IST [Polaris SCM Discovery] INFO: Adapter finished
2025-11-13 20:52:26.1483 IST [Bridge CLI] INFO: Starting Adapter: Set Polaris Assessment Mode to CI
2025-11-13 20:52:26.1485 IST [Set Polaris Assessment Mode to CI] INFO: Provided value for resource 'polaris.assessment.mode'
2025-11-13 20:52:26.1485 IST [Set Polaris Assessment Mode to CI] INFO: Adapter finished
2025-11-13 20:52:26.1519 IST [Bridge CLI] INFO: Starting Adapter: Create Polaris Project & Branch By Default
2025-11-13 20:52:26.1520 IST [Create Polaris Project & Branch By Default] INFO: Provided value for resource 'polaris.onboarding'
2025-11-13 20:52:26.1521 IST [Create Polaris Project & Branch By Default] INFO: Adapter finished
2025-11-13 20:52:28.5046 IST [Polaris Initializer] INFO: Successfully created test for "SCA(scaPackage)" assessment. The short test ID is "ZZIHEAC"
2025-11-13 20:52:28.5187 IST [Polaris Initializer] INFO: Successfully created test for "SAST(sastFull)" assessment. The short test ID is "DHC20MO"
2025-11-13 20:52:28.5382 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.id'
2025-11-13 20:52:28.5386 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.id'
2025-11-13 20:52:28.5390 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.shortId'
2025-11-13 20:52:28.5395 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.shortId'
2025-11-13 20:52:28.5399 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.streamId'
2025-11-13 20:52:28.5402 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.project.id'
2025-11-13 20:52:28.5404 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.branch.id'
2025-11-13 20:52:28.5409 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.portfolioid'
2025-11-13 20:52:28.5412 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.tenant.id'
2025-11-13 20:52:28.5415 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.application.id'
2025-11-13 20:52:28.5421 IST [Polaris Initializer] INFO: Adapter finished
2025-11-13 20:52:28.5552 IST [Bridge CLI] INFO: Starting Adapter: Check pull request
2025-11-13 20:52:28.5937 IST [Check pull request] INFO: Provided value for resource 'environment.scan.pull'
2025-11-13 20:52:28.5941 IST [Check pull request] INFO: Adapter finished
2025-11-13 20:52:28.6398 IST [Polaris Controller] INFO: Running for "sca" assessment with scan type "scaPackage"
2025-11-13 20:52:28.6401 IST [Polaris Controller] INFO: fetching recommended "detect" tool info...
2025-11-13 20:52:29.4260 IST [Polaris Controller] INFO: checking "detect" tool installation inside bridge home directory: /Users/madhusud/.blackduck/bridge/tools/blackduck-detect/10.4.0
2025-11-13 20:52:29.4263 IST [Polaris Controller] INFO: Running command:/Library/Java/JavaVirtualMachines/jdk-21.jdk/Contents/Home/bin/java -version
2025-11-13 20:52:29.4939 IST [Polaris Controller] INFO: Checking tool version for "detect" in "/Users/madhusud/.blackduck/bridge/tools/blackduck-detect/10.4.0"
2025-11-13 20:52:29.4977 IST [Polaris Controller] INFO: Got tool version for "detect": 10.4.0
2025-11-13 20:52:29.7937 IST [Polaris Controller] INFO: "detect" tool is already installed...
2025-11-13 20:52:29.7939 IST [Polaris Controller] INFO: Running for "sast" assessment with scan type "sastFull"
2025-11-13 20:52:29.7939 IST [Polaris Controller] INFO: fetching recommended "coverity" tool info...
2025-11-13 20:52:30.0901 IST [Polaris Controller] INFO: checking "coverity" tool installation inside bridge home directory: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0
2025-11-13 20:52:30.0904 IST [Polaris Controller] INFO: Checking tool version for "cov_thin_client" in "/Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0"
2025-11-13 20:52:30.0919 IST [Polaris Controller] INFO: Running command:/Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/coverity --version
2025-11-13 20:52:30.1858 IST [Polaris Controller] INFO: Got tool version for "cov_thin_client": 2025.9.0
2025-11-13 20:52:30.4753 IST [Polaris Controller] INFO: "coverity" tool is already installed...
2025-11-13 20:52:30.4755 IST [Polaris Controller] INFO: fetching recommended "Sigma" tool info...
2025-11-13 20:52:30.7959 IST [Polaris Controller] INFO: checking "Sigma" tool installation inside bridge home directory: /Users/madhusud/.blackduck/bridge/tools/sigma/2025.10.0
2025-11-13 20:52:30.7961 IST [Polaris Controller] INFO: Checking tool version for "sigma" in "/Users/madhusud/.blackduck/bridge/tools/sigma/2025.10.0"
2025-11-13 20:52:30.7982 IST [Polaris Controller] INFO: Running command:/Users/madhusud/.blackduck/bridge/tools/sigma/2025.10.0/sigma --version
2025-11-13 20:52:30.8731 IST [Polaris Controller] INFO: Got tool version for "sigma": 2025.10.0
2025-11-13 20:52:31.1577 IST [Polaris Controller] INFO: "Sigma" tool is already installed...
2025-11-13 20:52:31.1579 IST [Polaris Controller] INFO: Scan is configured to run asynchronously, Bridge will not wait for the scan to complete.
2025-11-13 20:52:31.1820 IST [Polaris Controller] INFO: Provided value for resource 'coverity.id'
2025-11-13 20:52:31.1822 IST [Polaris Controller] INFO: Provided value for resource 'sigma.id'
2025-11-13 20:52:31.1825 IST [Polaris Controller] INFO: Provided value for resource 'detect.id'
2025-11-13 20:52:31.1826 IST [Bridge CLI] INFO: Starting adapters for stage polaris-sca-package
2025-11-13 20:52:31.1826 IST [Bridge CLI] INFO: Starting adapters for stage polaris-sast
2025-11-13 20:52:31.1826 IST [Bridge CLI] INFO: Starting adapters for stage polaris-artifacts-uploader
2025-11-13 20:52:31.1842 IST [Bridge CLI] INFO: Starting Adapter: Polaris Coverity Capture
2025-11-13 20:52:31.1843 IST [Bridge CLI] INFO: Starting Adapter: Polaris Artifacts Uploader
2025-11-13 20:52:31.1842 IST [Bridge CLI] INFO: Starting Adapter: Polaris SCA Package Manager Scan
2025-11-13 20:52:31.1850 IST [Polaris Controller] INFO: Adapter finished
2025-11-13 20:52:31.2122 IST [Bridge CLI] INFO: Starting Adapter: Default Adapter for execution path
2025-11-13 20:52:31.2126 IST [Default Adapter for execution path] INFO: Provided value for resource 'coverity.execution.path'
2025-11-13 20:52:31.2126 IST [Default Adapter for execution path] INFO: Adapter finished
2025-11-13 20:52:31.2199 IST [Bridge CLI] INFO: Starting Adapter: Default Adapter for execution path
2025-11-13 20:52:31.2201 IST [Default Adapter for execution path] INFO: Provided value for resource 'sigma.execution.path'
2025-11-13 20:52:31.2201 IST [Default Adapter for execution path] INFO: Adapter finished
2025-11-13 20:52:31.2850 IST [Polaris Coverity Capture] INFO: Identified workflow: Polaris
2025-11-13 20:52:31.2857 IST [Polaris Coverity Capture] INFO: command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/coverity capture --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Async_Mode_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir -o analyze.location=connect
2025-11-13 20:52:31.3350 IST [Polaris Coverity Capture] INFO: coverity 2025.9.0 covcli-2025.9-push-12
2025-11-13 20:52:31.3351 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CACHE_API_TOKEN_FILE=/var/folders/wm/gkd75sk54h57yqd0_j95gp2r0000gn/T/polaris_coverity_cache1035890619/.authKey
2025-11-13 20:52:31.3351 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CACHE_KEY=673c666f-5f9a-4514-b30a-9817bd0c02b1
2025-11-13 20:52:31.3351 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CACHE_URL=https://poc.polaris.blackduck.com/api/cache
2025-11-13 20:52:31.3351 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CLI_CAPTURE_ZIP_ARCHIVE=/Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Async_Mode_main/nodejs-npm/.bridge/polaris_coverity_capture/idir.zip
2025-11-13 20:52:31.3351 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CLI_POLARIS_CLIENT=true
2025-11-13 20:52:31.3367 IST [Polaris Coverity Capture] INFO: Detected that stdout is not connected to a terminal.  Defaulting ticker mode to 'none'.
2025-11-13 20:52:31.3368 IST [Polaris Coverity Capture] INFO: If this is not correct, explicitly set the ticker mode to the desired value using the '--ticker-mode' option.
2025-11-13 20:52:31.3382 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Async_Mode_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir create
2025-11-13 20:52:31.4046 IST [Polaris Coverity Capture] INFO: Using lightweight capture with thin client.
2025-11-13 20:52:31.4049 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-internal-manage-cache check
2025-11-13 20:52:32.2474 IST [Polaris Coverity Capture] INFO: Caching is enabled.
2025-11-13 20:52:32.2509 IST [Polaris Coverity Capture] INFO: Telemetry is enabled
2025-11-13 20:52:33.1505 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Async_Mode_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir list-capture-diagnostics
2025-11-13 20:52:33.1667 IST [Polaris Coverity Capture] INFO: Executing action no-op: nothing to do for initialization
2025-11-13 20:52:33.5899 IST [Polaris Coverity Capture] INFO: Executing action Delete compiler configurations for intermediate directory '/Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Async_Mode_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir'
2025-11-13 20:52:33.5900 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Async_Mode_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler gcc --comptype clangcc --template
2025-11-13 20:52:33.8584 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Async_Mode_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler cc --comptype gcc --template
2025-11-13 20:52:34.1030 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Async_Mode_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler c++ --comptype g++ --template
2025-11-13 20:52:34.3476 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Async_Mode_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler clang --comptype clangcc --template
2025-11-13 20:52:34.5955 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Async_Mode_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler java --comptype java --template
2025-11-13 20:52:34.8480 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Async_Mode_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler go --comptype go --template
2025-11-13 20:52:35.1001 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Async_Mode_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler ccache --comptype prefix --template
2025-11-13 20:52:35.3660 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Async_Mode_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler kotlinc --comptype kotlinc --template
2025-11-13 20:52:35.6299 IST [Polaris Coverity Capture] WARNING: Template config template-java-config-0 already exists for java and will be reused. 
2025-11-13 20:52:35.6299 IST [Polaris Coverity Capture] WARNING: Template config template-apt-config-0 already exists for apt and will be reused. 
2025-11-13 20:52:35.6299 IST [Polaris Coverity Capture] WARNING: Template config template-javaw-config-0 already exists for javaw and will be reused. 
2025-11-13 20:52:35.6353 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Async_Mode_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --dart
2025-11-13 20:52:35.8723 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Async_Mode_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --javascript
2025-11-13 20:52:36.0967 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Async_Mode_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --php
2025-11-13 20:52:36.3284 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Async_Mode_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --python
2025-11-13 20:52:36.5790 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Async_Mode_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --ruby
2025-11-13 20:52:36.8128 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Async_Mode_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --comptype capture-config-files --file-regex $capture-config-files$ --template
2025-11-13 20:52:36.8285 IST [Polaris Coverity Capture] WARNING: Configuration already exists for file regex $capture-config-files$
2025-11-13 20:52:36.8285 IST [Polaris Coverity Capture] INFO:           and it will not be updated.
2025-11-13 20:52:37.2610 IST [Polaris Coverity Capture] INFO: Executing action no-op: no compilers need to be unconfigured
2025-11-13 20:52:37.6888 IST [Polaris Coverity Capture] INFO: Executing action no-op: compiler configurations loaded
2025-11-13 20:52:38.2436 IST [Polaris Coverity Capture] INFO: Executing action Emit files using buildless capture: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-internal-capture-files --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Async_Mode_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Async_Mode_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --ticker-mode none --append-log --capture-list-file /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Async_Mode_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/capture-file-list-2338622128 --record-with-source
2025-11-13 20:52:38.2743 IST [Polaris Coverity Capture] INFO: Buildless capture started.
2025-11-13 20:52:38.2916 IST [Polaris Coverity Capture] INFO: Emitting 84 Files.
2025-11-13 20:52:38.7800 IST [Polaris Coverity Capture] INFO: Buildless capture completed.
2025-11-13 20:52:38.7821 IST [Polaris Coverity Capture] INFO: Executing action No unwanted TUs to delete
2025-11-13 20:52:38.7821 IST [Polaris Coverity Capture] INFO: Executing action Action cleanup: Unwanted TUs action cleanup
2025-11-13 20:52:38.7822 IST [Polaris Coverity Capture] INFO: Executing action deleteResidualTUs /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Async_Mode_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir
2025-11-13 20:52:38.7824 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Async_Mode_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir list-capture-diagnostics
2025-11-13 20:52:38.8011 IST [Polaris Coverity Capture] INFO: Executing action Invalidate capture results
2025-11-13 20:52:38.8011 IST [Polaris Coverity Capture] INFO: Executing action Invoke cov-run-sigma: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-run-sigma --project-dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Async_Mode_main/nodejs-npm --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Async_Mode_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir --coverity-config /var/folders/wm/gkd75sk54h57yqd0_j95gp2r0000gn/T/cov-run-sigma-config-3716442836/coverity.yaml --sigma-binary-path /Users/madhusud/.blackduck/bridge/tools/sigma/2025.10.0/sigma --enable-telemetry
2025-11-13 20:52:38.8300 IST [Polaris Coverity Capture] INFO: cov-run-sigma version 2025.9.0 on Darwin 24.6.0 arm64
2025-11-13 20:52:38.8300 IST [Polaris Coverity Capture] INFO: Internal version numbers: 477d3c5ddd p-2025.9-push-57
2025-11-13 20:52:38.8300 IST [Polaris Coverity Capture] INFO: 
2025-11-13 20:52:40.0330 IST [Polaris Coverity Capture] INFO: Executing action Action cleanup: Coverity configuration for Sigma
2025-11-13 20:52:40.5072 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Async_Mode_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir list-capture-diagnostics
2025-11-13 20:52:40.5606 IST [Polaris Coverity Capture] INFO: Capture summary:
2025-11-13 20:52:40.5607 IST [Polaris Coverity Capture] INFO:     SUCCEEDED: 87
2025-11-13 20:52:40.5607 IST [Polaris Coverity Capture] INFO:     INCOMPLETE: 0
2025-11-13 20:52:40.5607 IST [Polaris Coverity Capture] INFO:     FAILED: 0
2025-11-13 20:52:40.5607 IST [Polaris Coverity Capture] INFO:     IGNORED: 3
2025-11-13 20:52:40.5607 IST [Polaris Coverity Capture] INFO:     FILES CAPTURED: 87
2025-11-13 20:52:40.5607 IST [Polaris Coverity Capture] INFO:     LINES OF CODE: 32920
2025-11-13 20:52:40.5627 IST [Polaris Coverity Capture] INFO: Capture phase took 8.316s.
2025-11-13 20:52:40.5627 IST [Polaris Coverity Capture] WARNING: !! SOURCES FOR UNSUPPORTED LANGUAGES WERE DETECTED !!
2025-11-13 20:52:40.5627 IST [Polaris Coverity Capture] WARNING: 
2025-11-13 20:52:40.5627 IST [Polaris Coverity Capture] WARNING: Source files for the following languages were detected, but these languages are not supported on Mac OS ARM:
2025-11-13 20:52:40.5627 IST [Polaris Coverity Capture] WARNING:   * C#
2025-11-13 20:52:40.5628 IST [Polaris Coverity Capture] WARNING: In order to analyze these files, please analyze the project on an operating system and architecture where they are supported.
2025-11-13 20:52:40.5840 IST [Polaris Coverity Capture] INFO: To analyze your project, type '/Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/coverity analyze --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Async_Mode_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir -o analyze.location=connect'.
2025-11-13 20:52:40.5857 IST [Polaris Coverity Capture] INFO: Coverity Capture completed successfully
2025-11-13 20:52:40.5926 IST [Polaris Coverity Capture] INFO: Provided value for resource 'coverity.completed'
2025-11-13 20:52:40.5927 IST [Polaris Coverity Capture] INFO: Provided value for resource 'coverity.idir.output'
2025-11-13 20:52:40.5929 IST [Polaris Coverity Capture] INFO: Provided value for resource 'polaris.test.sast.tests.sastFull.artifacts.path'
2025-11-13 20:52:40.5931 IST [Polaris Coverity Capture] INFO: Adapter finished
2025-11-13 20:52:40.5950 IST [Bridge CLI] INFO: Starting Adapter: Default Adapter for execution path
2025-11-13 20:52:40.5951 IST [Default Adapter for execution path] INFO: Provided value for resource 'detect.execution.path'
2025-11-13 20:52:40.5951 IST [Default Adapter for execution path] INFO: Adapter finished
2025-11-13 20:52:40.6262 IST [Polaris SCA Package Manager Scan] INFO: Running command /Library/Java/JavaVirtualMachines/jdk-21.jdk/Contents/Home/bin/java -jar /Users/madhusud/.blackduck/bridge/tools/blackduck-detect/10.4.0/detect-10.4.0.jar --detect.cleanup=false --detect.bdio.file.name=scan --detect.bdio.output.path=/Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Async_Mode_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/bdio/blackduck_artifact --detect.output.path=/Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Async_Mode_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect --detect.tools=DETECTOR --detect.component.location.analysis.enabled=true --blackduck.offline.mode=true --blackduck.offline.mode.force.bdio=true
2025-11-13 20:52:41.0000 IST [Polaris SCA Package Manager Scan][main] WARNING: --- Detect-Self-Updater:  Self-Update feature is disabled because of the following reasons:
2025-11-13 20:52:41.0000 IST [Polaris SCA Package Manager Scan][main] WARNING: --- Detect-Self-Updater:  Detect in offline mode is incompatible with the Self-Update feature.
2025-11-13 20:52:41.0000 IST [Polaris SCA Package Manager Scan][main] WARNING: --- Detect-Self-Updater:  Black Duck URL is required for the Self-Update feature.
2025-11-13 20:52:41.8443 IST [Polaris SCA Package Manager Scan] INFO: ______     _            _
2025-11-13 20:52:41.8444 IST [Polaris SCA Package Manager Scan] INFO: |  _  \   | |          | |
2025-11-13 20:52:41.8444 IST [Polaris SCA Package Manager Scan] INFO: | | | |___| |_ ___  ___| |_
2025-11-13 20:52:41.8444 IST [Polaris SCA Package Manager Scan] INFO: | | | / _ \ __/ _ \/ __| __|
2025-11-13 20:52:41.8444 IST [Polaris SCA Package Manager Scan] INFO: | |/ /  __/ ||  __/ (__| |_
2025-11-13 20:52:41.8444 IST [Polaris SCA Package Manager Scan] INFO: |___/ \___|\__\___|\___|\__|
2025-11-13 20:52:41.8445 IST [Polaris SCA Package Manager Scan] INFO: 
2025-11-13 20:52:41.9639 IST [Polaris SCA Package Manager Scan] INFO: 
2025-11-13 20:52:41.9640 IST [Polaris SCA Package Manager Scan] INFO: Detect Version: 10.4.0
2025-11-13 20:52:41.9640 IST [Polaris SCA Package Manager Scan] INFO: 
2025-11-13 20:52:41.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 20:52:41.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Current property values:
2025-11-13 20:52:41.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- --property = value [notes]
2025-11-13 20:52:41.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ------------------------------------------------------------
2025-11-13 20:52:41.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- blackduck.offline.mode = true [cmd] 
2025-11-13 20:52:41.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- blackduck.offline.mode.force.bdio = true [cmd] 
2025-11-13 20:52:41.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.bdio.file.name = scan [cmd] 
2025-11-13 20:52:41.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.bdio.output.path = /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Async_Mode_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/bdio/blackduck_artifact [cmd] 
2025-11-13 20:52:41.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.cleanup = false [cmd] 
2025-11-13 20:52:41.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.component.location.analysis.enabled = true [cmd] 
2025-11-13 20:52:41.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.excluded.directories = /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Async_Mode_main/nodejs-npm/.bridge [env] 
2025-11-13 20:52:41.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.output.path = /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Async_Mode_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect [cmd] 
2025-11-13 20:52:41.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.tools = DETECTOR [cmd] 
2025-11-13 20:52:41.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ------------------------------------------------------------
2025-11-13 20:52:41.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 20:52:41.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Detect build date: 2025-04-24
2025-11-13 20:52:42.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Source directory: /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Async_Mode_main/nodejs-npm
2025-11-13 20:52:42.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Output directory: /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Async_Mode_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect
2025-11-13 20:52:42.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Run directory: /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Async_Mode_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-15-22-41-928
2025-11-13 20:52:42.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 20:52:42.0000 IST [Polaris SCA Package Manager Scan][main] WARNING: --- Correlated Scanning is not available for Rapid/Stateless scan mode or offline scanning. A correlation ID will not be set.
2025-11-13 20:52:42.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 20:52:42.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Docker tool will not be run.
2025-11-13 20:52:42.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 20:52:42.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Bazel tool will not be run.
2025-11-13 20:52:42.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 20:52:42.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Will include the Detectors tool.
2025-11-13 20:52:42.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Searching for detectors.
2025-11-13 20:52:42.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Evaluating detectors. This may take a while.
2025-11-13 20:52:42.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ======================================================================================================
2025-11-13 20:52:42.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Detector Report
2025-11-13 20:52:42.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ======================================================================================================
2025-11-13 20:52:42.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 	/Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Async_Mode_main/nodejs-npm (depth 0)
2025-11-13 20:52:42.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 		NPM Package Lock: SUCCESS
2025-11-13 20:52:42.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 			Found file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Async_Mode_main/nodejs-npm/package-lock.json
2025-11-13 20:52:42.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 			Found file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Async_Mode_main/nodejs-npm/package.json
2025-11-13 20:52:42.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 20:52:42.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Detectors actions finished.
2025-11-13 20:52:42.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 20:52:42.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Project name: owasp-nodejs-goat
2025-11-13 20:52:42.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Project version: 1.3.0
2025-11-13 20:52:43.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 20:52:43.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Signature Scanner tool will not be run.
2025-11-13 20:52:43.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 20:52:43.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Vulnerability Impact Analysis tool will not be run.
2025-11-13 20:52:43.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 20:52:43.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- IaC Scanner tool will not be run.
2025-11-13 20:52:44.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 20:52:44.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ##################################################################################################
2025-11-13 20:52:44.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #                                                                                                #
2025-11-13 20:52:44.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  Product Notice                                                                                #
2025-11-13 20:52:44.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  © 2024 Black Duck Software, Inc.                                                              #
2025-11-13 20:52:44.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  This Black Duck Component Locator and all associated documentation are proprietary            #
2025-11-13 20:52:44.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  to Black Duck Software, Inc. and may only be used pursuant to the terms and conditions of a   #
2025-11-13 20:52:44.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  written license agreement with Black Duck Software, Inc. All other use, reproduction,         #
2025-11-13 20:52:44.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  modification, or distribution of the Black Duck Component Locator or the associated           #
2025-11-13 20:52:44.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  documentation is strictly prohibited.                                                         #
2025-11-13 20:52:44.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #                                                                                                #
2025-11-13 20:52:44.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ##################################################################################################
2025-11-13 20:52:44.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Running Component Locator v1.1.12 on /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Async_Mode_main/nodejs-npm
2025-11-13 20:53:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Component Location Analysis file saved at: /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Async_Mode_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-15-22-41-928/scan/components-with-locations.json
2025-11-13 20:53:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 20:53:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 20:53:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 20:53:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Creating status file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Async_Mode_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-15-22-41-928/status/status.json
2025-11-13 20:53:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 20:53:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Skipping cleanup, it is disabled.
2025-11-13 20:53:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 20:53:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 20:53:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ======== Detect Result ========
2025-11-13 20:53:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 20:53:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Component Location Analysis File: /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Async_Mode_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-15-22-41-928/scan/components-with-locations.json
2025-11-13 20:53:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 20:53:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ======== Detect Status ========
2025-11-13 20:53:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 20:53:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- NPM: SUCCESS
2025-11-13 20:53:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Overall Status: SUCCESS - Detect exited successfully.
2025-11-13 20:53:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 20:53:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ===============================
2025-11-13 20:53:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 20:53:27.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Detect duration: 00h 00m 46s 958ms
2025-11-13 20:53:27.9224 IST [Polaris SCA Package Manager Scan] INFO: Provided value for resource 'detect.completed'
2025-11-13 20:53:27.9225 IST [Polaris SCA Package Manager Scan] INFO: Provided value for resource 'polaris.test.sca.tests.scaPackage.artifacts.path'
2025-11-13 20:53:27.9227 IST [Polaris SCA Package Manager Scan] INFO: Adapter finished
2025-11-13 20:53:27.9588 IST [Polaris Artifacts Uploader] INFO: uploading artifact for "SAST(sastFull)" assessment with id "e311d502-124f-42c1-affe-1693cd552078"
2025-11-13 20:53:27.9592 IST [Polaris Artifacts Uploader] INFO: uploading artifact for "SCA(scaPackage)" assessment with id "eeb1ca3f-ca77-4261-911c-43802597b679"
2025-11-13 20:53:29.4958 IST [Polaris Artifacts Uploader] INFO: Uploading artifact /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Async_Mode_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/blackduck-sca-artifacts.zip for "SCA(scaPackage)" assessment
2025-11-13 20:53:29.5174 IST [Polaris Artifacts Uploader] INFO: Uploading artifact /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Async_Mode_main/nodejs-npm/.bridge/polaris_coverity_capture/idir.zip for "SAST(sastFull)" assessment
2025-11-13 20:53:30.1697 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact:   4%  16384/384178
2025-11-13 20:53:30.1741 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact:   7%  16384/208308
2025-11-13 20:53:30.3761 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact:  29%  114688/384178
2025-11-13 20:53:30.3800 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact:  39%  81920/208308
2025-11-13 20:53:30.3843 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact:  70%  147456/208308
2025-11-13 20:53:30.7925 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact:  55%  212992/384178
2025-11-13 20:53:30.8007 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact:  81%  311296/384178
2025-11-13 20:53:30.8008 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact: 100%  208308/208308
2025-11-13 20:53:31.0002 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact: 100%  384178/384178
2025-11-13 20:53:31.2916 IST [Polaris Artifacts Uploader] INFO: successfully uploaded artifact "/Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Async_Mode_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/blackduck-sca-artifacts.zip"
2025-11-13 20:53:31.4993 IST [Polaris Artifacts Uploader] INFO: successfully uploaded artifact "/Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_Polaris_Async_Mode_main/nodejs-npm/.bridge/polaris_coverity_capture/idir.zip"
2025-11-13 20:53:31.7821 IST [Polaris Artifacts Uploader] INFO: successfully resumed "SCA(scaPackage)" assessment with id "eeb1ca3f-ca77-4261-911c-43802597b679"
2025-11-13 20:53:31.9876 IST [Polaris Artifacts Uploader] INFO: successfully resumed "SAST(sastFull)" assessment with id "e311d502-124f-42c1-affe-1693cd552078"
2025-11-13 20:53:32.0086 IST [Polaris Artifacts Uploader] INFO: Provided value for resource 'polaris.test.sast.tests.sastFull.artifacts.uploadSuccessful'
2025-11-13 20:53:32.0104 IST [Polaris Artifacts Uploader] INFO: Provided value for resource 'polaris.test.sca.tests.scaPackage.artifacts.uploadSuccessful'
2025-11-13 20:53:32.0110 IST [Polaris Artifacts Uploader] INFO: Adapter finished
2025-11-13 20:53:32.0646 IST [Polaris Status Provider] INFO: Results for test "SAST(sastFull)" with ID "e311d502-124f-42c1-affe-1693cd552078" will be available at https://poc.polaris.blackduck.com/portfolio/portfolios/edf596d3-b54f-4a6b-9e5c-209f2e526c67/portfolio-items/f6f40d05-1268-4824-a147-bd35b7506448/projects/e684c68e-3360-40f9-8953-62fcc9d0e027/tests/e311d502-124f-42c1-affe-1693cd552078/detected-issues after successful completion of scan
2025-11-13 20:53:32.0651 IST [Polaris Status Provider] INFO: Results for test "SCA(scaPackage)" with ID "eeb1ca3f-ca77-4261-911c-43802597b679" will be available at https://poc.polaris.blackduck.com/portfolio/portfolios/edf596d3-b54f-4a6b-9e5c-209f2e526c67/portfolio-items/f6f40d05-1268-4824-a147-bd35b7506448/projects/e684c68e-3360-40f9-8953-62fcc9d0e027/tests/eeb1ca3f-ca77-4261-911c-43802597b679/detected-issues after successful completion of scan
2025-11-13 20:53:32.0651 IST [Polaris Status Provider] INFO: "SAST(sastFull)" test with ID "DHC20MO" & "SCA(scaPackage)" test with ID "ZZIHEAC" are queued, you can track the status of the tests at https://poc.polaris.blackduck.com/scans/tests
2025-11-13 20:53:32.0651 IST [Polaris Status Provider] INFO: Polaris issues view for project "async-mode", branch "main" will be available at https://poc.polaris.blackduck.com/portfolio/portfolios/edf596d3-b54f-4a6b-9e5c-209f2e526c67/portfolio-items/f6f40d05-1268-4824-a147-bd35b7506448/projects/e684c68e-3360-40f9-8953-62fcc9d0e027/issues?branchId=7e8ffa23-8d7b-46ec-9991-911babeaca87 after successful completion of scan
2025-11-13 20:53:32.0741 IST [Polaris Status Provider] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.summary.url'
2025-11-13 20:53:32.0744 IST [Polaris Status Provider] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.summary.url'
2025-11-13 20:53:32.0746 IST [Polaris Status Provider] INFO: Provided value for resource 'polaris.project.issues.url'
2025-11-13 20:53:32.0749 IST [Polaris Status Provider] INFO: Adapter finished
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
Job Name: MBP_Github_Polaris_Async_Mode/main
[Pipeline] echo
Build Number: 3
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