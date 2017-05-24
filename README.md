# Git Integration Pack

Pack which allows integration with Git repositories.

## Configuration

Copy the example configuration in [git.yaml.example](./git.yaml.example)
to `/opt/stackstorm/configs/git.yaml` and edit as required.

It should contain an array of one or more repos to monitor. Each entry must contain:

* ``url`` - URL to the Git repository you want to monitor. You can use any
  of supported transport protocols such as SSH or HTTP. For example:
  ``git@github.com:StackStorm/st2.git`` (SSH transport),
  ``https://github.com/StackStorm/st2.git`` (HTTP transport).
* ``branch`` - BRANCH to of the Git repository to monitor. 

## Sensors

### GitCommitSensor

This sensors periodically polls defined Git repository for new commits. When a
new commit is detected, a trigger is dispatched.
