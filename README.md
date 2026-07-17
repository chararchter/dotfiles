This is my dotfile for backend software development on Mac.

# Install everything from Brewfile with Homebrew
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

# Troubleshooting
After installing packages:

1. Verify installation:
   ```bash
   <command> --version
    ```


2. If the version is missing or unexpected:

Check which executable is being used:
  ```bash
  which <command>
  type -a <command>
  ```

If an old location is cached, clear it:
  ```bash
  hash -r
  ```

Run the version check again.
