# Watchlog Helm Charts Repository

This is the Helm repository for Watchlog Agent.

## Usage

Add the repository:

```bash
helm repo add watchlog https://charts.watchlog.io
helm repo update
```

Install the agent:

```bash
helm install watchlog-agent watchlog/watchlog-agent \
  --namespace monitoring \
  --create-namespace \
  --set watchlog.apiKey="your-api-key" \
  --set watchlog.server="https://your-server.com" \
  --set watchlog.clusterName="my-cluster"
```

## Files

- `index.yaml` - Helm repository index file
- `watchlog-agent-*.tgz` - Packaged Helm charts

