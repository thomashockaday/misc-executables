# Misc Executables
#### A small collection of time-saving shell scripts

## How to Use
- Download the repository.
- Edit the `config` file, setting `WORKDIR` to the location of the folder where you downloaded the repo to.
- Create a copy of all of the files in `/usr/local/sbin`.
- That's it!

---

Below is a breakdown of each script. They should be ran from the root folder of a repository.

| File | Description | Usage Case |
| --- | --- | --- |
| __config__ | Variable storage. Running this won't do anything. | none |
| __importexecs__ | Transfers repo files into `/usr/local/sbin` | `$ importexecs` |
| __dockap__ | Deploy a site using a Capistrano Docker container | `$ dockap [staging/production] deploy` |
| __setup__ | Quickly setup and launch a development environment using either Docker or Vagrant as a parameter. Optional parameter includes dependency installation and .env file creation. | `$ setup [docker/vagrant] [initial?]` |
| __docssh__ | Enter a running Docker web container | `$ docssh` |
| __mysqlport__ | Print the port number of the running mysql Docker container | `$ mysqlport` |
| __give-em-one-of-these__ | For when some gangsta starts dissin' yo fly girl | `$ give-em-one-of-these` |

---

## Contributing to the Repo
- Make changes to the files in your local repo.
- Run `$ importexecs` to transfer all of the files to `/usr/local/sbin`.
- Test.
- Commit and push.
