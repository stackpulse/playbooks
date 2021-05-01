# Kubernetes Java Memory Dump

<img src="https://github.com/kubernetes/kubernetes/raw/master/logo/logo.png" width="100">

![env](https://img.shields.io/static/v1?label=env&message=Kubernetes&style=flat&logo=Kubernetes&color=326CE5)
![uses-slack](https://img.shields.io/static/v1?label=uses&message=Slack&style=flat&logo=slack&color=4A154B)

[![Import to StackPulse](../../images/open_in_stackpulse.svg)](https://app.stackpulse.io/playbook/create?tab=playbook#https://github.com/stackpulse/playbooks/blob/master/kubernetes/java-memory-dump/playbook.yaml)

This playbook performs a memory dump of an application running in a Kubernetes pod, uploads it to a cloud storage of your choise and sends the summary along with the option to restart the pod directly from Slack.

## Your benefits

- Get a heap dump of your Java application without the need to setup or orchestrate the tooling by yourself
- Auto save the dump file in a cloud storage bucket and track it on a Slack channel
- Option to restart the pod directly from Slack without accessing the cluster

## Your experience

![slack_screenshot](../../images/k8s_java_heapdump.svg)

## How to get started

[![Import to StackPulse](../../images/open_in_stackpulse.svg)](https://app.stackpulse.io/playbook/create?tab=playbook#https://github.com/stackpulse/playbooks/blob/master/kubernetes/java-memory-dump/playbook.yaml)

### Permissions

This playbook requires certain spd permissions. In order to enable them please follow these steps:

1. Run the command ```kubectl edit ClusterRole stackpulse-step -o yaml -n stackpulse```

2. Add the following api groups:
```

```yaml
- apiGroups:
  - ""
  resources:
  - pods/exec
  verbs:
  - create
- apiGroups:
  - ""
  resources:
  - pods
  - pods/log
  - events
  - nodes
  - configmaps
  verbs:
  - get
  - list
- apiGroups:
  - ""
  resources:
  - pods
  verbs:
  - delete
```

3. Save the new configuration.

Not a Stackpulse user? Follow these steps:

1. Make sure your have a [StackPulse](https://stackpulse.com/get-started) account
2. Configure a  new [Slack integration](https://docs.stackpulse.io/getting_started/#step-3-configure-a-new-slack-integration)
3. Deploy an [SPD (StackPulse Daemon)](https://docs.stackpulse.io/spds/) in your Kubernetes Cluster
4. Import [this playbook](https://app.stackpulse.io/playbooks) into your account
5. Connect it to monitoring alerts or execute manually
