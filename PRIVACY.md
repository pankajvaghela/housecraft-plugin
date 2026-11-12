# HouseCraft privacy policy

Updated: 12 November 2026.

This policy covers the open-source HouseCraft agent plugin and its companion HouseCraft Viewer, maintained by Pankaj Vaghela. It describes the local workflow; it does not cover the separate services you use to run your AI agent.

## Data used by the workflow

You choose which floor plans, photos, measurements and project files to share with your agent. The agent uses those inputs to create home geometry, measurement notes and renovation variants. You do not need to provide an address or other identifying details to use HouseCraft.

Setup records selected tools, local executable paths, tool versions, the viewer checkout and readiness results locally. These details help the agent reuse your setup. Credentials do not belong in that record or in a house project.

## Where data goes

HouseCraft does not operate a backend for this plugin, require a HouseCraft account, or add analytics to the viewer. The companion viewer reads a selected project and serves it on your computer at a loopback address. Importing a JSON file in the viewer does not upload it to a HouseCraft service.

Your AI agent may send prompts, files and tool results to its provider according to your account, configuration and that provider’s policies. Local preview does not mean your entire AI interaction stays on your computer.

Installation downloads code from GitHub and dependencies from the npm registry. Those services receive network information when contacted and apply their own policies. Optional Blender or AgentCAD integrations follow their own settings; the HouseCraft workflow requires an explicit request before using cloud processing or uploading home data through them.

## Retention and control

Project files, original inputs, downloaded exports and local setup records remain where you save them until you delete them. HouseCraft does not automatically expire or back up these files. Projects imported into the viewer remain in the browser session until you close or reload it; download any changes you want to keep. The local preview process keeps its startup snapshot until you stop it.

You can stop the preview, delete local project and setup files, and uninstall the plugin. These actions do not delete conversation history, backups or copies retained by your agent provider or other services; use those services’ controls separately.

## Support and policy changes

Use [GitHub Issues](https://github.com/pankajvaghela/housecraft-plugin/issues) for non-sensitive support and privacy questions. Issues are public: do not post home photos, floor plans, addresses, credentials or private logs. Content you choose to post there is handled under GitHub’s policies and remains until removed through GitHub’s controls.

Changes to this policy are recorded in this repository with an updated date. Review the version accompanying the plugin you use.
