# docker-ci-helm-kit

Image that is built around **docker**, **k8s** and **helm** and designed to be used in a CI pipeline.

Utilities included and their use cases:

name | use cases | examples
--- | --- | ---
docker | Build and push images to the registry | `docker build`, `docker push`
aws-cli | Auth on AWS and work with it | `aws ecr get-login --no-include-email`
kubectl | Deploy to Kubernetes cluster | `kubectl apply -f file.yaml`
helm | Build and deploy Helm charts | `helm package --version 200 my-chart`
helm-s3 | Helm plugin that allows to use AWS S3 as a chart repository | `helm s3 push my-chart-200.tgz coolrepo`

## License

[MIT](LICENSE).
