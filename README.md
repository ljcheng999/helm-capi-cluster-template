# helm-capi-cluster-template

![Version: 1.0.2](https://img.shields.io/badge/Version-1.0.2-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 1.0.2](https://img.shields.io/badge/AppVersion-1.0.2-informational?style=flat-square)

A Helm chart for public cloud cluster with Cluster API

## Maintainers

| Name | Email | Url |
| ---- | ------ | --- |
| Lucious Johnny Cheng |  | <ljcheng.kubesources.com> |

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| awsClusterRoleIdentity.allowedNamespaces | list | `[]` |  |
| awsClusterRoleIdentity.create | bool | `false` |  |
| awsClusterRoleIdentity.durationSeconds | int | `900` |  |
| awsClusterRoleIdentity.name | string | `""` |  |
| awsClusterRoleIdentity.roleARN | string | `""` |  |
| awsClusterRoleIdentity.sessionName | string | `""` |  |
| cluster.clusterNetwork.pods.cidrBlocks[0] | string | `"192.168.0.0/16"` |  |
| cluster.create | bool | `true` |  |
| cluster.name | string | `""` |  |
| controlPlane.additionalTags | object | `{}` |  |
| controlPlane.addons | object | `{}` |  |
| controlPlane.apiVersion | string | `""` |  |
| controlPlane.associateOIDCProvider | bool | `false` |  |
| controlPlane.create | bool | `false` |  |
| controlPlane.endpointAccess | object | `{}` |  |
| controlPlane.iamAuthenticatorConfig | object | `{}` |  |
| controlPlane.logging | object | `{}` |  |
| controlPlane.name | string | `""` |  |
| controlPlane.network.subnets | list | `[]` |  |
| controlPlane.network.vpc.id | string | `""` |  |
| controlPlane.partition | string | `""` |  |
| controlPlane.region | string | `""` |  |
| controlPlane.roleAdditionalPolicies | list | `[]` |  |
| controlPlane.sshKeyName | string | `""` |  |
| global.accountID | string | `""` |  |
| global.additionalTags | object | `{}` |  |
| global.clusterVersion | string | `"v1.31.0"` |  |
| global.labels | object | `{}` |  |
| global.name | string | `"capi"` |  |
| global.namePrefix | string | `""` |  |
| global.namespace | string | `"whatever"` |  |
| global.region | string | `""` |  |
| nodeGroup.amiData | object | `{}` |  |
| nodeGroup.amiType | string | `""` |  |
| nodeGroup.availabilityZones | list | `[]` |  |
| nodeGroup.awsLaunchTemplate.imageLookupBaseOS | string | `"amzn_2"` |  |
| nodeGroup.awsLaunchTemplate.imageLookupFormat | string | `""` |  |
| nodeGroup.awsLaunchTemplate.imageLookupOrg | string | `""` |  |
| nodeGroup.awsLaunchTemplate.instanceMetadataOptions.httpPutResponseHopLimit | int | `2` |  |
| nodeGroup.awsLaunchTemplate.instanceMetadataOptions.httpTokens | string | `"required"` |  |
| nodeGroup.awsLaunchTemplate.instanceType | string | `"m5.xlarge"` |  |
| nodeGroup.awsLaunchTemplate.rootVolume.size | int | `250` |  |
| nodeGroup.awsLaunchTemplate.rootVolume.type | string | `"gp3"` |  |
| nodeGroup.create | bool | `false` |  |
| nodeGroup.roleAdditionalPolicies[0] | string | `"arn:aws:iam::aws:policy/AmazonEKSVPCResourceController"` |  |
| nodeGroup.roleAdditionalPolicies[1] | string | `"arn:aws:iam::aws:policy/AmazonSSMManagedInstanceCore"` |  |
| nodeGroup.roleAdditionalPolicies[2] | string | `"arn:aws:iam::aws:policy/service-role/AmazonEBSCSIDriverPolicy"` |  |
| nodeGroup.subnetIDs | list | `[]` |  |
| nodeGroup.systemNodesReplicas | int | `1` |  |
| nodeGroup.userNodesReplicas | int | `1` |  |
| provider | string | `"aws"` |  |

----------------------------------------------
Autogenerated from chart metadata using [helm-docs v1.14.2](https://github.com/norwoodj/helm-docs/releases/v1.14.2)
