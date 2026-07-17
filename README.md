These are my dotfiles for backend software development on macOS.

# Install the packages from the Brewfile with Homebrew

On a fresh installation of macOS:

1. Open the Terminal app.

2. Go to your home directory (the one containing `Desktop`, `Documents`, and `Downloads`):

   ```bash
   cd ~
   ```

3. Create a directory named `Code`:

   ```bash
   mkdir Code
   ```

4. Clone this dotfiles repository into `~/Code`:

   ```bash
   git clone https://github.com/chararchter/dotfiles.git ~/Code/dotfiles
   ```

   On a fresh macOS, this command prompts you to install the Xcode Command Line Tools, which provide `git`. Accept the prompt, wait for the install to finish, then run the command again.

5. Install [Homebrew](https://brew.sh):

   ```bash
   /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
   ```

6. Change into the `dotfiles` directory, which contains the `Brewfile`, and install the packages listed in it:

   ```bash
   cd ~/Code/dotfiles
   brew bundle
   ```

# Troubleshooting

After installing the packages:

1. Check that a package installed correctly by printing its version. Replace `<command>` with the tool you want to check (for example, `git`):

   ```bash
   <command> --version
   ```

2. If the version is missing or not the one you expected, show which executable the shell runs for that command:

   ```bash
   which <command>
   type -a <command>
   ```

   If the shell still points to an old executable, clear its cached command locations:

   ```bash
   hash -r
   ```

   Then run the version check from step 1 again.
