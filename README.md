# Flannel example configurations

# Intro

- Flannel is a virtual network that gives a subnet to each host for use with container runtimes.
- For more information on flannel, see [Flannel Github](https://github.com/coreos/flannel)

# Usage

- Ensure you have an etcd cluster running and the etcdctl tool installed.
- Create a flannel JSON file in a local directory and run:
```bash
$ etcdctl set coreos.com/network/config < flannel-config.json
```
- Check the etcd key using
```bash
$ etcdctl get coreos.com/network/config
```

### Contributing
File issues in GitHub to report bugs or issue a pull request to contribute.
