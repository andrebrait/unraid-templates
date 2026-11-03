# unraid-templates

Unraid Docker templates maintained by André Brait.

| Template | Application |
|---|---|
| [protonvpn-cli](templates/protonvpn-cli.xml) | [Proton VPN CLI container](https://github.com/andrebrait/protonvpn-cli-docker) |

## Installing a template

These templates are not yet listed in Community Applications. To add one manually, run this in the Unraid terminal:

```bash
wget -O /boot/config/plugins/dockerMan/templates-user/my-protonvpn-cli.xml \
  https://raw.githubusercontent.com/andrebrait/unraid-templates/main/templates/protonvpn-cli.xml
```

Then open **Docker → Add Container** and select **protonvpn-cli** under the user templates.

## Support

Report problems with an application in its own repository; each template's **Support** link points there. Report template-only problems, such as a wrong default or field description, in this repository.
