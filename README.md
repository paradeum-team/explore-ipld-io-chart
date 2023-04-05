# explore-ipld-io-chart

A Helm chart for Kubernetes

![Version: 0.1.13](https://img.shields.io/badge/Version-0.1.13-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: v0.1.24](https://img.shields.io/badge/AppVersion-v0.1.24-informational?style=flat-square)

## Installing the Chart

### Add repository

```
helm repo add paradeum-team https://paradeum-team.github.io/helm-charts/
```

### Install chart

```
helm install my-ipfs-cluster-extend paradeum-team/ipfs-cluster-extend --version 0.1.13
```

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| affinity | object | `{}` |  |
| autoscaling.enabled | bool | `false` |  |
| autoscaling.maxReplicas | int | `100` |  |
| autoscaling.minReplicas | int | `1` |  |
| autoscaling.targetCPUUtilizationPercentage | int | `80` |  |
| envFrom | list | `[]` |  |
| env[0].name | string | `"TITLE"` |  |
| env[0].value | string | `"cid-utils-website"` |  |
| extraVolumeMounts[0].mountPath | string | `"/etc/localtime"` |  |
| extraVolumeMounts[0].name | string | `"localtime"` |  |
| extraVolumeMounts[0].readOnly | bool | `true` |  |
| extraVolumes[0].hostPath.path | string | `"/etc/localtime"` |  |
| extraVolumes[0].name | string | `"localtime"` |  |
| fullnameOverride | string | `""` |  |
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.repository | string | `"registry.solarfs.io/ipfs/explore-ipld-io"` |  |
| image.tag | string | `"v0.1.24"` |  |
| imagePullSecrets | list | `[]` |  |
| ingress.annotations | object | `{}` |  |
| ingress.className | string | `""` |  |
| ingress.enabled | bool | `false` |  |
| ingress.hosts[0].host | string | `"chart-example.local"` |  |
| ingress.hosts[0].paths[0].path | string | `"/"` |  |
| ingress.hosts[0].paths[0].pathType | string | `"ImplementationSpecific"` |  |
| ingress.tls | list | `[]` |  |
| nameOverride | string | `""` |  |
| nodeSelector | object | `{}` |  |
| podAnnotations | object | `{}` |  |
| podSecurityContext | object | `{}` |  |
| replicaCount | int | `1` |  |
| resources | object | `{}` |  |
| securityContext | object | `{}` |  |
| service.port | int | `80` |  |
| service.type | string | `"ClusterIP"` |  |
| serviceAccount.annotations | object | `{}` |  |
| serviceAccount.create | bool | `true` |  |
| serviceAccount.name | string | `""` |  |
| tolerations | list | `[]` |  |
