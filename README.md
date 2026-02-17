# Bio

I'm **Terje Kvernes**, a systems administrator, software developer, generalized hacker, and writer. I work with Linux (mostly RHEL and Fedora), MacOS, NetApp, Cisco, APC infrastructure and a lot of other hardware. I used to work a lot with audio-visual equipment (mostly Crestron based), but less recently. I also do company-wide Zoom management.

My toolchest at work includes stuff like:

- Rust
- Python
- Ansible
- CFEngine
- Fleet/OSquery
- terraform (and a bit of Packer, targeting AWS, Azure, and OpenStack)
- perl (not as much as I used to, thankfully)
- shell scripting (bash, zsh)
- monitoring through Zabbix/Grafana/Prometheus (and Nagios for some reason)
- and whatever else the job throws at me... I also have done work in Go, C, Fortran...

In my spare time I hike, write fiction, and get fascinated by new and novel ideas.

## Projects

### Work-adjacent projects

- [mreg](https://github.com/unioslo/mreg), [mreg-cli](https://github.com/unioslo/mreg-cli) and [mreg-api](https://github.com/unioslo/mreg-api): A DNS management system, its command line interface, and its Python API. Written in Python, specifically for the University of Oslo, but with some promise of being useful to others.
- [Treetop](https://github.com/terjekv/treetop-core): A high performance policy engine for authorization requests, built on [Cedar](https://www.cedarpolicy.com/en).
  - The core engine above is exposed via a [REST server](https://github.com/terjekv/treetop-rest) with its own CLI.
  - A [python client library](https://github.com/terjekv/treetop-client-python) is also available.
- [EESSI](https://github.com/EESSI/): European Environment for Scientific Software Installations (sadly, not as active as I'd like to be)
  - I mostly dealt with monitoring for the project. The page generator was originally written in Python but migrated to [Rust](https://github.com/EESSI/cvmfs-status-page-rust). Apart from the HTML output this generator also
  produces a [Prometheus](https://prometheus.io) metrics endpoint and JSON output for use in other contexts. The page is available at [status.eessi.io](http://status.eessi.io).
  - This side project also led to a multithreaded type safe [Rust CVMFS scraper](https://github.com/EESSI/cvmfs-server-scraper-rust)
- [EasyBuild](https://easybuild.io): A software build and installation framework, mostly used in HPC environments. I've contributed EasyConfigs and some other components. Again something I wish I had more time for.

### Personal projects

- [hubuum](https://github.com/hubuum/hubuum): A non-opinionated CMDB.
  - This may become more than slightly work adjacent, but right now it's a personal project.
- [Callgrind GitHub Action](https://github.com/terjekv/github-action-iai-callgrind): A GitHub Action for running Callgrind tests for Rust code on pull requests, showing improvements and regressions per test as a PR comment.
Tracks performance against the main branch and between individual commits in the PR itself. It also benchmarks for all features. A few examples: [1](https://github.com/terjekv/treetop-rest/pull/5#issuecomment-3865129482), [2](https://github.com/terjekv/treetop-core/pull/7#issuecomment-3856867140) (the latter used an old version of the action and did not track across commits).

### Other projects

- [github-authorized-keys](https://github.com/terjekv/github-authorized-keys): Using teams on github to manage ssh authorized keys.

### Other stuff

#### Talks and presentations

- ARM HPC Users group 2020: [EasyBuild on ARM](https://www.youtube.com/watch?v=HyR-STGRnfM). Experiences in running EasyBuild on ARM, going through some of the issues with porting software reliant on SSE intrinsics and how to get around such issues.
