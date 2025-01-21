# invidious

![Version: 0.0.1](https://img.shields.io/badge/Version-0.0.1-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 2.20241110.0](https://img.shields.io/badge/AppVersion-2.20241110.0-informational?style=flat-square)

Invidious is an alternative front-end to YouTube

**Homepage:** <https://invidious.io>

## Maintainers

| Name | Email | Url |
| ---- | ------ | --- |
| Leon Klingele | <mail@leonklingele.de> |  |
| JuniorJPDJ |  | <https://github.com/JuniorJPDJ> |

## Source Code

* <https://github.com/iv-org/invidious>

## Requirements

| Repository | Name | Version |
|------------|------|---------|
| oci://registry-1.docker.io/bitnamicharts | postgresql | ~16 |

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| affinity | object | `{}` |  |
| autoscaling.enabled | bool | `false` |  |
| autoscaling.maxReplicas | int | `16` |  |
| autoscaling.minReplicas | int | `1` |  |
| autoscaling.targetCPUUtilizationPercentage | int | `50` |  |
| config.channel_threads | int | `1` |  |
| config.db.dbname | string | `"invidious"` |  |
| config.db.host | string | `""` |  |
| config.db.password | string | `"kemal"` |  |
| config.db.port | int | `5432` |  |
| config.db.user | string | `"kemal"` |  |
| config.domain | string | `""` |  |
| config.feed_threads | int | `1` |  |
| config.full_refresh | bool | `false` |  |
| config.https_only | bool | `false` |  |
| config.port | int | `3000` |  |
| deploymentLabels | object | `{}` |  |
| fullnameOverride | string | `""` |  |
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.repository | string | `"quay.io/invidious/invidious"` |  |
| image.tag | string | `"latest"` |  |
| imagePullSecrets | list | `[]` |  |
| ingress.annotations | object | `{}` |  |
| ingress.className | string | `""` |  |
| ingress.enabled | bool | `false` |  |
| ingress.hosts[0].host | string | `"chart-example.local"` |  |
| ingress.hosts[0].paths[0].path | string | `"/"` |  |
| ingress.hosts[0].paths[0].pathType | string | `"ImplementationSpecific"` |  |
| ingress.tls | list | `[]` |  |
| name | string | `"invidious"` |  |
| nameOverride | string | `""` |  |
| nodeSelector | object | `{}` |  |
| podSecurityContext.fsGroup | int | `1000` |  |
| podSecurityContext.runAsGroup | int | `1000` |  |
| podSecurityContext.runAsUser | int | `1000` |  |
| postgresql.auth.database | string | `"invidious"` |  |
| postgresql.auth.password | string | `"kemal"` |  |
| postgresql.auth.username | string | `"kemal"` |  |
| postgresql.enabled | bool | `true` |  |
| postgresql.image.tag | int | `16` |  |
| postgresql.primary.initdb.password | string | `"kemal"` |  |
| postgresql.primary.initdb.scriptsConfigMap | string | `"invidious-postgresql-init"` |  |
| postgresql.primary.initdb.username | string | `"kemal"` |  |
| replicaCount | int | `1` |  |
| resources | object | `{}` |  |
| securityContext.allowPrivilegeEscalation | bool | `false` |  |
| securityContext.capabilities.drop[0] | string | `"ALL"` |  |
| service.port | int | `3000` |  |
| service.type | string | `"ClusterIP"` |  |
| sighelper.enabled | bool | `true` |  |
| sighelper.image.pullPolicy | string | `"IfNotPresent"` |  |
| sighelper.image.repository | string | `"quay.io/invidious/inv-sig-helper"` |  |
| sighelper.image.tag | string | `"latest"` |  |
| tolerations | list | `[]` |  |

