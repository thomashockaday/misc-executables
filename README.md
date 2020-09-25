# Misc Executables

#### A small collection of time-saving shell scripts

## How to Use
- Download the repository.
- Create a config file by copying the `config.example` file and removing ".example"
- Edit the `config` file, setting `WORKDIR` to the location of the folder where you downloaded the repo to.
- Create a copy of all of the executable files in `/usr/local/sbin`. You can do this quickly by dragging the `importexecs` file into a Terminal window.
- Add `export PATH="/usr/local/sbin:$PATH"` to the bottom of your profile. You can do this quickly by running `$ echo export PATH="/usr/local/sbin:$PATH" >> ~/.zshrc` (or relevant profile).
- That's it!

---

Below is a breakdown of each script. They should be ran from the root folder of a repository.

| File | Description | Usage Case |
| --- | --- | --- |
| __awslogin__ | Generates a 12 hour login token for Amazon Elastic Container Registry | `$ awslogin` |
| __brewm__ | Update Homebrew as well as any installed formulae, then check for errors | `$ brewm` |
| __config__ | Variable storage. Running this won't do anything. | none |
| __dclean__ | Remove all "dangling" docker images | `$ dclean` |
| __dockill__ | Removes all exited Docker containers | `$ dockill` |
| __importexecs__ | Transfers repo files into `/usr/local/sbin` | `$ importexecs` |

---

## Contributing to the Repo
- Make changes to the files in your local repo.
- Run `$ importexecs` to transfer all of the files to `/usr/local/sbin`.
- Test.
- Commit and push.
