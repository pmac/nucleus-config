# Nucleus Config

## Kubernetes YAML

- Cluster: [frankfurt](frankfurt/) in [AWS eu-central-1a](https://eu-central-1.console.aws.amazon.com/ec2/v2/home?region=eu-central-1)
  - [nucleus-dev](frankfurt/nucleus-dev/)
    - [Namespace](frankfurt/nucleus-dev/ns.yaml)
    - [Deployment](frankfurt/nucleus-dev/deploy.yaml)
  - [nucleus-stage](frankfurt/nucleus-stage/)
    - [Namespace](frankfurt/nucleus-stage/ns.yaml)
    - [Deployment](frankfurt/nucleus-stage/deploy.yaml)
  - [nucleus-prod](frankfurt/nucleus-prod/)
    - [Namespace](frankfurt/nucleus-prod/ns.yaml)
    - [Deployment](frankfurt/nucleus-prod/deploy.yaml)
- Cluster: [iowa-b](iowa-b/) in [GCP us-central-1b](https://console.cloud.google.com/kubernetes/clusters/details/us-central1-b/iowa-b?project=meao-202709)
  - [nucleus-dev](iowa-b/nucleus-dev/)
    - [Namespace](iowa-b/nucleus-dev/ns.yaml)
    - [Deployment](iowa-b/nucleus-dev/deploy.yaml)
  - [nucleus-stage](iowa-b/nucleus-stage/)
    - [Namespace](iowa-b/nucleus-stage/ns.yaml)
    - [Deployment](iowa-b/nucleus-stage/deploy.yaml)
  - [nucleus-prod](iowa-b/nucleus-prod/)
    - [Namespace](iowa-b/nucleus-prod/ns.yaml)
    - [Deployment](iowa-b/nucleus-prod/deploy.yaml)

- CI/CD: [.gitlab-ci.yml](.gitlab-ci.yml)
  - Git branch to [job](https://gitlab.com/mozmeao/nucleus-config/-/jobs) mapping:
    - [master](https://github.com/mozmeao/nucleus-config/tree/master)
      - frankfurt dev
      - iowa-b dev
      - frankfurt stage
      - iowa-b stage
      - frankfurt prod
      - iowa-b prod
    - [frankfurt](https://github.com/mozmeao/nucleus-config/tree/frankfurt)
      - frankfurt dev
      - frankfurt stage
      - frankfurt prod
    - [iowa-b](https://github.com/mozmeao/nucleus-config/tree/iowa-b)
      - iowa-b dev
      - iowa-b stage
      - iowa-b prod
    - [stage](https://github.com/mozmeao/nucleus-config/tree/stage)
      - frankfurt stage
      - iowa-b stage
    - [prod](https://github.com/mozmeao/nucleus-config/tree/prod)
      - frankfurt prod
      - iowa-b prod
    - [frankfurt-prod](https://github.com/mozmeao/nucleus-config/tree/frankfurt-prod)
      - frankfurt prod
    - [iowa-b-prod](https://github.com/mozmeao/nucleus-config/tree/iowa-b-prod)
      - iowa-b prod
