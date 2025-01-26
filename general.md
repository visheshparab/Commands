#### install nvm(node version manager)

- brew install nvm
- source $(brew --prefix nvm)/nvm.sh
- echo 'source $(brew --prefix nvm)/nvm.sh' >> ~/.profile

#### install node

- nvm install [VERSION]

#### use specific node version

- nvm use [VERSION]

#### list all node version available

- nvm ls

#### brew services list

- brew services list

## Install postgreSql

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
