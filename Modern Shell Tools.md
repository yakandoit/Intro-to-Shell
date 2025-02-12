Finding Files
Logo
GitHub - junegunn/fzf: A command-line fuzzy finder
GitHub
WSL/Linux
MacOS
Copy
brew install fzf
Once installed, do:

fzf stands for fuzzy finder. It allows you to find anything with a fuzzy search (you can make spelling errors). If you just run fzf, it will do a fuzzy find on your current directory

Copy
fzf
But we can do so much more than that! To do so, we need to add some keybindings by running this command:

Copy
eval "$(fzf --bash)"
Now try out these new keybindings:

CTRL-T - Paste the selected files and directories onto the command-line

CTRL-R - Paste the selected command from history onto the command-line

ALT-C - cd into the selected directory

Now notice that if you quit the terminal or start a new terminal, these keybindings won't be available. To make the change permanent, we need to save it into a config file. For bash, this config file is is at ~/.bashrc

Copy
nano ~/.bashrc

## Inside the editor, add this line
eval "$(fzf --bash)"
