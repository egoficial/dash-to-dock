# Dash to Dock - Modified Version

This GNOME Shell extension moves the dash out of the overview, transforming it into a dock for easier application launching and faster window and desktop switching without leaving the desktop view.

![Preview](https://raw.githubusercontent.com/egoficial/dash-to-dock/refs/heads/main/media/preview.png)

## Modifications
- Changed $base_padding to 6px.
- Changed $base_border_radius to 6px.
- Changed $remark_color (Alpha) to 0.
- Changed $dash_padding (It is no longer multiplied by 2)
- Changed $dash_padding (4px is no longer added)
- Changed set-internal-children-property ($dock_icons_distance is no longer divided by 2)


## Installation from Source
To install the extension from source, clone the repository and build it.

### Build Dependencies
To compile the stylesheet, an implementation of SASS is required. Dash to Dock supports dart-sass (sass), sassc, and ruby-sass. We recommend using dart-sass (sass) or sassc, as ruby-sass is deprecated.

By default, Dash to Dock builds with sassc. To change this behavior, set the SASS environment variable:

```sh
export SASS=dart  # or export SASS=ruby
```

### Building and Installing
Clone the repository and install the extension:

```sh
git clone git@github.com:egoficial/dash-to-dock.git dash-to-dock
make -C dash-to-dock install
```

After installation, reload the GNOME Shell:
- Under Xorg: Press `Alt+F2`, type `r`, and press `Enter`.
- Under Wayland: Log out and log back in.

Enable the extension using `gnome-extensions-app` (GNOME Extensions) or `dconf`.

If `msgfmt` is missing, install the `gettext` package from your distribution's repository.

For more details, visit the original project: [Dash to Dock](https://micheleg.github.io/dash-to-dock/).
