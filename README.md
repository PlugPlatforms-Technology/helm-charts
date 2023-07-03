# helm-charts

Helm chart repository
[![Release Charts](https://github.com/PlugPlatforms-Technology/helm-charts/actions/workflows/release.yaml/badge.svg)](https://github.com/PlugPlatforms-Technology/helm-charts/actions/workflows/release.yaml)

## Usage

[Helm](https://helm.sh) must be installed to use the charts.  Please refer to
Helm's [documentation](https://helm.sh/docs) to get started.

Once Helm has been set up correctly, add the repo as follows:

```bash
  helm repo add plugs https://github.com/PlugPlatforms-Technology/helm-charts
```

If you had already added this repo earlier, run `helm repo update` to retrieve
the latest versions of the packages.  You can then run `helm search repo
plugs` to see the charts.

### To install the plugs chart

```bash
  helm install plugs plugs/plugs
```

### To uninstall the chart

```bash
  helm uninstall plugs
```

### Local development

```bash
helm template plugs charts/plugs/ --values charts/plugs/values.yaml
```

```bash
helm upgrade --install nginx charts/plugs/ --values charts/plugs/values.yaml
```
