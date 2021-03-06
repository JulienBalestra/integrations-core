# CHANGELOG - Datadog Checks Dev

## 0.17.0 / 2019-01-07

* [Added] Use standalone py3 validation. See [#2854][1].
* [Fixed] Fix root folder name when running 'validate' commands on integrations-extras. See [#2879][2].
* [Fixed] Pin pytest because of a regression in pytest-benchmark. See [#2878][3].

## 0.16.0 / 2018-12-22

* [Added] Remove requirements.txt from check template. See [#2816][4].
* [Added] Add ability to log warnings during pytest. See [#2764][5].
* [Fixed] Fix agent_changelog command. See [#2808][6].
* [Added] Update templates for new integrations. See [#2794][7].
* [Added] Add python3 compatibility validation. See [#2736][8].
* [Added] Validate checks dependencies against the embedded environment. See [#2746][9].
* [Added] Add constant to check if platform is Linux. See [#2782][10].
* [Fixed] Do not consider empty string as a version change. See [#2771][11].
* [Changed] Rename `ddev release freeze` to `ddev release agent_req_file`, refactor commands code. See [#2765][12].
* [Added] Add validation for configuration files. See [#2759][13].
* [Added] Add ability to pass state to e2e tear down. See [#2724][14].
* [Added] Add ability to use dev version of base package for e2e. See [#2689][15].

## 0.15.1 / 2018-11-30

* [Fixed] Handle unreleased checks for agent reqs validation. See [#2664][16].

## 0.15.0 / 2018-11-27

* [Added] Added Watt units to metadata validation. See [#2645][17].
* [Added] Added Heap and Volume units to metadata validation. See [#2647][18].
* [Fixed] Gently handle Yubikey exceptions. See [#2641][19].
* [Added] Added validation step for the agent-requirements file. See [#2642][20].

## 0.14.1 / 2018-11-22

* [Fixed] Increase gpg timeout to give time to developers to interact with Yubikeys. See [#2613][21].
* [Fixed] Fix requirements-agent-release.txt updating. See [#2617][22].

## 0.14.0 / 2018-11-16

* [Added] Support agent repo. See [#2600][23].
* [Added] Improve trello releasing. See [#2599][24].
* [Added] Refactor validations under `validate` command. See [#2593][25].
* [Added] Upgrade docker-compose and requests. See [#2503][26].
* [Added] Disable pytest output capturing when debugging. See [#2502][27].
* [Added] Support specifying type of semver version bumps. See [#2491][28].
* [Fixed] Fixed off-by-one missing latest release. See [#2478][29].
* [Added] Fix codecov error on appveyor. See [#2474][30].
* [Fixed] Use raw string literals when \ is present. See [#2465][31].
* [Fixed] Improve output of `ddev manifest verify` command. See [#2444][32].
* [Added] Add service_checks.json files validation. See [#2432][33].
* [Added] Make all tox envs available to E2E. See [#2457][34].
* [Added] Ensure new checks include the E2E fixture. See [#2455][35].
* [Fixed] Handle any clipboard errors for E2E. See [#2454][36].
* [Added] Prevent misconfigured tox files. See [#2447][37].
* [Fixed] Add `datadog-` prefix to packages name. See [#2430][38].

## 0.13.0 / 2018-10-17

* [Added] Ensure new checks use editable install of datadog_checks_base for tests. See [#2427][39].
* [Fixed] Relax e2e config parsing. See [#2416][40].
* [Fixed] Fix sleep on WaitFor helper. See [#2418][41].

## 0.12.1 / 2018-10-15

* [Fixed] Improve handling of github api errors for trello. See [#2411][42].
* [Fixed] Make every check's `tests` directory path unique for coverage. See [#2406][43].

## 0.12.0 / 2018-10-15

* [Fixed] Fix trello for issue number in commit message. See [#2408][44].
* [Added] Support the initial release of integrations. See [#2399][45].

## 0.11.0 / 2018-10-11

* [Added] Add E2E support. See [#2375][46].
* [Added] Ensure new core checks use latest dev package for testing. See [#2386][47].
* [Fixed] Normalize line endings for release signing. See [#2364][48].
* [Added] Support more teams for Trello test cards. See [#2365][49].

## 0.10.0 / 2018-10-04

* [Added] Update base package paths. See [#2345][50].
* [Added] Add generic environment runner. See [#2342][51].
* [Added] Add WaitFor environment condition. See [#2343][52].
* [Added] Enable pytest plugin to control environments. See [#2336][53].

## 0.9.0 / 2018-09-30

* [Added] Allow testing of specific environments. See [#2312][54].
* [Added] Add run command. See [#2319][55].
* [Fixed] Fix namespace overwriting. See [#2311][56].
* [Fixed] Upgrade in-toto to gain full cross-platform release signing support. See [#2315][57].
* [Added] Command to validate metadata. See [#2269][58].

## 0.8.1 / 2018-09-25

* [Fixed] Fix Python 2 unicode handling for log pattern error message. See [#2303][59].

## 0.8.0 / 2018-09-25

* [Added] Add new templates for other integration types. See [#2285][60].
* [Added] Add release signing via in-toto. See [#2224][61].
* [Added] Add prometheus metadata.csv and metric map auto-generation. See [#2117][62].
* [Added] Keep track of the checks changed at every Datadog Agent release. See [#2277][63].

## 0.7.0 / 2018-09-18

* [Added] Fix manifest validation policy. See [#2258][64].
* [Added] Add config option to select the default repository. See [#2243][65].

## 0.6.2 / 2018-09-14

* [Fixed] Revert "Update base package paths (#2235)". See [#2240][66].

## 0.6.1 / 2018-09-14

* [Fixed] Move datadog_checks_base code into sub base package. See [#2167][67].

## 0.6.0 / 2018-09-14

* [Added] Update base package paths. See [#2235][68].
* [Added] Add ability to add wait time in docker_run. See [#2196][69].
* [Added] Add better debugging to test command. See [#2194][70].
* [Fixed] Gracefully handle tags that already exist. See [#2172][71].
* [Fixed] Fix release freeze command. See [#2188][72].
* [Added] Add ability to filter checks to test by changes. See [#2163][73].

## 0.5.0 / 2018-09-04

* [Added] Allow automated releasing by looking at github labels. See [#2169][74].
* [Fixed] Handle character limit for Trello card descriptions. See [#2162][75].

## 0.4.1 / 2018-08-31

* [Fixed] Fix trello command for other repos. See [#2155][76].

## 0.4.0 / 2018-08-28

* [Added] Add code coverage. See [#2105][77].
* [Added] Add command to create new integrations. See [#2037][78].

## 0.3.1 / 2018-08-03

* [Fixed] Fix clean command. See [#1992][79].

## 0.3.0 / 2018-07-30

* [Added] Allow passing --build to compose up. See [#1962][80].
* [Fixed] When setting repo paths do not resolve home. See [#1953][81].
* [Added] Add command to create Trello test cards from Agent release diffs. See [#1934][82].
* [Added] Add openldap to the list of agent integrations. See [#1923][83].
* [Added] Update dep tooling to support environment markers. See [#1921][84].

## 0.2.2 / 2018-07-19

* [Fixed] Relax condition error handling to allow more time. See [#1914][85].
* [Fixed] Do not skip release builds. See [#1913][86].
* [Fixed] Fix packaging of agent requirements. See [#1911][87].

## 0.2.1 / 2018-07-17

* [Fixed] make remove_path util more resilient to errors. See [#1900][88].

## 0.2.0 / 2018-07-17

* [Added] improve docker tooling. See [#1891][89].

## 0.1.1 / 2018-07-12

* [Fixed] fix changed-only test logic. See [#1878][90].

## 0.1.0 / 2018-07-12

* [Added] Add developer package. See [#1862][91].
[1]: https://github.com/DataDog/integrations-core/pull/2854
[2]: https://github.com/DataDog/integrations-core/pull/2879
[3]: https://github.com/DataDog/integrations-core/pull/2878
[4]: https://github.com/DataDog/integrations-core/pull/2816
[5]: https://github.com/DataDog/integrations-core/pull/2764
[6]: https://github.com/DataDog/integrations-core/pull/2808
[7]: https://github.com/DataDog/integrations-core/pull/2794
[8]: https://github.com/DataDog/integrations-core/pull/2736
[9]: https://github.com/DataDog/integrations-core/pull/2746
[10]: https://github.com/DataDog/integrations-core/pull/2782
[11]: https://github.com/DataDog/integrations-core/pull/2771
[12]: https://github.com/DataDog/integrations-core/pull/2765
[13]: https://github.com/DataDog/integrations-core/pull/2759
[14]: https://github.com/DataDog/integrations-core/pull/2724
[15]: https://github.com/DataDog/integrations-core/pull/2689
[16]: https://github.com/DataDog/integrations-core/pull/2664
[17]: https://github.com/DataDog/integrations-core/pull/2645
[18]: https://github.com/DataDog/integrations-core/pull/2647
[19]: https://github.com/DataDog/integrations-core/pull/2641
[20]: https://github.com/DataDog/integrations-core/pull/2642
[21]: https://github.com/DataDog/integrations-core/pull/2613
[22]: https://github.com/DataDog/integrations-core/pull/2617
[23]: https://github.com/DataDog/integrations-core/pull/2600
[24]: https://github.com/DataDog/integrations-core/pull/2599
[25]: https://github.com/DataDog/integrations-core/pull/2593
[26]: https://github.com/DataDog/integrations-core/pull/2503
[27]: https://github.com/DataDog/integrations-core/pull/2502
[28]: https://github.com/DataDog/integrations-core/pull/2491
[29]: https://github.com/DataDog/integrations-core/pull/2478
[30]: https://github.com/DataDog/integrations-core/pull/2474
[31]: https://github.com/DataDog/integrations-core/pull/2465
[32]: https://github.com/DataDog/integrations-core/pull/2444
[33]: https://github.com/DataDog/integrations-core/pull/2432
[34]: https://github.com/DataDog/integrations-core/pull/2457
[35]: https://github.com/DataDog/integrations-core/pull/2455
[36]: https://github.com/DataDog/integrations-core/pull/2454
[37]: https://github.com/DataDog/integrations-core/pull/2447
[38]: https://github.com/DataDog/integrations-core/pull/2430
[39]: https://github.com/DataDog/integrations-core/pull/2427
[40]: https://github.com/DataDog/integrations-core/pull/2416
[41]: https://github.com/DataDog/integrations-core/pull/2418
[42]: https://github.com/DataDog/integrations-core/pull/2411
[43]: https://github.com/DataDog/integrations-core/pull/2406
[44]: https://github.com/DataDog/integrations-core/pull/2408
[45]: https://github.com/DataDog/integrations-core/pull/2399
[46]: https://github.com/DataDog/integrations-core/pull/2375
[47]: https://github.com/DataDog/integrations-core/pull/2386
[48]: https://github.com/DataDog/integrations-core/pull/2364
[49]: https://github.com/DataDog/integrations-core/pull/2365
[50]: https://github.com/DataDog/integrations-core/pull/2345
[51]: https://github.com/DataDog/integrations-core/pull/2342
[52]: https://github.com/DataDog/integrations-core/pull/2343
[53]: https://github.com/DataDog/integrations-core/pull/2336
[54]: https://github.com/DataDog/integrations-core/pull/2312
[55]: https://github.com/DataDog/integrations-core/pull/2319
[56]: https://github.com/DataDog/integrations-core/pull/2311
[57]: https://github.com/DataDog/integrations-core/pull/2315
[58]: https://github.com/DataDog/integrations-core/pull/2269
[59]: https://github.com/DataDog/integrations-core/pull/2303
[60]: https://github.com/DataDog/integrations-core/pull/2285
[61]: https://github.com/DataDog/integrations-core/pull/2224
[62]: https://github.com/DataDog/integrations-core/pull/2117
[63]: https://github.com/DataDog/integrations-core/pull/2277
[64]: https://github.com/DataDog/integrations-core/pull/2258
[65]: https://github.com/DataDog/integrations-core/pull/2243
[66]: https://github.com/DataDog/integrations-core/pull/2240
[67]: https://github.com/DataDog/integrations-core/pull/2167
[68]: https://github.com/DataDog/integrations-core/pull/2235
[69]: https://github.com/DataDog/integrations-core/pull/2196
[70]: https://github.com/DataDog/integrations-core/pull/2194
[71]: https://github.com/DataDog/integrations-core/pull/2172
[72]: https://github.com/DataDog/integrations-core/pull/2188
[73]: https://github.com/DataDog/integrations-core/pull/2163
[74]: https://github.com/DataDog/integrations-core/pull/2169
[75]: https://github.com/DataDog/integrations-core/pull/2162
[76]: https://github.com/DataDog/integrations-core/pull/2155
[77]: https://github.com/DataDog/integrations-core/pull/2105
[78]: https://github.com/DataDog/integrations-core/pull/2037
[79]: https://github.com/DataDog/integrations-core/pull/1992
[80]: https://github.com/DataDog/integrations-core/pull/1962
[81]: https://github.com/DataDog/integrations-core/pull/1953
[82]: https://github.com/DataDog/integrations-core/pull/1934
[83]: https://github.com/DataDog/integrations-core/pull/1923
[84]: https://github.com/DataDog/integrations-core/pull/1921
[85]: https://github.com/DataDog/integrations-core/pull/1914
[86]: https://github.com/DataDog/integrations-core/pull/1913
[87]: https://github.com/DataDog/integrations-core/pull/1911
[88]: https://github.com/DataDog/integrations-core/pull/1900
[89]: https://github.com/DataDog/integrations-core/pull/1891
[90]: https://github.com/DataDog/integrations-core/pull/1878
[91]: https://github.com/DataDog/integrations-core/pull/1862
