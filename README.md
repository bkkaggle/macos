# MacOS

# settings

- Desktop
  - wallpaper1
- Dock
  - show recent: off
- users and groups
  - drag wallpaper2 to image
- touchpad
  - tap to click: on
  - tracking speed: fast
- display
  - night shift
    - schedule: sunset to sunrise
- energy saver
  - slightly dim display: off
- security
  - password immediately

# Finder

- drag photos to favorites

# dock

- finder
- chrome
- mail
  - settings
    - composing
      - automatically cc myself: on
- photos
- apps
- settings
- vscode
- terminal
  - font: 16
  - keyboard
    - option as meta key: on
- pocket

# apps

- zsh
  - run `chsh -s /bin/zsh``

- chrome
  - sync
    - turn off history
    
- vscode
    - get settings from settings sync
    
    - create `~/.prettierrc` with:
    
```
{
  "jsxSingleQuote": true,
  "semi": false,
  "singleQuote": true,
  "tabWidth": 4,
  "printWidth": 100,
  "useTabs": true
}
```

- git
  - installer from https://git-scm.com/downloads
  - `git config --global user.email "bk@tinymanager.com"`
  - `git config --global user.name "Bilal Khan"`
  - `git config --global credential.helper osxkeychain`
  - `git config --global credential.helper 'cache --timeout=84000'`
  
  - git lfs
    - follow https://git-lfs.github.com/
    - `brew install git-lfs`
    - `git lfs install`
    
    
 - nvm
  - `touch ~/.zshrc`
  - `curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.0/install.sh | bash`
  - `nvm install --lts`
  - `nvm use --lts`
  - `nvm alias default 12.13.1` (replace with lts version)
  
  - gatsby
    - `npm install -g gatsby-cli`
  
  - expo
    - `npm install expo-cli --global`

- conda
  - download latest from https://docs.conda.io/en/latest/miniconda.html
  - `bash Miniconda3-latest-MacOSX-x86_64.sh`
  - init conda
  - copy conda lines from ~/.bash_profile to ~/.zshrc
  - restart terminal
  - environment
    - `conda create -n pytorch python=3.7`
    - `pip install tensorflow`
    - `conda install pytorch torchvision cpuonly -c pytorch`
    - `conda install pandas scikit-learn pylint`
    - `pip install scikit-image tqdm mlcrate pytorch_zoo fire pre-commit kaggle twine`
    
    - kaggle api
      - add api token to `/home/bilal/.kaggle/kaggle.json`
    
    - gcloud (system python)
      - download from https://cloud.google.com/sdk/docs/
      - `./google-cloud-sdk/install.sh`
      - `gcloud init`
      
      - proxy: 
        - `curl -o cloud_sql_proxy https://dl.google.com/cloudsql/cloud_sql_proxy.darwin.amd64`
        - `chmod +x cloud_sql_proxy`

- homebrew
  - `/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`
  
  - wget: `brew install wget`


- c++
  - download xcode and developer tools
  - follow https://www.devsbedevin.net/vscode-debugging-c-cpp-code-on-macos-catalina/ for debugging
  - `brew install cmake`


- ssh
  - disable ports and no password logins
  - follow https://www.ssh.com/ssh/copy-id
  - `ssh-keygen`
  - `ssh-copy-id -i ~/.ssh/mykey user@host`
  - `ssh -i ~/.ssh/mykey user@host`
  - renable ports and no password logins

- mysql workbench
