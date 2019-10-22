# My first release of RAT

This page contains findings about how RAT is released ....
as I tried to forge a 0.13 release at around 2018-05.

# ASF setup

* https://www.apache.org/dev/publishing-maven-artifacts.html

# Basic setup: the regular Maven release plugin process

```
$ mvn release:prepare -DdryRun=true
$ mvn deploy
$ mvn release:clean
$ mvn release:prepare
$ mvn release:perform
```

# Applied to RAT ....

1. Checkout via SVN with ASF user
```
$ svn --username <yourasfid> co https://svn.apache.org/repos/asf/creadur/rat/trunk ratRelease
```
1. Perform dryRun
1. Perform release

# Open questions

## Q:How to handle reference to older version

```
$ mvn release:prepare -DdryRun=true

<snip>
[INFO] Checking dependencies and plugins for snapshots ...

What is the release version for "Apache Creadur Rat"?
(org.apache.rat:apache-rat-project) 0.13: :
What is SCM release tag or label for "Apache Creadur Rat"?
(org.apache.rat:apache-rat-project) apache-rat-project-0.13: :
What is the new development version for "Apache Creadur Rat"?
(org.apache.rat:apache-rat-project) 0.14-SNAPSHOT: :

<snip>

[ERROR] Failed to execute goal
org.apache.maven.plugins:maven-release-plugin:2.5.3:prepare
(default-cli) on project apache-rat-project: The artifact
(org.apache.rat:apache-rat-plugin) requires a different version (0.13)
than what is found (0.12) for the expression (previousRatVersion) in the
project (org.apache.rat:apache-rat-project). -> [Help 1]
[ERROR]
```

## Q:Where do release artefacts land finally?

* https://www.apache.org/dist/creadur/
 
## Q:Do I need to setup my .m2?

```
```
