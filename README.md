# P7 Ember: a consistent dark and orange desktop for Fedora 45 / GNOME 51

A personal, dark-only GNOME theme set built around one idea: **the whole system should look like one design**, from the boot menu to the third-party apps. It uses soft-3D surfaces, flat faces, one orange accent (`#F5732A`), smoked-glass popups and a topographic "Ember Layers" wallpaper.

![Desktop](08-top-calendar.png)

## Screenshots

### Boot and login

| | |
|---|---|
| ![GRUB boot menu](01-grub.png) GRUB boot menu | ![Plymouth boot splash](02-plymouth.png) Plymouth boot splash |
| ![Login screen (GDM)](03-gdm-user-list.png) Login screen (GDM) | ![Log out dialog](04-log-out.png) Log out dialog |
| ![Lock screen](05-lock-screen.png) Lock screen | ![Unlock prompt](06-unlock.png) Unlock prompt |

> These six screens cannot be captured with a screenshot tool, so they were photographed on the laptop and then re-created at full resolution (2560×1600) from the theme's own artwork, stylesheets and fonts.

### Desktop and apps

| | |
|---|---|
| ![Quick Settings and power menu](07-quick-settings.png) Quick Settings and power menu | ![Calendar and notifications](08-top-calendar.png) Calendar and notifications |
| ![System monitor (Vitals)](09-vitals.png) System monitor (Vitals) | ![Ulauncher](10-ulauncher.png) Ulauncher |
| ![Extension Manager and Blur my Shell](11-extensions.png) Extension Manager and Blur my Shell | ![Files](12-home-folder.png) Files |
| ![Settings](13-settings.png) Settings | ![Terminal (Ptyxis)](14-terminal.png) Terminal (Ptyxis) |
| ![Midnight Commander](15-midnight-commander.png) Midnight Commander | ![GIMP splash](16-gimp-splash.png) GIMP splash |
| ![GIMP](17-gimp.png) GIMP | ![Overview](18-overview.png) Overview |
| ![Applications](19-applications.png) Applications | ![FileZilla](20-filezilla.png) FileZilla |
| ![VS Code](21-vsc.png) VS Code | ![Tweaks](22-tweaks.png) Tweaks |
| ![Music](23-music.png) Music | ![Video Player](24-video.png) Video Player |
| ![Evolution](25-evolution.png) Evolution | ![Planify](26-planify.png) Planify |
| ![Files: rename dialog](27-folder-rename-popup.png) Files: rename dialog | ![Software](28-software.png) Software |
| ![Calendar](29-calendar.png) Calendar | ![gedit](30-gedit.png) gedit |
| ![Calculator, Weather, Clocks and Maps](31-accessories.png) Calculator, Weather, Clocks and Maps |  |

## What is themed

- **Boot:** GRUB theme with custom artwork and selection pill; Plymouth boot splash
- **Login and lock screen:** GDM theme rebuilt into the system gresource (user list, password field with an orange "next" button, calendar and Quick Settings)
- **GNOME Shell:** top bar, Quick Settings, calendar and notifications with smoked/frosted glass, menus, dock, exit dialogs
- **GTK 4 / libadwaita and GTK 3:** P7-Dark, with pill buttons, two-tone surfaces and orange selection
- **Icons:** P7-Icons, a generated set with a dark tile, light-orange rim, white glyph and one orange accent
- **Cursors:** P7-Ember-Cursors
- **Terminal:** Ptyxis palette "P7 Ember" with light glass
- **Apps:**
  - VS Code colour theme and activity-bar icon theme
  - Firefox (userChrome/userContent)
  - Chrome colour theme
  - GIMP theme "P7-Flat" and splash
  - FileZilla icon set
  - Evolution
  - Ulauncher theme
  - Glass Widgets skin
- **Wallpapers:** "Ember Layers" variants, generated for this project (2560×1600 and 3840×2400)

## Extensions used

User Themes, Blur my Shell, Dash to Dock, Just Perfection, Tiling Shell, Vitals, Weather O'Clock, Modern Clock, Clipboard Indicator, Color Picker, Removable Drive Menu, Unblank lock screen, Pigeon Email Notifier, Auto Move Windows, Glass Widgets, Customize Clock on Lock Screen

## Credits

- GTK and Shell themes built on [WhiteSur](https://github.com/vinceliuice/WhiteSur-gtk-theme) by vinceliuice
- Icon fallback: Slot-Dark-Icons
- Fonts: [Inter](https://rsms.me/inter/) by Rasmus Andersson and [JetBrains Mono](https://www.jetbrains.com/lp/mono/) by JetBrains (both SIL Open Font License)
- The authors of the extensions listed above
- Design and testing: me
- Design work, code and troubleshooting: [Claude](https://www.anthropic.com/claude) (Anthropic)

## How Claude helped

I designed the look and tested every step; Claude did the technical work with me over several sessions:

- **Design:** turned my mockups and reference images into a written design system (colours, shadows, button and glass rules) and kept every component consistent with it
- **Code:** wrote the GTK 3/4 and GNOME Shell CSS/SCSS layers, the GDM gresource build, the Firefox and Ulauncher styles, and the VS Code theme and icon-font extension
- **Generated assets:** wrote Python scripts that generate the icon set, the GRUB graphics, the cursors and the wallpapers
- **Installers:** wrote install scripts with backups and an undo option for every change, plus a release pack
- **Testing:**
  - operated a Fedora virtual machine directly through screen control
  - read my laptop screenshots, down to sampling exact pixel colours
  - read diagnostic logs to find root causes (for example, an old theme overriding GTK 3 apps, or the lock screen using the system theme)
- **Research:** checked current documentation and release notes (GNOME Shell, Blur my Shell, VS Code, Firefox, GIMP 3)
- **Quality:** used separate reviewer agents to check scripts before I ran them
- **Screenshots:** re-created the boot and login screens from my photos, using the theme's real assets

## Status

Personal setup for my laptop (Fedora 45 Workstation, GNOME Shell 51, Wayland, 2560×1600 at 125 %). The theme files are not published yet.
