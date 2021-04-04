# StackPulse Create Incident War Room

<img src="../../images/stackpulse.png" width="100" alt="StackPulse">

![uses-slack](https://img.shields.io/static/v1?label=uses&message=Slack&style=flat&logo=slack&color=4A154B)
![uses-zoom](https://img.shields.io/static/v1?label=uses&message=Zoom&style=flat&logo=zoom&color=2D8CFF)
![uses-pagerduty](https://img.shields.io/static/v1?label=uses&message=PagerDuty&style=flat&logo=pagerduty&color=47BA04)

[![Import to StackPulse](../../images/open_in_stackpulse.svg)](https://app.stackpulse.io/playbook/create?tab=playbook#https://github.com/stackpulse/playbooks/blob/master/stackpulse/create-incident-war-room-pagerduty)

This playbook opens a new Slack channel to be used as a war room for a new incident.
It additionally creates a Zoom call and pages the current on caller on PagerDuty at the time of the incident.
This playbook should be set up to be triggered by an incident creation event.

## Your benefits

- Coordinate all incident stakeholders faster with on demand war room channel and Zoom meeting creation.
- Configurable invitees list allows to invite relevant participants per use case.
- Seamlessly page your on caller with the creation of a StackPulse incident.

## Your experience

![war room created](../../images/war_room.gif)

![war room created](../../images/war_room_created.svg)

## How to get started

[![Import to StackPulse](../../images/open_in_stackpulse.svg)](https://app.stackpulse.io/playbook/create?tab=playbook#https://github.com/stackpulse/playbooks/blob/master/stackpulse/create-incident-war-room-pagerduty)

Not a Stackpulse user? Follow these steps:

1. Make sure your have a [StackPulse](https://stackpulse.com/get-started) account
2. Configure a new [Slack integration](https://docs.stackpulse.io/getting_started/#step-3-configure-a-new-slack-integration)
3. Set up your Zoom and PagerDuty API keys as [Custom Secrets](https://docs.stackpulse.io/integrations/#custom-integrations-secrets)
4. Import [this playbook](https://app.stackpulse.io/playbooks) into your account
5. This playbook has a default trigger attached to it. It will be triggered when a StackPulse incident is created

> :memo: Note: If your account is missing one of the required integrations, or has multiple instances of an integration, go to the `TRIGGER` tab to select the required ones.
