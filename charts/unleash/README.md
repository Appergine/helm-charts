# unleash

![Version: 0.0.5](https://img.shields.io/badge/Version-0.0.5-informational?style=flat-square) ![AppVersion: 3.2.31](https://img.shields.io/badge/AppVersion-3.2.31-informational?style=flat-square)

Unleash is a open source feature flag & toggle system, that gives you a great overview over all feature toggles across all your applications and services.

**Homepage:** <https://github.com/Appergine/helm-charts>

## Maintainers

| Name | Email | Url |
| ---- | ------ | --- |
| jose-appergine |  |  |

## Requirements

| Repository | Name | Version |
|------------|------|---------|
| https://charts.helm.sh/stable/ | postgresql | 8.5.0 |

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| containerPort | int | `4242` |  |
| extraContainers | string | `""` |  |
| extraVolumes | string | `""` |  |
| image.pullPolicy | string | `"Always"` |  |
| image.repository | string | `"unleashorg/unleash-server"` |  |
| image.tag | string | `"3.2.30"` |  |
| ingress.enabled | bool | `false` |  |
| livenessProbe.enabled | bool | `false` |  |
| postgresql.enabled | bool | `true` |  |
| postgresql.extraEnv | list | `[]` |  |
| postgresql.global.postgresql | object | `{}` |  |
| postgresql.image.debug | bool | `false` |  |
| postgresql.image.pullPolicy | string | `"IfNotPresent"` |  |
| postgresql.image.registry | string | `"docker.io"` |  |
| postgresql.image.repository | string | `"bitnami/postgresql"` |  |
| postgresql.image.tag | string | `"11.7.0-debian-10-r9"` |  |
| postgresql.ldap.baseDN | string | `""` |  |
| postgresql.ldap.bindDN | string | `""` |  |
| postgresql.ldap.bind_password | string | `nil` |  |
| postgresql.ldap.enabled | bool | `false` |  |
| postgresql.ldap.port | string | `""` |  |
| postgresql.ldap.prefix | string | `""` |  |
| postgresql.ldap.scheme | string | `""` |  |
| postgresql.ldap.search_attr | string | `""` |  |
| postgresql.ldap.search_filter | string | `""` |  |
| postgresql.ldap.server | string | `""` |  |
| postgresql.ldap.suffix | string | `""` |  |
| postgresql.ldap.tls | bool | `false` |  |
| postgresql.ldap.url | string | `""` |  |
| postgresql.livenessProbe.enabled | bool | `true` |  |
| postgresql.livenessProbe.failureThreshold | int | `6` |  |
| postgresql.livenessProbe.initialDelaySeconds | int | `30` |  |
| postgresql.livenessProbe.periodSeconds | int | `10` |  |
| postgresql.livenessProbe.successThreshold | int | `1` |  |
| postgresql.livenessProbe.timeoutSeconds | int | `5` |  |
| postgresql.master.affinity | object | `{}` |  |
| postgresql.master.annotations | object | `{}` |  |
| postgresql.master.extraVolumeMounts | list | `[]` |  |
| postgresql.master.extraVolumes | list | `[]` |  |
| postgresql.master.labels | object | `{}` |  |
| postgresql.master.nodeSelector | object | `{}` |  |
| postgresql.master.podAnnotations | object | `{}` |  |
| postgresql.master.podLabels | object | `{}` |  |
| postgresql.master.priorityClassName | string | `""` |  |
| postgresql.master.tolerations | list | `[]` |  |
| postgresql.metrics.enabled | bool | `true` |  |
| postgresql.metrics.image.pullPolicy | string | `"IfNotPresent"` |  |
| postgresql.metrics.image.registry | string | `"docker.io"` |  |
| postgresql.metrics.image.repository | string | `"bitnami/postgres-exporter"` |  |
| postgresql.metrics.image.tag | string | `"0.8.0-debian-10-r28"` |  |
| postgresql.metrics.livenessProbe.enabled | bool | `true` |  |
| postgresql.metrics.livenessProbe.failureThreshold | int | `6` |  |
| postgresql.metrics.livenessProbe.initialDelaySeconds | int | `5` |  |
| postgresql.metrics.livenessProbe.periodSeconds | int | `10` |  |
| postgresql.metrics.livenessProbe.successThreshold | int | `1` |  |
| postgresql.metrics.livenessProbe.timeoutSeconds | int | `5` |  |
| postgresql.metrics.prometheusRule.additionalLabels | object | `{}` |  |
| postgresql.metrics.prometheusRule.enabled | bool | `false` |  |
| postgresql.metrics.prometheusRule.namespace | string | `""` |  |
| postgresql.metrics.prometheusRule.rules | list | `[]` |  |
| postgresql.metrics.readinessProbe.enabled | bool | `true` |  |
| postgresql.metrics.readinessProbe.failureThreshold | int | `6` |  |
| postgresql.metrics.readinessProbe.initialDelaySeconds | int | `5` |  |
| postgresql.metrics.readinessProbe.periodSeconds | int | `10` |  |
| postgresql.metrics.readinessProbe.successThreshold | int | `1` |  |
| postgresql.metrics.readinessProbe.timeoutSeconds | int | `5` |  |
| postgresql.metrics.securityContext.enabled | bool | `false` |  |
| postgresql.metrics.securityContext.runAsUser | int | `1001` |  |
| postgresql.metrics.service.annotations."prometheus.io/port" | string | `"9187"` |  |
| postgresql.metrics.service.annotations."prometheus.io/scrape" | string | `"true"` |  |
| postgresql.metrics.service.loadBalancerIP | string | `nil` |  |
| postgresql.metrics.service.type | string | `"ClusterIP"` |  |
| postgresql.metrics.serviceMonitor.additionalLabels | object | `{}` |  |
| postgresql.metrics.serviceMonitor.enabled | bool | `false` |  |
| postgresql.networkPolicy.allowExternal | bool | `true` |  |
| postgresql.networkPolicy.enabled | bool | `false` |  |
| postgresql.persistence.accessModes[0] | string | `"ReadWriteOnce"` |  |
| postgresql.persistence.annotations | object | `{}` |  |
| postgresql.persistence.enabled | bool | `true` |  |
| postgresql.persistence.mountPath | string | `"/bitnami/postgresql"` |  |
| postgresql.persistence.size | string | `"1Gi"` |  |
| postgresql.persistence.subPath | string | `""` |  |
| postgresql.postgresqlDataDir | string | `"/bitnami/postgresql/data"` |  |
| postgresql.postgresqlDatabase | string | `"unleash"` |  |
| postgresql.postgresqlPassword | string | `"yq78uqbFeGkYk7"` |  |
| postgresql.postgresqlUsername | string | `"postgres"` |  |
| postgresql.readinessProbe.enabled | bool | `true` |  |
| postgresql.readinessProbe.failureThreshold | int | `6` |  |
| postgresql.readinessProbe.initialDelaySeconds | int | `5` |  |
| postgresql.readinessProbe.periodSeconds | int | `10` |  |
| postgresql.readinessProbe.successThreshold | int | `1` |  |
| postgresql.readinessProbe.timeoutSeconds | int | `5` |  |
| postgresql.replication.applicationName | string | `"my_application"` |  |
| postgresql.replication.enabled | bool | `false` |  |
| postgresql.replication.numSynchronousReplicas | int | `1` |  |
| postgresql.replication.password | string | `"repl_password"` |  |
| postgresql.replication.slaveReplicas | int | `2` |  |
| postgresql.replication.synchronousCommit | string | `"on"` |  |
| postgresql.replication.user | string | `"repl_user"` |  |
| postgresql.resources.requests.cpu | string | `"250m"` |  |
| postgresql.resources.requests.memory | string | `"256Mi"` |  |
| postgresql.securityContext.enabled | bool | `true` |  |
| postgresql.securityContext.fsGroup | int | `1001` |  |
| postgresql.securityContext.runAsUser | int | `1001` |  |
| postgresql.service.annotations | object | `{}` |  |
| postgresql.service.port | int | `5432` |  |
| postgresql.service.type | string | `"ClusterIP"` |  |
| postgresql.serviceAccount.enabled | bool | `false` |  |
| postgresql.shmVolume.chmod.enabled | bool | `true` |  |
| postgresql.shmVolume.enabled | bool | `true` |  |
| postgresql.slave.affinity | object | `{}` |  |
| postgresql.slave.annotations | object | `{}` |  |
| postgresql.slave.extraVolumeMounts | list | `[]` |  |
| postgresql.slave.extraVolumes | list | `[]` |  |
| postgresql.slave.labels | object | `{}` |  |
| postgresql.slave.nodeSelector | object | `{}` |  |
| postgresql.slave.podAnnotations | object | `{}` |  |
| postgresql.slave.podLabels | object | `{}` |  |
| postgresql.slave.priorityClassName | string | `""` |  |
| postgresql.slave.tolerations | list | `[]` |  |
| postgresql.updateStrategy.type | string | `"RollingUpdate"` |  |
| postgresql.volumePermissions.enabled | bool | `false` |  |
| postgresql.volumePermissions.image.pullPolicy | string | `"Always"` |  |
| postgresql.volumePermissions.image.registry | string | `"docker.io"` |  |
| postgresql.volumePermissions.image.repository | string | `"bitnami/minideb"` |  |
| postgresql.volumePermissions.image.tag | string | `"buster"` |  |
| postgresql.volumePermissions.securityContext.runAsUser | int | `0` |  |
| readinessProbe.enabled | bool | `false` |  |
| replicaCount | int | `1` |  |
| resources | object | `{}` |  |
| service.port | int | `4242` |  |
| service.type | string | `"ClusterIP"` |  |
| vpa.enabled | bool | `false` |  |
