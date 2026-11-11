# unraid-templates

Unraid Docker and plugin templates maintained by André Brait.

| Template | Type | Application |
|---|---|---|
| [fanctrlplus2](templates/fanctrlplus2.xml) | Plugin | [FanCtrl Plus 2](https://github.com/andrebrait/fanctrlplus) |
| [nut-dw](templates/nut-dw.xml) | Plugin | [Network UPS Tools (NUT) for UNRAID](https://github.com/andrebrait/NUT-unRAID), fork of desertwitch's plugin |
| [dwttm](templates/dwttm.xml) | Plugin | [Tmux Terminal Manager (TTM)](https://github.com/andrebrait/TTM-unRAID), fork of desertwitch's plugin |
| [unRAID6-Sanoid](templates/unRAID6-Sanoid.xml) | Plugin | [Sanoid](https://github.com/andrebrait/unRAID6-Sainoid), fork of steini84's plugin |
| [enhanced.log](templates/enhanced.log.xml) | Plugin | [Enhanced Log v2](https://github.com/andrebrait/unraid-enhancedlog), fork of Derek Kaser's plugin |
| [open.files](templates/open.files.xml) | Plugin | [Open Files v2](https://github.com/andrebrait/unraid-openfiles), fork of Derek Kaser's plugin |
| [protonvpn](templates/protonvpn.xml) | Docker | [Proton VPN CLI container](https://github.com/andrebrait/protonvpn-cli-docker) |

## Installing a template

FanCtrl Plus 2 is listed in Community Applications. Install it from the **Apps** tab, or install the plugin directly from **Plugins → Install Plugin** with:

```text
https://raw.githubusercontent.com/andrebrait/fanctrlplus/main/plugin/fanctrlplus2.plg
```

The NUT, TTM, Sanoid, Enhanced Log and Open Files plugins are forks of existing plugins. They keep the original plugin filename (for example `nut-dw.plg`), so they cannot be installed next to the original plugin. Their templates are pending Community Applications review; until they are listed, install them from **Plugins → Install Plugin** with:

```text
https://raw.githubusercontent.com/andrebrait/NUT-unRAID/master/plugin/nut-dw.plg
https://raw.githubusercontent.com/andrebrait/TTM-unRAID/main/plugin/dwttm.plg
https://raw.githubusercontent.com/andrebrait/unRAID6-Sainoid/master/unRAID6-Sanoid.plg
https://raw.githubusercontent.com/andrebrait/unraid-enhancedlog/main/plugin/enhanced.log.plg
https://raw.githubusercontent.com/andrebrait/unraid-openfiles/main/plugin/open.files.plg
```

The Docker templates are not yet listed in Community Applications. To add one manually, run this in the Unraid terminal:

```bash
wget -O /boot/config/plugins/dockerMan/templates-user/my-protonvpn.xml \
  https://raw.githubusercontent.com/andrebrait/unraid-templates/main/templates/protonvpn.xml
```

Then open **Docker → Add Container** and select **protonvpn** under the user templates.

## Support

Report problems with an application in its own repository; each template's **Support** link points there. Report template-only problems, such as a wrong default or field description, in this repository.
