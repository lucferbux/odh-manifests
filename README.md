# Open Data Hub Manifests
A repository for [Open Data Hub](https://opendatahub.io) components Kustomize manifests.

## Community

* Website: https://opendatahub.io
* Documentation: https://opendatahub.io/docs/
* ODH Community: https://opendatahub.io/community/

## ODH Core Components

Open Data Hub is an end-to-end AI/ML platform on top of OpenShift Container Platform that provides a core set of integrated components to support end end-to-end MLOps workflow for Data Scientists and Engineers. The components currently available as part of the ODH Core deployment are:

* [ODH Dashboard](https://github.com/opendatahub-io/odh-dashboard)
* [ODH Notebook Controller](odh-notebook-controller/README.md)
* [ODH Notebook Images](https://github.com/opendatahub-io/notebooks/blob/main/README.md)
* [ModelMesh](model-mesh/README.md)
  * [TrustyAI Explainability](https://github.com/trustyai-explainability)

## ODH Incubating Components
* [Distributed Workloads](https://github.com/opendatahub-io/distributed-workloads)
  * [Code Flare](https://github.com/project-codeflare)
* [ODH Notebook Images](https://github.com/opendatahub-io/odh-manifests/tree/master/notebook-images/overlays/additional)
  * Elyra Notebook
  * Code Server Notebook
  * R Studio Notebook (CPU & CUDA)

Any components that were removed with the update to ODH 1.4 have been relocated to the [ODH Contrib](https://github.com/opendatahub-io-contrib) organization under the [odh-contrib-manifests](https://github.com/opendatahub-io-contrib/odh-contrib-manifests) repo.  You can reference the [odh-contrib kfdef](kfdef/odh-contrib.yaml) as a reference on how to deploy any of the odh-contrib-manifests components

### Component Versions

| Manifest Version | ODH Dashboard      | ODH Notebook Controller | ODH Notebook Images | Data Science Pipelines | ModelMesh |
| ---------------- | ------------------ | ----------------------- | ------------------- |----------------------- | --------- |
| master           | v2.14.0-incubation | v1.6                    | 2023a               | v0.2.2                 | v0.11.0   |

Release notes and component versions for each ODH release is available on [opendatahub.io](https://opendatahub.io/blog/?type=release)

## Deploy

We are relying on [Kustomize v3](https://github.com/kubernetes-sigs/kustomize), [kfctl](https://github.com/kubeflow/kfctl) and [Open Data Hub Operator](https://github.com/opendatahub-io/opendatahub-operator/blob/master/README.md) for deployment.

The two ways to deploy are:

1. Following [Getting Started](https://opendatahub.io/docs/quick-installation/) guide using a KFDef from this repository as the custom resource.

## Issues
To submit issues please file a GitHub issue in [opendatahub-community](https://github.com/opendatahub-io/opendatahub-community/issues)
