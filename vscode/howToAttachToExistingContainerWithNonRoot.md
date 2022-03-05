# VSCode: how to attach to the existing running container with non-root user

1. Install [Remote Container extension](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers)
2. Open command pallet (`F1` / Shift+Command+P (Mac) / Ctrl+Shift+P (Windows/Linux).) and select `Remote-Containers: Open Attached Container Configuration File`
3. Select a configuration file for the container you want to attach to.
4. Add `"remoteUser": "user-name-inside-container"` to the configuration file. You can also use UID like `"remoteUser": "1000"` instead of username.
5. In addition, if you want to open a workspace in the container, add `"workspaceFolder": "/path/to/workspace"` to the configuration file.
6. Save the configuration file and reload the VS Code window.
