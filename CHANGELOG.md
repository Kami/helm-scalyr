# Changelog

## 0.2.4 - in development

* Kubelet TLS cert validation is now enabled by default. For information on how to disable it or
  use a custom CA bundle, please refer to the README.md file.
* New ``podLabels`` values option has been added.
* Unncessary ``ports`` section has been removed from deployment and daemonset resource definition
  file.
* agent container livenesProbe which utilizes ``scalyr-agent-2 status -H`` command has been added
  and enabled by default.
* Chart installation will now fail early if ``scalyr.config`` entry value contains a string value
  which is not correctly base64 encoded.
