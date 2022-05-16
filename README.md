# OhMyPosh

## ChromeOs

Download Oh My Posh
```bash
sudo wget https://github.com/JanDeDobbeleer/oh-my-posh/releases/latest/download/posh-linux-amd64 -O /usr/local/bin/oh-my-posh
sudo chmod +x /usr/local/bin/oh-my-posh

```

Install themes
```bash
mkdir ~/.poshthemes
wget https://github.com/JanDeDobbeleer/oh-my-posh/releases/latest/download/themes.zip -O ~/.poshthemes/themes.zip
unzip ~/.poshthemes/themes.zip -d ~/.poshthemes
chmod u+rw ~/.poshthemes/*.json
rm ~/.poshthemes/themes.zip

```

Ctrl+Shift+J to open dev console, input following code to get NERD font support.
```javascript
term_.prefs_.set('font-family', 'MesloLGM NF');
term_.prefs_.set('user-css-text', '@font-face {font-family: "MesloLGM NF"; src: url("https://raw.githubusercontent.com/ryanoasis/nerd-fonts/master/patched-fonts/Meslo/M/Regular/complete/Meslo%20LG%20M%20Regular%20Nerd%20Font%20Complete.ttf"); font-weight: normal; font-style: normal;}')
```

ANd in .bashrc
```
eval "$(oh-my-posh init bash --config ~/.poshthemes/wolojoli.omp.json)"
```
