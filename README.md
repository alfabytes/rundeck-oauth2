# Rundeck with OAuth2 Proxy

This repository contains Helm charts and configuration files for deploying Rundeck and OAuth2 Proxy. The structure of the repository is as follows:

### Charts

The `charts` directory contains the Helm charts for Rundeck and OAuth2 Proxy. These charts are used to deploy the respective applications on Kubernetes.

- **rundeck**: Helm chart for deploying Rundeck.
- **oauth2-proxy**: Helm chart for deploying OAuth2 Proxy.

### Values

The `values` directory contains the configuration files for customizing the deployment of Rundeck and OAuth2 Proxy. These files are used to override the default values in the Helm charts.

- **rundeck**: Configuration file for Rundeck.
- **oauth2-proxy**: Configuration file for OAuth2 Proxy.

## Usage

To deploy Rundeck and OAuth2 Proxy using Helm, follow these steps:

1. **Clone the Repository**

    ```bash
    git clone https://github.com/alfabytes/rundeck-oauth2.git
    cd rundeck-oauth2
    ```

2. **Deploy Rundeck**

    ```bash
    helm install rundeck ./charts/rundeck -f ./values/rundeck/values.yaml
    ```

3. **Deploy OAuth2 Proxy**

    ```bash
    helm install oauth2-proxy ./charts/oauth2-proxy -f ./values/oauth2-proxy/values.yaml
    ```
