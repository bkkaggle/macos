# macos

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

# Finder

- drag photos to favorites

# dock

- finder
- chrome
- mail
- photos
- apps
- settings
- vscode


# apps

- zsh
  - run `chsh -s /bin/zsh``

- chrome
  - sync
    - turn off history
    
- vscode

- iterm2

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
    - `conda install pandas scikit-learn`
    - `pip install scikit-image tqdm mlcrate pytorch_zoo fire pre-commit kaggle`
    
    - kaggle api
      - TODO: add api token to `/home/bilal/.kaggle/kaggle.json`
    
    - gcloud (system python)
      - download from https://cloud.google.com/sdk/docs/
      - `./google-cloud-sdk/install.sh`
      - `gcloud init`
      
 
      

- homebrew
  - `/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`
