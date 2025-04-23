# ⚙️ Laravel Project Installer Scripts

This repository contains Bash scripts to help you quickly scaffold Laravel projects with optional support for [FilamentPHP](https://filamentphp.com/) and [Nutgram](https://github.com/nutgram/nutgram-laravel).  

📁 Scripts are designed to be stored in: `~/.config/bin`  
🖥️ Make sure this directory is in your `$PATH` for easy access.
---

## 📦 Installation

1. **Clone the repository into `~/.config/bin`:**

   ```bash
   git clone https://github.com/your-username/your-repo.git ~/.config/bin
   ```

2. **Make sure the scripts are executable:**

   ```bash
   chmod +x ~/.config/bin/*
   ```

3. **(Optional)** Add `~/.config/bin` to your shell's PATH:

   - For **bash/zsh** users, add this to `~/.bashrc` or `~/.zshrc`:

     ```bash
     export PATH="$HOME/.config/bin:$PATH"
     ```

   - Reload your shell:

     ```bash
     source ~/.bashrc  # or source ~/.zshrc
     ```

---

## 🚀 Usage

Run the Laravel setup script like so:

```bash
./laravel my_project_name [options]
```

Or, if you added it to your `$PATH`:

```bash
laravel my_project_name [options]
```

### Options

| Option        | Description                                    |
|---------------|------------------------------------------------|
| `--sqlite`    | Use SQLite instead of MySQL                    |
| `--migrate`   | Run `php artisan migrate` after install        |
| `--filament`  | Install and configure FilamentPHP              |
| `--nutgram`   | Install and configure Nutgram Telegram bot     |
| `--force`     | Delete the existing folder if it exists        |

---

## 🧰 File Structure

- `laravel` – Main script to create Laravel projects.
- `filament` – Sub-script to set up FilamentPHP.
- `nutgram` – Sub-script to set up Nutgram Telegram bot.

These are sourced automatically by the main script.

---

## 🛡️ Safety

When using the `--force` flag:
- You will be prompted before deleting an existing project folder.
- Pressing `Enter` or typing `y` confirms deletion.

---

## 🧑‍💻 Author

Made by Diyorbek Turg'unboyev \
Backend Developer | PHP, Laravel

---

## 🪪 License

MIT