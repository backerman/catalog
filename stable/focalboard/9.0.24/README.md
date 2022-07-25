# focalboard

![Version: 9.0.24](https://img.shields.io/badge/Version-9.0.24-informational?style=flat-square) ![AppVersion: 7.1.0](https://img.shields.io/badge/AppVersion-7.1.0-informational?style=flat-square)

Focalboard is an open source, self-hosted alternative to Trello, Notion, and Asana.

TrueCharts can be installed as both *normal* Helm Charts or as Apps on TrueNAS SCALE.

This readme is just an automatically generated general guide on installing our Helm Charts and Apps.
For more information, please click here: [focalboard](https://truecharts.org/docs/charts/stable/focalboard)

**This chart is not maintained by the upstream project and any issues with the chart should be raised [here](https://github.com/truecharts/charts/issues/new/choose)**

## Source Code

* <https://www.focalboard.com/>
* <https://github.com/mattermost/focalboard>
* <https://github.com/FlipEnergy/container-images/blob/main/focalboard>

## Requirements

Kubernetes: `>=1.16.0-0`

## Dependencies

| Repository | Name | Version |
|------------|------|---------|
| https://charts.truecharts.org/ | postgresql | 8.0.45 |
| https://library-charts.truecharts.org | common | 10.4.7 |

## Installing the Chart

### TrueNAS SCALE

To install this App on TrueNAS SCALE check our [Quick-Start Guide](https://truecharts.org/docs/manual/Quick-Start%20Guides/02-Installing-an-App/).

### Helm

To install the chart with the release name `focalboard`

```console
helm repo add TrueCharts https://helm.truecharts.org
helm repo update
helm install focalboard TrueCharts/focalboard
```

## Uninstall

### TrueNAS SCALE

**Upgrading, Rolling Back and Uninstalling the Chart**

To upgrade, rollback or delete this App from TrueNAS SCALE check our [Quick-Start Guide](https://truecharts.org/docs/manual/Quick-Start%20Guides/04-Upgrade-rollback-delete-an-App/).

### Helm

To uninstall the `focalboard` deployment

```console
helm uninstall focalboard
```

## Configuration

### Helm

#### Available Settings

Read through the [values.yaml](./values.yaml) file. It has several commented out suggested values.
Other values may be used from the [values.yaml](https://github.com/truecharts/library-charts/tree/main/charts/stable/common/values.yaml) from the [common library](https://github.com/k8s-at-home/library-charts/tree/main/charts/stable/common).

#### Configure using the Commandline

Specify each parameter using the `--set key=value[,key=value]` argument to `helm install`.

```console
helm install focalboard \
  --set env.TZ="America/New York" \
    TrueCharts/focalboard
```

#### Configure using a yaml file

Alternatively, a YAML file that specifies the values for the above parameters can be provided while installing the chart.

```console
helm install focalboard TrueCharts/focalboard -f values.yaml
```

#### Connecting to other apps

If you need to connect this App to other Apps on TrueNAS SCALE, please refer to our [Linking Apps Internally](https://truecharts.org/docs/manual/Quick-Start%20Guides/06-linking-apps/) quick-start guide.

## Support

- Please check our [quick-start guides for TrueNAS SCALE](https://truecharts.org/docs/manual/SCALE%20Apps/Quick-Start%20Guides/Important-MUST-READ).
- See the [Website](https://truecharts.org)
- Check our [Discord](https://discord.gg/tVsPTHWTtr)
- Open a [issue](https://github.com/truecharts/apps/issues/new/choose)

---

## Sponsor TrueCharts

TrueCharts can only exist due to the incredible effort of our staff.
Please consider making a [donation](https://truecharts.org/docs/about/sponsor) or contributing back to the project any way you can!

---

All Rights Reserved - The TrueCharts Project