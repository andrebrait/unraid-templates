# unraid-templates

Unraid Docker and plugin templates maintained by André Brait.

| Template | Type | Application |
|---|---|---|
| [fanctrlplus2](templates/fanctrlplus2.xml) | Plugin | [FanCtrl Plus 2](https://github.com/andrebrait/fanctrlplus) |
| [protonvpn](templates/protonvpn.xml) | Docker | [Proton VPN CLI container](https://github.com/andrebrait/protonvpn-cli-docker) |
| [usb-sleep](templates/usb-sleep.xml) | Plugin | [USB Sleep](https://github.com/andrebrait/unraid-usb-sleep) |

## Installing a template

FanCtrl Plus 2 is listed in Community Applications. Install it from the **Apps** tab, or install the plugin directly from **Plugins → Install Plugin** with:

```text
https://raw.githubusercontent.com/andrebrait/fanctrlplus/main/plugin/fanctrlplus2.plg
```

USB Sleep is pending Community Applications review; until it is listed, install it from **Plugins → Install Plugin** with:

```text
https://raw.githubusercontent.com/andrebrait/unraid-usb-sleep/main/usb-sleep.plg
```

The Docker templates are not yet listed in Community Applications. To add one manually, run this in the Unraid terminal:

```bash
wget -O /boot/config/plugins/dockerMan/templates-user/my-protonvpn.xml \
  https://raw.githubusercontent.com/andrebrait/unraid-templates/main/templates/protonvpn.xml
```

Then open **Docker → Add Container** and select **protonvpn** under the user templates.

## Support

Report problems with an application in its own repository; each template's **Support** link points there. Report template-only problems, such as a wrong default or field description, in this repository.
