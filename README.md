# 🌟 Starship Prompt Config Backup

This repository contains my personal backup configuration for the [Starship](https://starship.rs) prompt.  
Feel free to use or modify it to suit your own terminal setup.

![Preview](ss.png)

---

## 📂 File: `starship.toml`

To use this configuration, follow the steps below:

### 📥 Installation

1. Copy the file to your local configuration directory:
   ```bash
   mkdir -p ~/.config
   cp starship.toml ~/.config/starship.toml
   ```

2. Or edit directly with:
   ```bash
   sudo nano ~/.config/starship.toml
   ```

> 💡 Make sure you have [Starship](https://starship.rs/guide/#%F0%9F%9A%80-installation) installed on your system.

---

## ⚙️ Configuration

```toml
add_newline = false
format = "$os$hostname$username$directory\n$character"

palette = "custom"

[palettes.custom]
bg_1 = "#3c8630"
bg_2 = "#ffffff"
fg_1 = "#000000"
fg_2 = "#ffffff"

[os]
format = '[🌐 Arch ](fg:fg_2 bg:bg_1)[](fg:bg_1 bg:bg_2)'
disabled = false

[hostname]
format = '[  $hostname ](fg:fg_1 bg:bg_2)[](fg:bg_2 bg:bg_1)'
ssh_only = false

[username]
format = '[ 👤 $user ](fg:fg_2 bg:bg_1)[](fg:bg_1 bg:bg_2)'
show_always = true

[directory]
format = '[ 📁 $path ](fg:fg_1 bg:bg_2)[](fg:bg_2 bg:none)'
truncation_length = 3
truncation_symbol = "…/"

[character]
success_symbol = "[➜](bold green)"
error_symbol = "[✗](bold red)"
vicmd_symbol = "[](bold yellow)"
```
3. Finish:
   ```
   CTRL + O & CTRL + X
   ```
