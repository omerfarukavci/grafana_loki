# grafana_loki

When this compose is up, it installs a Grafana, Loki and dummy_log container each. The dummy_log container generates random logs. Using the Docker loki log driver these are sent to Loki and thus can be viewed in Grafana as well. **But first of all, loki-docker-driver plugin for docker must be installed.** The following command can be used for installation:

`docker plugin install grafana/loki-docker-driver:latest --alias loki --grant-all-permissions`



Then it is used with the `docker compose up` command.
