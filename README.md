<p align="center">
  <img src=".assets/icon.png" alt="Logo" width="200"/>
</p>

## Description

This plugin allows you to protect your web applications against bots and fraudulent traffic by integrating [DataDome](https://datadome.co) directly into Traefik. Each incoming HTTP request is analyzed by DataDome, and malicious requests are automatically blocked before reaching your backend services.

## Environment Variables

| Variable                    | Required | Description                          |
|-----------------------------|----------|--------------------------------------|
| `DATADOME_SERVER_SIDE_KEY`  | Yes      | Your DataDome Server-Side API Key    |

### Configuration

You must set the `DATADOME_SERVER_SIDE_KEY` environment variable with your DataDome Server-Side API Key before starting Traefik:

```bash
export DATADOME_SERVER_SIDE_KEY="your-server-side-key"
```
