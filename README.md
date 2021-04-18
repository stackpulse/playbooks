# StackPulse Playbooks

![stackpulse-logo](images/stackpulse_logo_green_grey_horizontal.png)

StackPulse automates and orchestrates incident response and management, empowering SREs and developers to reduce toil, fix issues faster and deliver reliable software services. This repository contains a set of ready-to-use resources, created by StackPulse together with our partners and the community of our users, that will help you get started with managing and improving the reliability of **your** services.

To learn more about StackPulse, please refer to our [platform description](https://stackpulse.com/platform/) or to our [product documentation](https://docs.stackpulse.io). For your conveniece, playbooks presented in this repository are arranged by **use case**.

## Use-Cases

1. [Alert Enrichment and System Diagnostics](#alert-enrichment-and-system-diagnostics)

2. [Incident Management and Orchestration](#incident-management-and-orchestration)

## Alert Enrichment and System Diagnostics

Playbooks in this section enrich, analyze and triage alerts in real-time. They highlight the important data to be use for remediation by the on-caller engineers. Utilizing them in the incident response routine improves MTTR (Mean Time to Resolve) across all teams and personnel, as well as helps leveraging best diagnostics / troubleshooting practices for each system component regardless of the on-call engineers expertise level.

<br>

<table border=2 border-style=outset>

  <tr>
    <td border=0 width="110">
      <a href="https://github.com/stackpulse/playbooks/tree/master/kubernetes/pod-restarting">
      <img src="https://raw.githubusercontent.com/kubernetes/kubernetes/master/logo/logo.png"/>
      </a>
    </td>
    <td border=0 width="90%">
      <a href="https://github.com/stackpulse/playbooks/tree/master/kubernetes/pod-restarting"><b>Kubernetes Pod Restarting</b></a><br><br>
     This playbook solves consistent Pod Restarting events in a Kubernetes cluster.
     It gets the latest started pods in the namespace provided either by alert or by the user, then gets the current and previous (if exists) logs of the relevant container.
     <br><br>
    <div style="padding-top:1px">
        <img src="https://img.shields.io/static/v1?label=env&message=Kubernetes&style=flat&logo=Kubernetes&color=326CE5" alt="env">
        <img src="https://img.shields.io/static/v1?label=uses&message=Slack&style=flat&logo=slack&color=4A154B" alt="slack">
    </div>
    <div style="margin-top:15px">
        <a href="https://app.stackpulse.io/playbook/create?tab=playbook#https://github.com/stackpulse/playbooks/blob/master/kubernetes/pod-restarting/playbook.yaml" target="_blank" style="vertical-align:middle"><img src="images/open_in_stackpulse.svg" alt="import_in_stackpulse" width="130" id="btn-import-pod-restarting"></a>
    </div>
    </td>
  </tr>
</table>

<br>

<table border=2 border-style=outset>
  <tr>
    <td border=0 width="110">
      <a href="https://github.com/stackpulse/playbooks/tree/master/kubernetes/job-failed">
      <img src="https://raw.githubusercontent.com/kubernetes/kubernetes/master/logo/logo.png"/>
      </a>
    </td>
    <td border=0 width="90%">
      <a href="https://github.com/stackpulse/playbooks/tree/master/kubernetes/job-failed"><b>Kubernetes Job Failed</b></a><br><br>
      This playbook extracts logs from a failed Kubernetes job, sending them as a snippet to Slack, and optionally allows to delete or rerun, asking via Slack.
     <br><br>
    <div style="padding-top:1px">
        <img src="https://img.shields.io/static/v1?label=env&message=Kubernetes&style=flat&logo=Kubernetes&color=326CE5" alt="env">
        <img src="https://img.shields.io/static/v1?label=uses&message=Slack&style=flat&logo=slack&color=4A154B" alt="slack">
    </div>
    <div style="margin-top:15px">
        <a href="https://app.stackpulse.io/playbook/create?tab=playbook#https://github.com/stackpulse/playbooks/blob/master/kubernetes/job-failed/playbook.yaml" target="_blank" style="vertical-align:middle"><img src="images/open_in_stackpulse.svg" alt="import_in_stackpulse" width="130" id="btn-import-k8s-job-failed"></a>
    </div>
    </td>
  </tr>
</table>

<br>

<table border=2 border-style=outset>
  <tr>
    <td border=0 width="110">
      <a href="https://github.com/stackpulse/playbooks/tree/master/postgres/long-running-sessions">
        <img src="images/psql.png"/>
      </a>
    </td>
    <td border=0 width="90%">
      <a href="https://github.com/stackpulse/playbooks/tree/master/postgres/long-running-sessions"><b>Postgres Long Running Sessions</b></a><br><br>
      This playbook collects all non-idle long running sessions from PostgresSQL instance and send it to Slack recipients.<br><br>
    <div style="padding-top:1px">
        <img src="https://img.shields.io/static/v1?label=env&message=Kubernetes&style=flat&logo=Kubernetes&color=326CE5" alt="env">
        <img src="https://img.shields.io/static/v1?label=service&message=PostgresSQL&style=flat&logo=PostgreSQL&color=336791" alt="service">
        <img src="https://img.shields.io/static/v1?label=uses&message=Slack&style=flat&logo=slack&color=4A154B" alt="slack">
    </div>
    <div style="margin-top:15px">
        <a href="https://app.stackpulse.io/playbook/create?tab=playbook#https://github.com/stackpulse/playbooks/blob/master/postgres/long-running-sessions/playbook.yaml" target="_blank" style="vertical-align:middle"><img src="images/open_in_stackpulse.svg" alt="import_in_stackpulse" width="130" id="btn-import-postgres-long-running-sessions"></a>
    </div>
    </td>
  </tr>
</table>

<br>

<table border=2 border-style=outset>
  <tr>
    <td border=0 width="110">
      <a href="https://github.com/stackpulse/playbooks/tree/master/rabbitmq/queues-overview">
        <img src="images/rabbitmq.png"/>
      </a>
    </td>
    <td border=0 width="90%">
      <a href="https://github.com/stackpulse/playbooks/tree/master/rabbitmq/queues-overview"><b>RabbitMQ Queues Overview</b></a><br><br>
      This playbook collects an overview about RabbitMQ instance and classify it's most consumption queues by: <code>messages</code>, <code>unacknowledged messages</code>, <code>messages bytes</code> and <code>memory</code> and send it to Slack recipients.<br><br>
    <div style="padding-top:1px">
        <img src="https://img.shields.io/static/v1?label=env&message=Kubernetes&style=flat&logo=Kubernetes&color=326CE5" alt="env">
        <img src="https://img.shields.io/static/v1?label=service&message=RabbitMQ&style=flat&logo=RabbitMQ&color=FF6600" alt="service">
        <img src="https://img.shields.io/static/v1?label=uses&message=Slack&style=flat&logo=slack&color=4A154B" alt="slack">
    </div>
    <div style="margin-top:15px">
        <a href="https://app.stackpulse.io/playbook/create?tab=playbook#https://github.com/stackpulse/playbooks/blob/master/rabbitmq/queues-overview/playbook.yaml" target="_blank" style="vertical-align:middle"><img src="images/open_in_stackpulse.svg" alt="import_in_stackpulse" width="130" id="btn-import-rabbitmq-overview"></a>
    </div>
   </td>
  </tr>
</table>

<br>

<table border=2 border-style=outset>
  <tr>
    <td border=0 width="110">
      <a href="https://github.com/stackpulse/playbooks/tree/master/elastic/get-stats">
        <img src="images/elastic.png"/>
      </a>
    </td>
    <td border=0 width="90%">
      <a href="https://github.com/stackpulse/playbooks/tree/master/elastic/get-stats"><b>Elasticsearch Get Stats</b></a><br><br>
      This playbook collects diagnostic information, stats and metrics from an Elasticsearch cluster and sends it to specified recepients in Slack.<br><br>
    <div style="padding-top:1px">
        <img src="https://img.shields.io/static/v1?label=service&message=Elasticsearch&style=flat&logo=Elasticsearch&color=00BFB3" alt="service">
        <img src="https://img.shields.io/static/v1?label=uses&message=Slack&style=flat&logo=slack&color=4A154B" alt="slack">
    </div>
    <div style="margin-top:15px">
        <a href="https://app.stackpulse.io/playbook/create?tab=playbook#https://github.com/stackpulse/playbooks/blob/master/elastic/get-stats/playbook.yaml" target="_blank" style="vertical-align:middle"><img src="images/open_in_stackpulse.svg" alt="import_in_stackpulse" width="130" id="btn-import-elastic-get-stats"></a>
    </div>
   </td>
  </tr>
</table>

<br>

<table border=2 border-style=outset>
  <tr>
    <td border=0 width="110">
      <a href="https://github.com/stackpulse/playbooks/tree/master/redis/get-big-keys">
        <img src="images/redis.svg"/>
      </a>
    </td>
    <td border=0 width="90%">
      <a href="https://github.com/stackpulse/playbooks/tree/master/redis/get-big-keys"><b>Redis Get Big Keys</b></a><br><br>
      This playbook queries a Redis host and retrieves the current big keys.
      It then sends that output to Slack recipients of your choice as a snippet.<br><br>
    <div style="padding-top:1px">
        <img src="https://img.shields.io/static/v1?label=service&message=Redis&style=flat&logo=Redis&color=A41E11" alt="service">
        <img src="https://img.shields.io/static/v1?label=uses&message=Slack&style=flat&logo=slack&color=4A154B" alt="slack">
    </div>
    <div style="margin-top:15px">
        <a href="https://app.stackpulse.io/playbook/create?tab=playbook#https://github.com/stackpulse/playbooks/blob/master/redis/get-big-keys/playbook.yaml" target="_blank" style="vertical-align:middle"><img src="images/open_in_stackpulse.svg" alt="import_in_stackpulse" width="130" id="btn-import-redis-big-keys"></a>
    </div>
   </td>
  </tr>
</table>

<br>

<table border=2 border-style=outset>
  <tr>
    <td border=0 width="110">
      <a href="https://github.com/stackpulse/playbooks/tree/master/redis/diagnostics">
        <img src="images/redis.svg"/>
      </a>
    </td>
    <td border=0 width="90%">
      <a href="https://github.com/stackpulse/playbooks/tree/master/redis/diagnostics"><b>Redis Diagnostics</b></a><br><br>
      This playbook collects Redis cluster diagnostics that focus on common factors to high memory consumption and performance issues. It then sends that output via Slack.<br><br>
    <div style="padding-top:1px">
        <img src="https://img.shields.io/static/v1?label=service&message=Redis&style=flat&logo=Redis&color=A41E11" alt="service">
        <img src="https://img.shields.io/static/v1?label=uses&message=Slack&style=flat&logo=slack&color=4A154B" alt="slack">
    </div>
    <div style="margin-top:15px">
        <a href="https://app.stackpulse.io/playbook/create?tab=playbook#https://github.com/stackpulse/playbooks/blob/master/redis/diagnostics/playbook.yaml" target="_blank" style="vertical-align:middle"><img src="images/open_in_stackpulse.svg" alt="import_in_stackpulse" width="130" id="btn-import-redis-diagnostics"></a>
    </div>
   </td>
  </tr>
</table>

<br>

<table border=2 border-style=outset>
  <tr>
    <td border=0 width="110">
      <a href="https://github.com/stackpulse/playbooks/tree/master/linux/diagnostics">
        <img src="images/ssh.svg"/>
      </a>
    </td>
    <td border=0 width="90%">
      <a href="https://github.com/stackpulse/playbooks/tree/master/linux/diagnostics"><b>Linux Diagnostics</b></a><br><br>
      This playbook queries utilization of CPU, memory and storage for a given host and sends the output to Slack recipients of choice.<br><br>
    <div style="padding-top:1px">
        <img src="https://img.shields.io/badge/uses-ssh-red" alt="ssh">
        <img src="https://img.shields.io/static/v1?label=uses&message=Slack&style=flat&logo=slack&color=4A154B" alt="slack">
    </div>
    <div style="margin-top:15px">
        <a href="https://app.stackpulse.io/playbook/create?tab=playbook#https://github.com/stackpulse/playbooks/blob/master/linux/diagnostics/playbook.yaml" target="_blank" style="vertical-align:middle"><img src="images/open_in_stackpulse.svg" alt="import_in_stackpulse" width="130" id="btn-import-linux-diagnostics"></a>
    </div>
   </td>
  </tr>
</table>

<br>

## Incident Management and Orchestration

Playbooks in this section help automate incident management and communication flows across the organization or specific per teams and services.

<br>

<table border=2 border-style=outset>
  <tr>
    <td border=0 width="110">
      <a href="https://github.com/stackpulse/playbooks/tree/master/stackpulse/create-incident-war-room">
      <img src="images/stackpulse.png"/>
      </a>
    </td>
    <td border=0 width="90%">
      <a href="https://github.com/stackpulse/playbooks/tree/master/stackpulse/create-incident-war-room"><b>Create Incident War-room (Slack)</b></a><br><br>This playbook creates a Slack Incident War Room when an incident is created, invites the relevant participants (based on incident details or other logic).<br><br>
        <div style="padding-top:1px">
            <img src="https://img.shields.io/static/v1?label=uses&message=Slack&style=flat&logo=slack&color=4A154B" alt="slack">
        </div>
        <div style="margin-top:15px">
            <a href="https://app.stackpulse.io/playbook/create?tab=playbook#https://github.com/stackpulse/playbooks/blob/master/stackpulse/create-incident-war-room" target="_blank" style="vertical-align:middle"><img src="images/open_in_stackpulse.svg" alt="import_in_stackpulse" width="130" id="btn-import-create-war-room-slack"></a>
    </div>
  </td>
  </tr>
</table>

<br>

<table border=2 border-style=outset>
  <tr>
    <td border=0 width="110">
      <a href="https://github.com/stackpulse/playbooks/tree/master/stackpulse/create-incident-war-room-pagerduty">
      <img src="images/stackpulse.png"/>
      </a>
    </td>
    <td border=0 width="90%">
      <a href="https://github.com/stackpulse/playbooks/tree/master/stackpulse/create-incident-war-room-pagerduty"><b>Create Incident War-room (Slack, Zoom, PagerDuty)</b></a><br><br>Playbook that creates Incident War Room in Slack (and/or Video Conferencing software) when an incident is created, invites the relevant participants based on incident details (and/or on on-call rotation schedules).<br><br>
        <div style="padding-top:1px">
            <img src="https://img.shields.io/static/v1?label=uses&message=Slack&style=flat&logo=slack&color=4A154B" alt="slack">
            <img src="https://img.shields.io/static/v1?label=uses&message=Zoom&style=flat&logo=zoom&color=2D8CFF" alt="zoom">
            <img src="https://img.shields.io/static/v1?label=uses&message=PagerDuty&style=flat&logo=pagerduty&color=47BA04" alt="pagerduty">
        </div>
        <div style="margin-top:15px">
            <a href="https://app.stackpulse.io/playbook/create?tab=playbook#https://github.com/stackpulse/playbooks/blob/master/stackpulse/create-incident-war-room-pagerduty" target="_blank" style="vertical-align:middle"><img src="images/open_in_stackpulse.svg" alt="import_in_stackpulse" width="130" id="btn-import-create-war-room-pagerduty"></a>
    </div>
  </td>
  </tr>
</table>

<br>

<table border=2 border-style=outset>
  <tr>
    <td border=0 width="110">
      <a href="https://github.com/stackpulse/playbooks/tree/master/stackpulse/create-incident-war-room-opsgenie">
      <img src="images/stackpulse.png"/>
      </a>
    </td>
    <td border=0 width="90%">
      <a href="https://github.com/stackpulse/playbooks/tree/master/stackpulse/create-incident-war-room-opsgenie"><b>Create Incident War-room (Slack, Zoom, OpsGenie)</b></a><br><br>Playbook that creates Incident War Room in Slack (and/or Video Conferencing software) when an incident is created, invites the relevant participants based on incident details (and/or on on-call rotation schedules).<br><br>
        <div style="padding-top:1px">
            <img src="https://img.shields.io/static/v1?label=uses&message=Slack&style=flat&logo=slack&color=4A154B" alt="slack">
            <img src="https://img.shields.io/static/v1?label=uses&message=Zoom&style=flat&logo=zoom&color=2D8CFF" alt="zoom">
            <img src="https://img.shields.io/static/v1?label=uses&message=OpsGenie&style=flat&logo=opsgenie&color=0052CC" alt="opsgenie">
        </div>
        <div style="margin-top:15px">
            <a href="https://app.stackpulse.io/playbook/create?tab=playbook#https://github.com/stackpulse/playbooks/blob/master/stackpulse/create-incident-war-room-opsgenie" target="_blank" style="vertical-align:middle"><img src="images/open_in_stackpulse.svg" alt="import_in_stackpulse" width="130" id="btn-import-create-war-room-opsgenie"></a>
    </div>
  </td>
  </tr>
</table>

<br>

<table border=2 border-style=outset>
  <tr>
    <td border=0 width="110">
      <a href="https://github.com/stackpulse/playbooks/tree/master/stackpulse/archive-incident-war-room">
      <img src="images/stackpulse.png"/>
      </a>
    </td>
    <td border=0 width="90%">
      <a href="https://github.com/stackpulse/playbooks/tree/master/stackpulse/archive-incident-war-room"><b>Archive Incident War Room (Slack)</b></a><br><br>Playbook that runs upon incident resolution and asks the incident commander whether to archive the Slack War-room that belonged to the incident.<br><br>
        <div style="padding-top:1px">
            <img src="https://img.shields.io/static/v1?label=uses&message=Slack&style=flat&logo=slack&color=4A154B" alt="slack">
        </div>
        <div style="margin-top:15px">
            <a href="https://app.stackpulse.io/playbook/create?tab=playbook#https://github.com/stackpulse/playbooks/blob/master/stackpulse/archive-incident-war-room" target="_blank" style="vertical-align:middle"><img src="images/open_in_stackpulse.svg" alt="import_in_stackpulse" width="130" id="btn-import-archive-war-room"></a>
    </div>
  </td>
  </tr>
</table>
