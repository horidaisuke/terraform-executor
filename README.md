# [Departed] terraform-executor

This repository will be no longer maintenance.
Recommend to use [Official Orb](https://circleci.com/developer/ja/orbs/orb/circleci/terraform).

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

Tags name is made from join of [simple tags of docker](https://hub.docker.com/_/docker) and [versions of terraform](https://github.com/hashicorp/terraform/tags).

* `27.2.1-terraform-1.9.8`, `latest`

## License

View [license information](https://github.com/horidaisuke/terraform-executor/blob/main/LICENSE) for the software contained in this image.

This license is inherited from licenses of [library/docker](https://hub.docker.com/_/docker) and [terraform](https://github.com/hashicorp/terraform/blob/main/LICENSE).
