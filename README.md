# Nexo Shop Script

A customizable FiveM shop resource with a modern web-based interface, inspired by the NoPixel V-style shop experience.

> **Status:** Community release  
> **Price:** Free  
> **Author:** Nexo Studio

## ✨ Features

- Modern shop interface powered by the `web/` directory
- Configurable resource settings through `config.lua`
- Separated client, server, and shared resource files
- Designed to be easy to install and customize
- Add or adjust shop items according to your server's implementation

*The exact features and supported frameworks depend on the code included in this release.*

## 📁 Resource Structure

```text
nexo_shop/
├── client/          # Client-side scripts
├── server/          # Server-side scripts
├── shared/          # Shared scripts and definitions
├── web/             # Shop UI assets
├── config.lua       # Resource configuration
├── fxmanifest.lua   # FiveM resource manifest
└── README.md        # Project overview
```

## 📦 Installation

1. Download or clone this repository.
2. Extract the resource into your FiveM server's resources directory.
3. Keep the resource folder name consistent with the name used in your server configuration.
4. Review `config.lua` and adjust the available settings for your server.
5. Check `fxmanifest.lua` and make sure all required files and dependencies are present.
6. Add the resource to your `server.cfg`:

   ```cfg
   ensure nexo_shop
   ```

7. Restart the server or start the resource through your server management panel.
8. Check the server console for missing dependencies or configuration errors.

> **Important:** `nexo_shop` is an example resource folder name. If you use a different folder name, update the `ensure` line accordingly. Install any dependencies required by the resource before starting it.

## ⚙️ Configuration

Open `config.lua` and review the available options. Change only settings that exist in your version of the file.

Depending on how the script is implemented, you may be able to configure shop details, items, prices, locations, or other behavior. Refer to the comments and existing configuration values in `config.lua` for the options actually supported.

## 🛠️ Customization

- **Shop items:** Look for the item definitions or configuration entries used by the resource.
- **Shop UI:** The `web/` directory contains the interface assets. Back up files before editing them.
- **Client/server behavior:** Review the relevant scripts in `client/` and `server/`.
- **Shared definitions:** Check `shared/` for values used by both client and server code.

Make a backup before making changes, and test customizations on a development server first.

## ❓ Troubleshooting

- **Resource does not start:** Check the server console and verify the resource folder name.
- **UI does not open:** Confirm that the files referenced by `fxmanifest.lua` exist in `web/`.
- **Missing dependency errors:** Install and start the dependencies required by this resource.
- **Items or purchases do not work:** Review the server console, item definitions, and any framework or inventory integration required by your version.

## 🤝 Support

For support, bug reports, or suggestions, open an issue in this repository and include:
- The error message from the console
- Steps to reproduce the issue
- Your FiveM framework and relevant dependency versions

## 📄 License

Unless a separate license file or license statement is included in this repository, do not assume that the code is open-source licensed or that redistribution is permitted. Add your chosen license before publishing if you own the rights to do so.

---

Made with ❤️ by **Nexo Studio**
