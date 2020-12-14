# StackPulse Archive Incident War Room

<img src="../../images/stackpulse.png" width="100" alt="StackPulse">

![type](https://img.shields.io/badge/type-notification-green)
![uses-slack](https://img.shields.io/static/v1?label=uses&message=Slack&style=flat&logo=slack&color=4A154B)

[![Import to StackPulse](../../images/open_in_stackpulse.svg)](https://app.stackpulse.io/playbook/create#https://github.com/stackpulse/playbooks/blob/master/stackpulse/archive-incident-war-room/playbook.yaml)

This playbook interactively asks the incident commander whether to archive the incident's war room channel.
The default behavior after a timeout of five minuets will be to archive the channel.
This playbook should be triggered by an incident update event with a closed status.

## Your benefits

- Keep Slack workspace uncluttered with closed incident's war room channels and streamline your incident closure flow.

## Your experience

![war room archive](../../images/war_room_archive_question.png)

## How to get started

[![Import to StackPulse](../../images/open_in_stackpulse.svg)](https://app.stackpulse.io/playbook/create#https://github.com/stackpulse/playbooks/blob/master/stackpulse/archive-incident-war-room/playbook.yaml)

Not a Stackpulse user? Follow these steps:

1. Make sure your have a [StackPulse](https://stackpulse.com/get-started) account
2. Configure a  new [Slack integration](https://docs.stackpulse.io/getting_started/#step-3-configure-a-new-slack-integration)
3. Import [this playbook](https://app.stackpulse.io/playbooks) into your account
4. Connect it to be triggered by incident update events with `event.Status` is `closed`
