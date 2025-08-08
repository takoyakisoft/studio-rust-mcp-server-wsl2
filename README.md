# Roblox Studio MCP Server

This repository can be connected to Roblox Studio using Codex CLI on Windows.

## Install

WSL2 Ubuntu 24.04

```bash
wget -O Linux-rbx-studio-mcp.zip https://github.com/user-attachments/files/21680948/Linux-rbx-studio-mcp.zip
unzip Linux-rbx-studio-mcp.zip
rm Linux-rbx-studio-mcp.zip 

sudo mv ./rbx-studio-mcp /usr/local/bin/
sudo chmod +x /usr/local/bin/rbx-studio-mcp
```

## WSL2 Mirrored Mode Networking 

C:\Users\<user>\.wslconfig:
```ini
[wsl2]
networkingMode=mirrored
```

## Codex CLI MCP

 ~/.codex/config.toml:
```toml
[mcp_servers.roblox-studio]  
command = "rbx-studio-mcp"  
args = ["--stdio"]  
```
