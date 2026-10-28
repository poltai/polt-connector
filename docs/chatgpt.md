# Polt TMS in ChatGPT

> **Pilot.** The connection works on paid ChatGPT plans. Installing the plugin from this repository is still being tested.

Two pieces: the **app** gives ChatGPT access to Polt TMS, and the **skills** teach it the Polt TMS workflows. The **Polt TMS plugin** bundles both, with the Polt logo.

To sign in, ChatGPT needs the Polt TMS client ID and client secret for ChatGPT. Ask Polt.ai support for them and keep the secret private.

## Add the app (tested)

Works on Plus, Pro, Business and Enterprise. On Business and Enterprise, a workspace admin may need to allow developer mode first.

1. On chatgpt.com, open **Settings → Apps → Advanced settings** and turn on **Developer mode**.
2. Back in **Settings → Apps**, select **Create** and enter:
   - Name: `Polt TMS`
   - MCP server URL: `https://tms.polt.ai/api/mcp`
   - Authentication: **OAuth**, with the client ID and client secret from Polt.ai support
3. Select **Connect** and sign in with your Polt account.

Workspace admins can then publish the app to the people who work with loads.

Write actions, such as creating a load, may need a Business or Enterprise plan; on Plus and Pro, ChatGPT may only read.

## Add the skills

Either download `polt-tms-chatgpt.zip` from the latest [release](https://github.com/mike-polt/polt-connector/releases) and upload it as a plugin, or upload the single skill zips from the same release under **Skills → Create → Upload from your computer**.

In the ChatGPT desktop app you can also add this repository as a plugin marketplace (**Plugins → Add → Add a marketplace**, `mike-polt/polt-connector`) and install **Polt TMS** from it. Updates arrive when the marketplace is refreshed.

## Using it

Pick **Polt TMS** from the tools menu in a chat, or just ask about your loads. ChatGPT describes every change and asks for your confirmation before it creates, updates, books or resolves anything.

The broker you sign in with must have **Allow MCP connection** turned on in Polt TMS, under **Workspace settings → Connections → MCP**.
