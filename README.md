![Sphere Orb Logo](./img/header.png)

# Sphere Orb [![CircleCI Build Status](https://circleci.com/gh/hubci/sphere-orb.svg?style=shield "CircleCI Build Status")](https://app.circleci.com/ppelines/github/hubci/sphere-orb) [![CircleCI Orb Version](https://badges.circleci.com/orbs/hubci/sphere.svg)][reg-page] [![GitHub License](https://img.shields.io/badge/license-MIT-lightgrey.svg)](https://raw.githubusercontent.com/hubci/sphere-orb/trunk/LICENSE)


An orb to make it easy to detect which operating system (OS) and version your orb and/or CircleCI config is running on.

*Notes: This orb is the spiritual successor to the deprecated [OS Detect orb](https://github.com/CircleCI-Archived/os-detect-orb) by CircleCI.*

CircleCI Support

| Executor/OS    | Supported? | Shell |
|---             |---         |---    |
| Docker/Ubuntu  | yes        | Bash  |
| Docker/Debian  | yes        | Bash  |
| Docker/Alpine  | yes        | Bash  |
| macOS          | yes        | Bash  |
| machine/Ubuntu | yes        | Bash  |


## Usage

Example use as well as a list of available executors, commands, and jobs are available on this orb's [registry page][reg-page].

| Variables     | Description |
|---            |---          |
| $OSD_FAMILY   | The OS family. For example, linux or darwin
| $OSD_ID       | The OS slug name. For example, ubuntu, alpine or macos.
| $OSD_VERSION  | The OS version number, as advertised. For example, 18.04 for Ubuntu or 10.9 for macOS.
| $SUDO         | Contains the string "sudo" when the current user is not root and the `sudo` binary is available. Prefix this with your commands.


## Compatibility

Version 1 of this orb (as well as the v0 releases) will maintain compatibility with the original OS Detect orb.
For people transitioning from the old orb to this one, this will make that process easier.

When v2 lands later in 2023, it will be a breaking change that moves this orb to a more advanced and useful future.


## Resources

[CircleCI Orb Registry Page][reg-page] - The official registry page for this orb will include all versions, executors, commands, and have described the jobs.  
[CircleCI Orb Docs](https://circleci.com/docs/2.0/orb-intro/#section=configuration) - Docs for using and creating CircleCI Orbs.  


## Contributing
I welcome [issues](https://github.com/hubci/sphere-orb/issues) to and [pull requests](https://github.com/hubci/sphere-orb/pulls) against this repository!
For further questions/comments about this or other orbs, visit the Orb Category of [CircleCI Discuss](https://discuss.circleci.com/c/orbs).

### Publishing
New versions of this orb are published by pushing a SemVer git tag by [Ricardo N Feliciano](https://github.com/FelicianoTech).

## License
This project is licensed under the MIT License - read [LICENSE](LICENSE) file for details.



[reg-page]: https://circleci.com/developer/orbs/orb/hubci/sphere
