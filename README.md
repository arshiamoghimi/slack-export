# Slack Exporter
A python slack exporter


1. Go to https://api.slack.com/apps
2. Create an app
3. Under 'Features' go to 'OAuth & Permissions'
4. Add 'channels:history', 'channels:read', 'groups:history', 'groups:read', 'im:history', 'im:read', 'mpim:history', 'mpim:read', 'files:read', and 'users:read' to 'User Token Scopes'
5. Install the app to workspace
6. Copy the 'User OAuth Token'

```
# Export Private Channels and Group DMs and 1:1 DMs
python slack_export.py --token xoxs-123... --groups --directMessages

# Export only the "my_private_channel" Private Channel
python slack_export.py --token xoxs-123... --groups my_private_channel

# Export the Private Channels and Group DMs you select when prompted
python slack_export.py --token xoxs-123... --groups --prompt
```

