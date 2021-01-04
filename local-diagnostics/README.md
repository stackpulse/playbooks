# Redis Get Big Keys

<img src="../../images/ssh.png" width="100" alt="Redis">

![service](https://img.shields.io/static/v1?label=service&message=Redis&style=flat&logo=Redis&color=A41E11)
![uses-slack](https://img.shields.io/static/v1?label=uses&message=Slack&style=flat&logo=slack&color=4A154B)

[![Import to StackPulse](../../images/open_in_stackpulse.svg)](https://app.stackpulse.io/playbook/create#https://github.com/stackpulse/playbooks/blob/master/redis/get-big-keys/playbook.yaml)

This playbook queries given host memory, storage and cpu usage using well know linux commands  - df, ps and vmstat.
It then sends that output to Slack recipients of your choice as a snippet.

## Your benefits

- Automatically retrieve local information regarding your machine with common linux commands - df, ps and vmstat.

## Your experience

![redis big keys message](../../images/redis_big_keys.png)

## How to get started

[![Import to StackPulse](../../images/open_in_stackpulse.svg)](https://app.stackpulse.io/playbook/create#https://github.com/stackpulse/playbooks/blob/master/redis/get-big-keys/playbook.yaml)

Not a Stackpulse user? Follow these steps:

1. Make sure your have a [StackPulse](https://stackpulse.com/get-started) account
2. Configure a  new [Slack integration](https://docs.stackpulse.io/getting_started/#step-3-configure-a-new-slack-integration)
3. Set up your Redis password as a [Custom Secret](https://docs.stackpulse.io/integrations/#custom-integrations-secrets)
4. Import [this playbook](https://app.stackpulse.io/playbooks) into your account
5. Connect it to monitoring alerts or execute manually
