These are my dotfiles for backend software development on Mac.

On a fresh installation of macOS:

1. Open Terminal.
2. Go to your home directory (the one containing `Desktop`, `Documents`, and `Downloads`):

   ```bash
   cd ~
   ```

3. Create a directory for your code:

   ```bash
   mkdir Code
   ```

4. Download this dotfiles repo into `~/Code`.

5. Install [Homebrew](https://brew.sh):

   ```bash
   /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
   ```

6. Change into the directory containing the `Brewfile` and install everything:

   ```bash
   brew bundle
   ```
