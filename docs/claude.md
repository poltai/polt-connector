# Polt TMS in Claude

Works in Claude on the web, the desktop app, Cowork and Claude Code. Two pieces: the **connector** gives Claude access to Polt TMS, and the **plugin** teaches it the Polt TMS workflows.

## Team and Enterprise plans (recommended)

An owner sets it up once for everyone.

1. **Add the connector:** **Organization settings → Connectors → Add → Custom → Web**. Name: `Polt TMS`. URL: `https://tms.polt.ai/api/mcp`.
2. **Add the plugin:** **Organization settings → Plugins & skills**. Add this repository (`mike-polt/polt-connector`) to your organization's plugin marketplace, then make the `polt-tms` plugin available to the people who work with loads. Turn on auto-install so it appears for them without any steps.

Each person then opens **Settings → Connectors**, selects **Connect** next to Polt TMS, and signs in with their Polt account. That's all.

## Pro and Max plans

1. **Settings → Connectors → Add custom connector**. Name: `Polt TMS`. URL: `https://tms.polt.ai/api/mcp`.
2. Select **Connect** and sign in with your Polt account.
3. Optional but recommended: install the plugin so Claude knows the workflows. Add `mike-polt/polt-connector` as a plugin marketplace and install the `polt-tms` plugin.

## Claude Code

```bash
claude plugin marketplace add mike-polt/polt-connector
claude plugin install polt-tms@polt-connector
```

The plugin registers the Polt TMS connector. The first time Claude uses it, run `/mcp` and sign in with your Polt account.
