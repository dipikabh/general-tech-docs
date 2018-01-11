
# Steps to Install and Configure SublimeLinter Plugin in Sublime Text 3

1. Install the linter executable - e.g. pycodestyle (new name of pep8)

   ```bash
   pip install --user pycodestyle
   ```
   This will install the linter in your home directory. In this case, the executable will get stored in: `~/Library/Python/2.7/bin/pycodestyle`.
2. Install the sublimelint plugin for the linter. Since we have chosen the 
   pycodestyle linter, we need to install the `sublimelinter-pycodestyle` plugin.
3. Configure Sublime Text to look for executables in the path in which the 
   linter executable was installed. i.e. in Sublimelinter user settings, put
   the following:

   ```json
           "paths": {
            "osx": [
                "~/Library/Python/2.7/bin/"
            ]
        },
   ```

You might need to restart ST3 after this.