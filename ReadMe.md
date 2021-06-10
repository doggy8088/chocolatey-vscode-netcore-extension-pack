## .NET Core Extension Pack for Visual Studio Code

This extension pack packages some of the most popular (and some of my favorite) **.NET Core** related extensions. If you like it, please leave your `Rating & Review` and share with your friends. If you have any idea on how to improve this extension pack, I'm looking forwarded to hear from you. Just [let me know](https://github.com/doggy8088/netcore-extension-pack/issues) your awesome ideas! 😊

### How to build package

```sh
choco pack
```

### How to test install locally

```sh
choco install vscode-netcore-extension-pack -d -s .
```

### How to test uninstall locally

```sh
choco uninstall vscode-netcore-extension-pack -d -s .
```

### How to update this package

1. Edit `vscode-netcore-extension-pack.nuspec`

    * Update `<version>`
    * Update `<releaseNotes>` (reference from [here](https://raw.githubusercontent.com/go-gitea/gitea/master/CHANGELOG.md))

2. Test install

    ```sh
    choco pack
    choco install vscode-netcore-extension-pack -d -s . -y
    choco uninstall vscode-netcore-extension-pack -d -s . -y
    ```

3. Publish to Chocolatey Gallery

    ```sh
    choco push vscode-netcore-extension-pack.X.Y.Z.nupkg --source https://push.chocolatey.org/ --apikey YourChocolateyApiKey
    ```
