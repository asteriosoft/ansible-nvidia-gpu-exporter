# Nvidia gpu prometheus exporter

Docker nvidia gpu prometheus exporter deployment role.

## Table of content

- [Requirements](#requirements)
- [Default Variables](#default-variables)
  - [nvidia_gpu_exporter_arch](#nvidia_gpu_exporter_arch)
  - [nvidia_gpu_exporter_deploy](#nvidia_gpu_exporter_deploy)
  - [nvidia_gpu_exporter_device](#nvidia_gpu_exporter_device)
  - [nvidia_gpu_exporter_docker_network_attach_external](#nvidia_gpu_exporter_docker_network_attach_external)
  - [nvidia_gpu_exporter_docker_network_exernal_name](#nvidia_gpu_exporter_docker_network_exernal_name)
  - [nvidia_gpu_exporter_host_path](#nvidia_gpu_exporter_host_path)
  - [nvidia_gpu_exporter_host_port](#nvidia_gpu_exporter_host_port)
  - [nvidia_gpu_exporter_libnvidia_ml_so_1_path](#nvidia_gpu_exporter_libnvidia_ml_so_1_path)
  - [nvidia_gpu_exporter_libnvidia_ml_so_path](#nvidia_gpu_exporter_libnvidia_ml_so_path)
  - [nvidia_gpu_exporter_smi_tool_path](#nvidia_gpu_exporter_smi_tool_path)
  - [nvidia_gpu_exporter_user](#nvidia_gpu_exporter_user)
  - [nvidia_gpu_exporter_version](#nvidia_gpu_exporter_version)
- [Dependencies](#dependencies)
- [License](#license)
- [Author](#author)

---

## Requirements

- Minimum Ansible version: `2.3`

## Default Variables

### nvidia_gpu_exporter_arch

Architecture for exporter. Note: for 'systemd' deploy method only.

#### Default value

```YAML
nvidia_gpu_exporter_arch: x86_64
```

### nvidia_gpu_exporter_deploy

Deploy implementation method. Should be 'systemd' or 'docker'.

#### Default value

```YAML
nvidia_gpu_exporter_deploy: systemd
```

### nvidia_gpu_exporter_device

Specify nvidia device. Note: for 'docker' deploy method only.

#### Default value

```YAML
nvidia_gpu_exporter_device: /dev/nvidia0
```

### nvidia_gpu_exporter_docker_network_attach_external

Enable connection to existing network. Note: for 'docker' deploy method only.

#### Default value

```YAML
nvidia_gpu_exporter_docker_network_attach_external: false
```

### nvidia_gpu_exporter_docker_network_exernal_name

Specify existing network name to connect. Note: for 'docker' deploy method only.

#### Default value

```YAML
nvidia_gpu_exporter_docker_network_exernal_name: ''
```

### nvidia_gpu_exporter_host_path

Directory on host where docker compose will be store. Note: for 'docker' deploy method only.

#### Default value

```YAML
nvidia_gpu_exporter_host_path: /opt/monitoring/nvidia_exporter
```

### nvidia_gpu_exporter_host_port

Port to expose on host for docker container. Note: for 'docker' deploy method only.

#### Default value

```YAML
nvidia_gpu_exporter_host_port: '9835'
```

### nvidia_gpu_exporter_libnvidia_ml_so_1_path

Path to libnvidia-ml.so.1 on host. Note: for 'docker' deploy method only.

#### Default value

```YAML
nvidia_gpu_exporter_libnvidia_ml_so_1_path: /usr/lib/x86_64-linux-gnu/libnvidia-ml.so.1
```

### nvidia_gpu_exporter_libnvidia_ml_so_path

Path to libnvidia-ml.so on host. Note: for 'docker' deploy method only.

#### Default value

```YAML
nvidia_gpu_exporter_libnvidia_ml_so_path: /usr/lib/x86_64-linux-gnu/libnvidia-ml.so
```

### nvidia_gpu_exporter_smi_tool_path

Path for 'nvidia-smi' tool on host. Note: for 'docker' deploy method only.

#### Default value

```YAML
nvidia_gpu_exporter_smi_tool_path: /usr/bin/nvidia-smi
```

### nvidia_gpu_exporter_user

Username for systemd service. Note: for 'systemd' deploy method only.

#### Default value

```YAML
nvidia_gpu_exporter_user: nvidia_gpu_exporter
```

### nvidia_gpu_exporter_version

Version of nvidia-gpu-exporter. Note: for 'docker' deploy method only.

#### Default value

```YAML
nvidia_gpu_exporter_version: ''
```



## Dependencies

None.

## License

MIT

## Author

Asteriosoft DevOps Team
