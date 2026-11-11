# Vidyard for Microsoft 365 Copilot

Vidyard for Microsoft 365 Copilot is an agent that connects Copilot Chat to your
Vidyard account. Users ask Copilot about their videos, players, campaigns, AI
avatars, and video analytics, and do Vidyard work from the chat.

**Download:** [vidyard-m365-copilot.zip](https://github.com/Vidyard/m365-copilot-agent/releases/latest/download/vidyard-m365-copilot.zip)
(the latest release)

## Install for your organization

A Microsoft 365 admin installs the agent.

1. Download `vidyard-m365-copilot.zip` from the
   [latest release](https://github.com/Vidyard/m365-copilot-agent/releases/latest).
2. In the Microsoft 365 admin center, open **Copilot** > **Agents** and upload the
   zip as a custom agent. Microsoft's steps are in
   [Upload Microsoft Copilot custom agents](https://learn.microsoft.com/en-us/microsoft-365/copilot/agent-essentials/agent-lifecycle/agent-upload-agents).
3. Select the users who get the agent. To test first, select only yourself.
4. Review the permissions and finish the deployment.

To change who has the agent later, see
[Deploy agents](https://learn.microsoft.com/en-us/microsoft-365/copilot/agent-essentials/agent-lifecycle/agent-deploy).
Microsoft changes the admin center menus from time to time. If a label here does
not match, follow Microsoft's pages.

If your organization lets users upload custom apps in Teams, a user can also
upload the zip for their own account. See
[Sideload agents](https://learn.microsoft.com/en-us/microsoft-365/copilot/agent-essentials/agent-policies/agent-sideload).

## Sign in

Each user signs in with their Vidyard account the first time the agent uses a
Vidyard tool. The Vidyard consent screen lists the permissions that the agent asks
for. A user can decline a permission. The tools that need it then do not work for
that user.

## Update

Each release has a version number. To update, download the latest release and
upload it in the admin center.

## Check the download

Each release has a `SHA256SUMS` file with the SHA-256 hash of the zip.

- Windows PowerShell: `Get-FileHash vidyard-m365-copilot.zip`, then compare the
  hash with `SHA256SUMS`.
- macOS or Linux: `shasum -a 256 -c --ignore-missing SHA256SUMS` in the
  download folder.

## Support

See the [Vidyard MCP documentation](https://developer.vidyard.com/mcp), or email
[support@vidyard.com](mailto:support@vidyard.com).

This repository holds the releases only.
