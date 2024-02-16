<h1 align="center">
  <br>
  🕹️ Arcade theme for SDDM
  <br>
</h1>

<figure>
  <img src="preview.jpg" alt="Screenshot"/>
  <h5 align="center"><b>Login screenshot</b></h5>
</figure>

🚀 Dive into the ultimate gaming nostalgia with this electrifying login theme. Witness the glow
of neon lights, reminiscent of classic arcades and immerse yourself in the vibrant world of
pixelated wonders as your login screen transforms into a virtual arcade gaming room. 🔥

### Dependencies 🎮

  * sddm
  * qt5
  * qt5-quickcontrols
  * qt5-graphicaleffects
  * ttf-jetbrains-mono

### How to install it

```bash
# Clone this repo
git clone https://github.com/v1nns/sddm-arcade /tmp/arcade

# Move it to default themes path used by SDDM
sudo mv /tmp/arcade /usr/share/sddm/themes/
```

After these steps, you must change default theme inside the SDDM configuration file (default path is
*/usr/lib/sddm/sddm.conf.d/default.conf*).

```ini
[Theme]
# Current theme name
Current=arcade
```

> [!WARNING]
> If your login screen is rendering a larger font regardless of the font size inside the theme.conf (and you have HiDPI enabled), you may also include this setting in *default.conf*:
>
> ```ini
> [X11]
> ServerArguments=-nolisten tcp -dpi 96
> ```
> *P.S.: Change DPI to match a value that your monitor can handle.*

> [!TIP]
> For a detailed description about SDDM settings, check [this](https://wiki.archlinux.org/title/SDDM).

### Credits

- Based on the theme [`Chili login theme for SDDM`](https://github.com/MarianArlt/sddm-chili) by [**MarianArlt**](https://github.com/MarianArlt).

### License

This project is licensed under the GPLv3 License - see the [LICENSE](LICENSE.md) for details
