# Retrieve Cloudwatch Logs

<img src="../../images/aws.svg" width="150">

![service](https://img.shields.io/static/v1?label=service&message=AWS&style=flat&logo=AWS&color=E47911)
![uses-slack](https://img.shields.io/static/v1?label=uses&message=Slack&style=flat&logo=slack&color=4A154B)

[![Import to StackPulse](../../images/open_in_stackpulse.svg)](https://app.stackpulse.io/playbook/create?tab=playbook#https://github.com/stackpulse/playbooks/blob/master/aws/retrieve-cloudwatch-logs/playbook.yaml)

This playbook fetch the latest Cloudwatch logs using aws-cli, given region, group-name and stream-name. Then, notify the relevant stackholders using slack.

## Your benefits

- Get recent Cloudwatch logs given region, group name and stream-name
- Limit your max count of desirable logs
- Send and notify the relevant stackholders using slack

## Your experience

![elastic stats as snippets in Slack](../../images/retrieve-cloudwatch-logs-experience.png)

## How to get started

[![Import to StackPulse](../../images/open_in_stackpulse.svg)](https://app.stackpulse.io/playbook/create?tab=playbook#https://github.com/stackpulse/playbooks/blob/master/aws/retrieve-cloudwatch-logs/playbook.yaml)

Not a Stackpulse user? Follow these steps:

1. Make sure your have a [StackPulse](https://stackpulse.com/get-started) account
2. Configure a  new [Slack integration](https://docs.stackpulse.io/getting_started/#step-3-configure-a-new-slack-integration)
3. Choose one of the following methods to authenticate your AWS cloud provider:<br>
    a. Using aws api keys - with StackPulse custom secrets - password in [Custom Secrets](https://docs.stackpulse.io/integrations/#custom-integrations-secrets) <br>
    b. StackPulse aws integration<br>
    c. Configure remote spd runner with the desire roles <br>
4. Import [this playbook](https://app.stackpulse.io/playbooks) into your account
5. Connect it to monitoring alerts or execute manually
