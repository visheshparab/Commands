## Node Version Manager (NVM)

#### install nvm(node version manager)

    - brew install nvm
    - source $(brew --prefix nvm)/nvm.sh
    - echo 'source $(brew --prefix nvm)/nvm.sh' >> ~/.profile

#### Upgrade nvm

    - nvm upgrade

#### Display nvm version

    - nvm v
    - nvm -v
    - nvm --v
    - nvm version
    - nvm -version
    - nvm --version

#### list all available node version

    - Win: nvm list available

#### Install latest LTS node version

    - Win: nvm install lts

#### Install latest node version

    - Win: nvm install latest

#### install specific node version

    - nvm install [version]

#### Reinstall node

    - nvm reinstall [version]

#### use specific node version

    - nvm use [version]

#### list all node version installed

    - nvm ls
    - nvm list

#### Display active node version.

    - nvm current

#### Show if node is running in 32 or 64 bit mode.

    - nvm arch

#### Uninstall specific node version

    - nvm uninstall [version]

#### Set the directory where nvm should store different versions of node.js. If <path> is not set, the current root will be displayed.

    - nvm root [path]

---

#### brew services list

    - brew services list

---

## PostgreSQL

#### Install postgreSql

    - brew install postgresql@[version]

#### If you need to have postgresql@17 first in your PATH, run:

    - echo 'export PATH="/opt/homebrew/opt/postgresql@17/bin:$PATH"' >> ~/.zshrc

#### For compilers to find postgresql@17 you may need to set:

    - export LDFLAGS="-L/opt/homebrew/opt/postgresql@17/lib"
    - export CPPFLAGS="-I/opt/homebrew/opt/postgresql@17/include"

#### To start postgresql@17 now and restart at login:

    - brew services start postgresql@17

#### Or, if you don't want/need a background service you can just run:

    - LC_ALL="C" /opt/homebrew/opt/postgresql@17/bin/postgres -D /opt/homebrew/var/postgresql@17

#### Check version

    - postgres --version
    - psql --version

#### list all postgresql paths

    - brew list postgresql@[version]

#### information to set path and start postgresql service

    - brew info postgresql@[version]

#### path of postgresql

    - which postgres

---
