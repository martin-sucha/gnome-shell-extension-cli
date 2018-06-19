gnome-shell-extension-cli
=========================

A simple command line tool to manage Gnome Shell extensions.

An extension can be specified either using it's UUID or
a extensions.gnome.org URL.

Examples
--------

Install and enable an extension:

```
gnome-shell-extension-cli install drive-menu@gnome-shell-extensions.gcampax.github.com
# or
gnome-shell-extension-cli install https://extensions.gnome.org/extension/7/removable-drive-menu/
```

Just install, don't enable:

```
gnome-shell-extension-cli install --no-enable drive-menu@gnome-shell-extensions.gcampax.github.com
```

Install system-wide:

```
gnome-shell-extension-cli install --system drive-menu@gnome-shell-extensions.gcampax.github.com
```

Uninstall:

```
gnome-shell-extension-cli uninstall drive-menu@gnome-shell-extensions.gcampax.github.com
```

Enable/Disable/Reload:

```
gnome-shell-extension-cli enable drive-menu@gnome-shell-extensions.gcampax.github.com
gnome-shell-extension-cli disable drive-menu@gnome-shell-extensions.gcampax.github.com
gnome-shell-extension-cli reload drive-menu@gnome-shell-extensions.gcampax.github.com
```

List extensions (from running Gnome Shell):

```
gnome-shell-extension-cli list
# or as raw JSON
gnome-shell-extension-cli list --json
```

Fetch extension info from extensions.gnome.org

```
gnome-shell-extension-cli info drive-menu@gnome-shell-extensions.gcampax.github.com
# or as JSON
gnome-shell-extension-cli info --json drive-menu@gnome-shell-extensions.gcampax.github.com
```
