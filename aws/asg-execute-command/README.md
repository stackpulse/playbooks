# AWS Auto Scaling Group Execute Command

<img src="../../images/aws.svg" width="150">

![service](https://img.shields.io/static/v1?label=service&message=AWS&style=flat&logo=AWS&color=FF9900)
![uses-slack](https://img.shields.io/static/v1?label=uses&message=Slack&style=flat&logo=slack&color=4A154B)

[![Import to StackPulse](../../images/open_in_stackpulse.svg)](https://app.stackpulse.io/playbook/create?tab=playbook#https://github.com/stackpulse/playbooks/blob/master/aws/asg-execute-command/playbook.yaml)

This playbook executes a command on each instance of an AWS Auto Scaling Group and and then verifies its health.

## Your benefits

- Retrieve all instances of an AWS Auto Scaling Group and execute a remediation command on each one
- Get health metrics for a given AWS Auto Scaling Group

## Your experience

### Parameters

![asg-execute-command-result](../../images/asg-params.png)

### Result

![asg-execute-command-result](../../images/asg-execute-command-result.svg)

## How to get started

[![Import to StackPulse](../../images/open_in_stackpulse.svg)](https://app.stackpulse.io/playbook/create?tab=playbook#https://github.com/stackpulse/playbooks/blob/master/aws/asg-execute-command/playbook.yaml)

Not a StackPulse user? Follow these steps:

1. Make sure your have a [StackPulse](https://stackpulse.com/get-started) account
2. Configure a  new [Slack integration](https://docs.stackpulse.io/getting_started/#step-3-configure-a-new-slack-integration)
3. Set up your AWS authentication process-
    a. Remote SPD with dedicated AWS role.
    b. Using AWS integrarion.
    c. Using AWS user tokens.
4. Import [this playbook](https://app.stackpulse.io/playbooks) into your account
5. Connect it to monitoring alerts or execute manually
