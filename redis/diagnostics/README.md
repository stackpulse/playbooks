# Redis Diagnostics

<img src="../../images/redis.svg" width="100" alt="Redis">

![type](https://img.shields.io/badge/type-triage-green)
![service](https://img.shields.io/static/v1?label=service&message=Redis&style=flat&logo=Redis&color=A41E11)
![uses-slack](https://img.shields.io/static/v1?label=uses&message=Slack&style=flat&logo=slack&color=4A154B)

[![Import to StackPulse](../../images/open_in_stackpulse.svg)](https://app.stackpulse.io/playbook/create#https://github.com/stackpulse/playbooks/blob/master/redis/diagnostics/playbook.yaml)

This playbook queries a Redis host and retrieves multiple diagnostics:
* General Info - Displays curated data that acts as the first line of triage. for example, the amount of connected clients, used memory, and more.
* Slow Logs - Details the last N (defaults to 10) slowest queries executed in your Redis instance.
* Client List - Allows you to quickly understand who use (or abuse) your Redis instance and how.
* Big Keys - Retrieves statistics about keys size in your Instance. large keys can be very costly in terms of memory usage.

At the end of each step, its output is sent to Slack recipients of your choice.

## Your benefits

- Automatically retrieve an overview of your Redis instance diagnostics.

## Your experience

![redis diagnostics message](../../images/redis-diagnostics.png)

## How to get started

[![Import to StackPulse](../../images/open_in_stackpulse.svg)](https://app.stackpulse.io/playbook/create#https://github.com/stackpulse/playbooks/blob/master/redis/diagnostics/playbook.yaml)

Not a Stackpulse user? Follow these steps:

1. Make sure your have a [StackPulse](https://stackpulse.com/get-started) account
2. Configure a  new [Slack integration](https://docs.stackpulse.io/getting_started/#step-3-configure-a-new-slack-integration)
3. Set up your Redis password as a [Custom Secret](https://docs.stackpulse.io/integrations/#custom-integrations-secrets)
4. Import [this playbook](https://app.stackpulse.io/playbooks) into your account
5. Connect it to monitoring alerts or execute manually
