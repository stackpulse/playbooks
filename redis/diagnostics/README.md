# Redis Diagnostics

<img src="../../images/redis.svg" width="100" alt="Redis">

![type](https://img.shields.io/badge/type-triage-green)
![service](https://img.shields.io/static/v1?label=service&message=Redis&style=flat&logo=Redis&color=A41E11)
![uses-slack](https://img.shields.io/static/v1?label=uses&message=Slack&style=flat&logo=slack&color=4A154B)

[![Import to StackPulse](../../images/open_in_stackpulse.svg)](https://app.stackpulse.io/playbook/create#https://github.com/stackpulse/playbooks/blob/master/redis/diagnostics/playbook.yaml)

This playbook performs diagnostic operations on a Redis cluster and sends them via Slack:

* General Info: Curated basic info such as # of connected clients, memory utilization, memory peaked utilization, server uptime.
* Slow Logs: Last X (default: 10) slowest queries executed.
* Client List: Lists clients with their respective memory utilization, # of pending queries, idle time and age.
* Big Keys: Retrieves keys statistics and memory utilization by data type.

At the end of each step, its output is sent to Slack recipients of your choice.

## Your benefits

* Provides a set of Redis cluster diagnostics that focus on common factors of high memory consumption and performance issues.

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
