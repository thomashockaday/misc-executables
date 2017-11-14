# Misc Executables
#### A small collection of time-saving shell scripts

## How to Use
- Download the repository.
- Create a config file by copying the `config.example` file and removing ".example"
- Edit the `config` file, setting `WORKDIR` to the location of the folder where you downloaded the repo to, and `LOCATION` to your city.
- Create a copy of all of the executable files in `/usr/local/sbin`. You can do this quickly by dragging the `importexecs` file into a Terminal window.
- Add `export PATH="/usr/local/sbin:$PATH"` to the bottom of `~/.zshrc`.
- That's it!

---

Below is a breakdown of each script. They should be ran from the root folder of a repository.

| File | Description | Usage Case |
| --- | --- | --- |
| __config__ | Variable storage. Running this won't do anything. | none |
| __importexecs__ | Transfers repo files into `/usr/local/sbin` | `$ importexecs` |
| __setup__ | Quickly setup and launch a development environment using either Docker or Vagrant as a parameter. Optional parameter includes dependency installation and .env file creation. | `$ setup [docker/vagrant] [initial?]` |
| __docssh__ | Enter a running Docker web container | `$ docssh` |
| __mysqlport__ | Print the port number of the running mysql Docker container | `$ mysqlport` |
| __brewm__ | Update Homebrew as well as any installed formulae, then check for errors | `$ brewm` |
| __weather__ | Show the weather forecast for your configured location | `$ weather` |

---

## Contributing to the Repo
- Make changes to the files in your local repo.
- Run `$ importexecs` to transfer all of the files to `/usr/local/sbin`.
- Test.
- Commit and push.
