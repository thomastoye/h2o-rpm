H2O COPR
========

[COPR project](https://copr.fedorainfracloud.org/coprs/snthaoeu/h2o)

Based on [`tatsushid`'s work](https://github.com/tatsushid/h2o-rpm)

This repository is used to build [H2O](https://h2o.examp1e.net/) RPM's for CentOS trough [COPR](https://copr.fedorainfracloud.org/).

If you're looking for a Debian package, please see [h2o-deb](https://github.com/tatsushid/h2o-deb)

## Installation

### Quick enable

If you have `yum-plugin-copr`:

```
$ dnf enable snthaoeu/h2o
$ yum -y install h2o
```

### Manually adding the repository

Add the relevant repository from [here](https://copr.fedorainfracloud.org/coprs/snthaoeu/h2o) to `/etc/yum.repos.d` then install with `yum -y install h2o`.

## Usage

Once the installation finishes successfully, you can see a configuration file
at `/etc/h2o/h2o.conf`.

To start h2o, please run

```bash
service h2o start
```

or

```bash
systemctl enable h2o.service
systemctl start h2o.service
```

## License

This is under MIT License. Please see the
[LICENSE](https://github.com/tatsushid/h2o-rpm/blob/master/LICENSE) file for
details.
