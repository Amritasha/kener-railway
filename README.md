# Deploy and Host Kener on Railway

Kener is a modern, open-source status page and uptime monitoring tool. It provides a clean, customizable public status page for your services with real-time uptime tracking, incident management, and scheduled maintenance announcements — fully self-hosted and entirely under your control.

## About Hosting Kener

Hosting Kener is straightforward — it is a Node.js application with no external database dependency by default, using a local file-based store for state. On Railway, you deploy a single service with a persistent volume attached to retain status history and incident records across restarts. Kener reads its monitor configurations from a YAML file, which defines which endpoints to poll, at what interval, and what thresholds to alert on. A public domain is assigned automatically by Railway and can be pointed to a custom domain for your status page URL.

## Common Use Cases

- Publishing a public status page for a SaaS product to communicate uptime to customers
- Monitoring internal service endpoints and getting alerted when they go down
- Managing and communicating planned maintenance windows to users proactively

## Dependencies for Kener Hosting

- **Persistent Volume** — retains incident history, uptime records, and configuration across container restarts
- **monitors.yaml** — defines the services and endpoints Kener should poll and display

### Deployment Dependencies

- [Kener Documentation](https://kener.ing/docs)
- [Kener GitHub Repository](https://github.com/rajnandan1/kener)
- [Railway Volumes](https://docs.railway.com/reference/volumes)

## Why Deploy Kener on Railway?

Railway is a singular platform to deploy your infrastructure stack. Railway will host your infrastructure so you do not have to deal with configuration, while allowing you to vertically and horizontally scale it.

By deploying Kener on Railway, you are one step closer to supporting a complete full-stack application with minimal burden. Host your servers, databases, AI agents, and more on Railway.
