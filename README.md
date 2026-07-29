# lmaa.space Status

GitHub-native monitoring and the public status page for [lmaa.space](https://lmaa.space), live at **[status.lmaa.space](https://status.lmaa.space)**.

[Velvet](https://github.com/phranck/velvet) checks the five configured IPv4 health endpoints every five minutes. Response times are sampled every six hours. Validated public data and internal monitor state live on the dedicated `velvet-data` branch and are retained for 365 days.

Confirmed failures and planned maintenance are tracked as GitHub Issues. The repository needs no external monitoring provider or API key. IPv6 monitoring remains unavailable until GitHub-hosted runners provide documented native IPv6 connectivity.

The configuration is stored in [`velvet.yml`](velvet.yml). Monitoring and deployment run through GitHub Actions using the repository-scoped `GITHUB_TOKEN`.

## License

This repository has been published under the [MIT](https://layered.mit-license.org) license.
