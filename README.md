# 🚀 ARCHITECT SCRIPT

A post-install script designed to set up a complete and ready-to-use **Arch Linux system** right after using `archinstall`. Optimized for **gamers**, this script provides modular configuration options, minimal bloat, and performance in mind.

---

> ⚠️ **DISCLAIMER**  
> This script is derived from personal post-install notes and fully suits my hardware and needs. It has been thoroughly tested on my system but **comes with no warranty** for compatibility on your machine.
>
> This is not a distribution. It's a helper to **speed up post-installation**, and its maintenance is your responsibility.
>
> Arch Linux is a **DIY (Do It Yourself)** distribution. It assumes you have technical knowledge or are willing to read the documentation. If you're not self-sufficient, Arch is not for you.
>
> > 📌 From the [Arch Wiki](https://wiki.archlinux.org/title/Arch_Linux):  
> > _"While many GNU/Linux distributions attempt to be more user-friendly, Arch Linux has always been and will remain a user-centric distribution. It is designed for competent GNU/Linux users who are willing to read documentation and solve their own problems."_  
> >
> > Running Arch without reading documentation defeats its purpose.
> > 
> 🧠 **Note:** If you are using an **NVIDIA GPU**, it must be from the **16xx (Turing) series or newer** to use the **`nvidia-open-dkms`** driver (open kernel modules).  
>  
> If you own a **Pascal GTX 10xx** or an **older GPU** (e.g., **Maxwell**, **Kepler**, or earlier such as **GTX 9xx / 8xx / 7xx**), you need the **proprietary driver** instead.  
> In that case, run the following command after the script:
> ```bash
> sudo pacman -S nvidia-dkms
> ```
> When prompted by `pacman`, **replace** `nvidia-open-dkms` with `nvidia-dkms`.
> > ⚠️ **Important information:**  
> [NVIDIA is planning to drop support for its Maxwell, Pascal, and Volta GPUs, along with the legacy proprietary driver](https://www.phoronix.com/news/Maxwell-Pascal-Volta-Legacy-Near).  
> If you're using one of these GPUs, it's strongly recommended to upgrade to a newer graphics card, ideally an **AMD GPU** or a **NVIDIA Turing or newer** model that supports the new open kernel modules (`nvidia-open`).

---

## ⚙️ Installation Command

```bash
sudo pacman -S --needed git base-devel \
  && git clone https://github.com/ryemislam/Architect.git ~/Architect \
  && cd ~/Architect \
  && chmod +x ./architect.sh \
  && ./architect.sh
```

At the end of the script, you can delete the ~/Architect folder.

## 🧩 Features Overview

1. **Pacman Setup** — Optimized package manager (parallel downloads, color, etc.)
2. **Shell Aliases** — Fast commands like:
   - `update-arch`
   - `clean-arch`
   - `fix-key`
   - `update-mirrors`
3. **GPU Configuration** — NVIDIA/AMD/Intel setup.
4. **AUR Support** — Install `yay` or `paru`, depending on your preference.
5. **Optional Components** — Printers, Firewall, Bluetooth, Sound, etc.
6. **Extra Software** — Browsers, games, apps, media tools, and more.

---

## 🔗 Resources

- 📖 [ArchWiki](https://wiki.archlinux.org/)
- [📚 Architect Wiki](https://github.com/Cardiacman13/Architect/wiki)
---
