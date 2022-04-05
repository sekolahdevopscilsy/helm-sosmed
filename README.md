## Sosmed Helm Chart
This repository used for sekolah devops cilsy

This helm contain kubernetes resource:
- [configMap](https://github.com/sekolahdevopscilsy/helm-sosmed/blob/main/templates/chart-cm-sosmed.yaml)
- [pod](https://github.com/sekolahdevopscilsy/helm-sosmed/blob/main/templates/chart-pod-sosmed.yaml)
- [service](https://github.com/sekolahdevopscilsy/helm-sosmed/blob/main/templates/chart-svc-sosmed.yaml)

Image used:
- [php-sosmed](https://hub.docker.com/repository/docker/sekolahdevopscilsy/php-sosmed)
- [mysql-sosmed](https://hub.docker.com/repository/docker/sekolahdevopscilsy/mysql-sosmed)

## Usage 
This chart uses load balancing service. So ensure your platform has provider to handle it like AWS, GCP, or other cloud provider.

To install this chart, simply run this command
```sh
cd helm-sosmed
helm install sosmed .
```