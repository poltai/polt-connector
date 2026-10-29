# Polt TMS in Gemini

> **Planned.** Gemini support is not available yet. This page describes how setup will work.

Needs **Gemini Enterprise**. Google offers custom MCP connections in Gemini Enterprise as a preview, and only admins can add them. The consumer Gemini app allows custom connectors only on personal Google accounts, so it doesn't work with company accounts.

## Gemini Enterprise admin, once

1. **Get the sign-in details.** Ask Polt.ai support for the Gemini OAuth details for your company: client ID, client secret, authorization URL, token URL and scopes. Keep the secret private.
2. **Add the connection:** add a custom MCP server connection with the URL `https://tms.polt.ai/api/mcp`, choose OAuth 2.0, and enter the details from step 1.
3. **Add the workflows:** download `polt-instructions.md` from the latest [release](https://github.com/poltai/polt-connector/releases), and paste its contents as the instructions of the agent that uses the Polt TMS connection.
4. Make the agent available to the people who work with loads.

## Everyone else

Open the Polt TMS agent in Gemini Enterprise and sign in with your Polt account when asked.
