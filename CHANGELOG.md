2.1.1
- repos: Silence pycodestyle error (that broke docker image generation)

2.1
- Add support for S3 fetcher to docker image
- Lift Python minimal requirements to 3.5
- Fix reporting of of repo patch IDs
- config: use 'qemux86-64' instead of 'qemu' as default for KAS_MACHINE
- Ensure SSH key ends with newline
- kas-docker: Make it harder to run as root
- kas-docker: Make loop device passing optional
- kas-docker: Various fixes

2.0
- Add support for Yocto 3.0 / latest Isar
- Move docker image to Debian buster
- Add git-lfs support to docker image
- Add Yocto testimage dependencies to docker image

1.1
- Restore mercurial support
- Add -c and --cmd as aliases for --task
- Fix repo patching when using a branch name as refspec
- Update repo remote URL on kas file changes
- kas-docker: fix SHELL forwarding
- kas-docker: use released image, rather than "latest"
- kas-docker: allow to define custom image version
- kasproject/kas: enable devshell and menuconfig targets
- kasproject/kas image: add gnupg and quilt
- kasproject/kas-isar image: fix /var/tmp handling

1.0
- isar: Take qemu-user-static from buster and adjust binfmt setup

0.20.1
- kas-docker: Restore KAS_PREMIRRORS support

0.20.0
- kas-docker: enable passing SSH configs
- kas-docker: add --no-proxy-from-env option
- kas-docker: Pass in NO_PROXY
- Add KAS_PREMIRRORS support
- Remove SSH_AGENT_PID forwarding

0.19.0
- Recursive include handler refactoring and cleanups
- A lot of code cleanups, refactoring and bug fixings
- Isar docker support improvements

0.18.0
- Add patch support for repos
- Use git diff-index to check if repo is dirty
- docker: add debootstrap and qemu-user-static

0.17.0
- Add iproute and zx-utils to the docker image
- Fix relative path for repos
- Write MACHINE and DISTRO as weak defaults

0.16.0
- Support Mercurial repos
- Support Gentoo distro

0.15.0
- Environment variable passthrough
- Support major distro variants
- Add initial support for multiconfig

0.14.0
- Multi-target support
- Avoid downloading same repo twice

0.13.0
- Increase config file version

0.12.0
- Remove dynamic configuration support (Python config files)
- Shell command prepares complete bitbake configuration
- Add to define task in config and environment
- Improved error handling and reporting

0.11.0
- Allow in-tree repos not to be in a git repo
- Pass through git proxy related environment variables
- Write deterministic local.conf and bblayers.con
- Make configuration file versioning independent of project version
- Cleanups for uploading project to PyPI
- Print proper error message for config file format exception

0.10.0
- Docker image creation (Debian Stretch), pushed on kasproject/kas
- Restructure documentation add support for Sphinx export it to readthedocs
- Add support for include feature for Yaml files
- Add support for Isar build system
- Handling of SIGTERM/TERM improved
- Parallel download of git sources
- Allow environment to overwrite proxy, target, machine and distro
- Add unit testing for include/merge config file handling
- Rename sublayers back to layers
- pylint & pep8 cleanups
- Allow to define workdir via KAS_WORK_DIR
- Shell honors SHELL and TERM environment variable

0.9.0
- initial public release
