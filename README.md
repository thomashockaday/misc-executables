# Misc Executables
#### A small collection of time-saving shell scripts

## How to Use
- Download the repository.
- Edit the `config` file, setting `WORKDIR` to the location of the folder where you downloaded the repo to.
- Create a copy of all of the files in `/usr/local/sbin`.
- That's it!

---

Below is a breakdown of each script. They should be ran from the root folder of a repository.

| File                      | Description                                        | Usage Case                           |
| ------------------------- | -------------------------------------------------- | ------------------------------------ |
| #### config               | Variable storage. Running this won't do anything.  | none                                 |
| #### importexecs          | Transfers repo files into `/usr/local/sbin`        | $ importexecs                        |
| #### dockap               | Deploy a site using a Capistrano Docker container  | $ dockap [staging/production] deploy |
| #### setup                | Quickly setup and launch a development environment | $ setup [docker/vagrant] [initial?]  |
| #### docssh               | Enter a running Docker container                   | $ docssh                             |
| #### mysqlport            | Print the port of the mysql Docker container       | $ mysqlport                          |
| #### give-em-one-of-these | For when some gangsta starts dissin' yo fly girl   | $ give-em-one-of-these               |

---

## Contributing to the Repo
- Make changes to the files in your local repo.
- Run `$ importexecs` to transfer all of the files to `/usr/local/sbin`.
- Test.
- Commit and push.
