0.6.4 (released 6 April 2017)
---------
* Update dexdeps to handle .dex format version 037 (#158)

0.6.3 (released π 2017)
---------
* Add maxMethodCount option to fail builds if the count is exceeded (#152)
* Add NDK support for AARs (#145)

0.6.2 (released 16 December 2016)
---------
* Don't attempt to count methods on files that don't exist (#139)

0.6.1 (released 14 September 2016)
---------
* Add runOnEachAssemble option to prevent task from running after assemble (#133)

0.6.0 (released 31 August 2016)
---------
* Remove output annotations to opt out of Gradle caching (#132)
* Add configurable slug for TeamCity statistics (#129)

0.5.6 (released 17 August 2016)
---------
* Remove StyledTextOutput use to un-break Gradle 3.0 (#126)
* Remove use of JDK-8-only methods on Process (#122)

0.5.5 (released 30 June 2016)
---------
* Warn when building with Java 7 and below (#120)
* Don't count Instant Run builds by default (#119)

0.5.4 (released 15 June 2016)
---------
* Fix crash on old versions Gradle (#112)
* Fix plugin for Gradle 2.14 (#110)

0.5.3 (released 7 June 2016)
---------
* Fix crash when logging a crash (thanks, Gradle) (#105)
* Add extra diagonistics when running with `--stacktrace` (#102)

0.5.2 (released 17 May 2016)
---------
* Un-break for JVM 7 and below (PR #99)

0.5.1 (released 16 May 2016)
---------

* Fix duplicate task invocation when `assemble` and `countDexMethods` are named on the command line (#97)
* Fix crash when `chartDir` already exists (#94)
* Fix crash when dx invocation fails for .aar (#93)
* Fix JVM verifier crash, again (#86)

0.5.0 (released 18 April 2016)
---------

* Add Android Test Module support (#81)
* Add Instant Run support (#78)
* Add AAR support (#70)
* Add TeamCity support (#68)

0.4.4 (released 4 April 2016)
---------

* Fix display of methods-remaining for multidex builds (don't show negative numbers) (issue #64)
* Add 'maxTreeDepth' config option (issue #54)

0.4.3 (released 14 March 2016)
---------

* Add sunburst chart generation (issue #57)

0.4.2 (released 16 February 2016)
---------

* Add percentage-used for method and field counts to Gradle output

0.4.1 (released 29 January 2016)
----------

* Change output-file extensions to '.json' and '.yml' for JSON and YAML outputs.
* Revert pull request #32 and remove `@Input` from `apkOrDex` (issues #40 and #46)

0.4.0 (released 23 January 2016)
----------

* BUG: Fix incorrect indentation on field-count-only YAML output
* Add YAML as a format option
* Add JSON as a format option
* Replace `printAsTree` with `format` and associated enum

0.3.1 (released 5 December 2015)
----------

* Report number of methods/fields remaining in console output
* Add description and group to Gradle tasks
* Add `includeTotalMethodCount` config option to print total count in the PackageTree output

0.3.0 (released 27 October 2015)
----------

* Remove `exportAsCSV` and just print the file unconditionally
* CHANGED: field counts are enabled by default
* Use Proguard mappings to de-obfuscate class and package names
* Add `exportAsCSV` option to support Jenkins Plot Plugin

0.2.1 (released 11 September 2015)
----------

* BUG: Fix invalid bytecode (issue #11)
* BUG: Work around Groovy-Java interop bug (issue #12)

0.2.0 (released 2 September 2015)
------------------

* Add field-reference count to DexMethodCountTask stdout
* Add configurability via a `dexcount` Gradle extension
* Add verbose output option
* Add option to include field counts in printed package lists
* Add option to sort printed package list by method count (issue #7)
* Add header to list-formatted output
* Include methods in the unnamed package (e.g. primitive arrays) in task output


0.1.1
-----

Initial open-source release
