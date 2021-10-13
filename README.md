# terraform-executor
Circleci executor installed terraform

## Usage

Define executor in `.circleci/config.yml` like this:

```yaml
executors:
  terraform-executor:
    docker:
      - image: horidaisuke/terraform-executor:latest
    shell: /bin/bash -leo pipefail
    environment:
      - BASH_ENV: /etc/profile
```

## Tags

* `20.10.9-terraform-0.15.5`, `latest`

## License

View [license information](https://github.com/horidaisuke/terraform-executor/blob/main/LICENSE) for the software contained in this image.

This license is inherited from licenses of [library/docker](https://hub.docker.com/_/docker) and [terraform](https://github.com/hashicorp/terraform/blob/main/LICENSE).
