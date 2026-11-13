# unraid-templates

Unraid Docker and plugin templates maintained by André Brait.

| Template | Type | Application |
|---|---|---|
| [fanctrlplus2](templates/fanctrlplus2.xml) | Plugin | [FanCtrl Plus 2](https://github.com/andrebrait/fanctrlplus) |
| [nut3](templates/nut3.xml) | Plugin | [NUT v3](https://github.com/andrebrait/NUT-unRAID), successor to desertwitch's Network UPS Tools (NUT) for UNRAID |
| [ttm2](templates/ttm2.xml) | Plugin | [TTM v2](https://github.com/andrebrait/TTM-unRAID), successor to desertwitch's Tmux Terminal Manager (TTM) |
| [sanoid](templates/sanoid.xml) | Plugin | [Sanoid](https://github.com/andrebrait/unraid-sanoid), successor to steini84's Sanoid plugin |
| [enhanced.log3](templates/enhanced.log3.xml) | Plugin | [Enhanced Log v3](https://github.com/andrebrait/unraid-enhancedlog), successor to Derek Kaser's Enhanced Log v2 |
| [open.files3](templates/open.files3.xml) | Plugin | [Open Files v3](https://github.com/andrebrait/unraid-openfiles), successor to Derek Kaser's Open Files v2 |
| [nerdtools](templates/nerdtools.xml) | Plugin | [NerdTools](https://github.com/andrebrait/unRAID-NerdTools), continuation of UnRAIDES' NerdTools |
| [protonvpn](templates/protonvpn.xml) | Docker | [Proton VPN CLI container](https://github.com/andrebrait/protonvpn-cli-docker) |
| [usb-sleep](templates/usb-sleep.xml) | Plugin | [USB Sleep](https://github.com/andrebrait/unraid-usb-sleep) |

## Installing a template

FanCtrl Plus 2 is listed in Community Applications. Install it from the **Apps** tab, or install the plugin directly from **Plugins → Install Plugin** with:

```text
https://raw.githubusercontent.com/andrebrait/fanctrlplus/main/plugin/fanctrlplus2.plg
```

The NUT v3, TTM v2, Enhanced Log v3, Open Files v3 and Sanoid plugins are new plugins that replace plugins their original authors no longer maintain (the same way FolderView3 replaced FolderView2). They use their own plugin names, so they do not clash with the originals. Installing one copies the settings of the old plugin and removes it. All five were tested on Unraid 7.4.0. Their templates are pending Community Applications review; until they are listed, install them from **Plugins → Install Plugin** with:

```text
https://raw.githubusercontent.com/andrebrait/NUT-unRAID/master/plugin/nut3.plg
https://raw.githubusercontent.com/andrebrait/TTM-unRAID/main/plugin/ttm2.plg
https://raw.githubusercontent.com/andrebrait/unraid-sanoid/master/sanoid.plg
https://raw.githubusercontent.com/andrebrait/unraid-enhancedlog/main/plugin/enhanced.log3.plg
https://raw.githubusercontent.com/andrebrait/unraid-openfiles/main/plugin/open.files3.plg
```

USB Sleep is pending Community Applications review; until it is listed, install it from **Plugins → Install Plugin** with:

```text
https://raw.githubusercontent.com/andrebrait/unraid-usb-sleep/main/usb-sleep.plg
```

NerdTools is pending Community Applications review. It keeps the original plugin name, so it updates an existing NerdTools install in place. Until it is listed, install it from **Plugins → Install Plugin** with:

```text
https://github.com/andrebrait/unRAID-NerdTools/releases/latest/download/NerdTools.plg
```

The Docker templates are not yet listed in Community Applications. To add one manually, run this in the Unraid terminal:

```bash
wget -O /boot/config/plugins/dockerMan/templates-user/my-protonvpn.xml \
  https://raw.githubusercontent.com/andrebrait/unraid-templates/main/templates/protonvpn.xml
```

Then open **Docker → Add Container** and select **protonvpn** under the user templates.

## Support

Report problems with an application in its own repository; each template's **Support** link points there. Report template-only problems, such as a wrong default or field description, in this repository.
