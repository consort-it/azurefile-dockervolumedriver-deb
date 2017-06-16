# azurefile-dockervolumedriver-deb

### About

This is a Ubuntu / Debian package of the Docker Volume Driver for Azure File Service over SMB/CIFS 🐳 [azurefile-dockervolumedriver](https://github.com/Azure/azurefile-dockervolumedriver).

### Version

Current version of the volume driver is: **v0.5.1 (2016-09-16)**

### Build

```bash
git clone https://github.com/consort-it/azurefile-dockervolumedriver-deb.git

dpkg-deb -b azurefile-dockervolumedriver-deb azurefile-dockervolumedriver-0.5.1.deb
```

### Push to repository

As we're using JFrog Artifactory, a push to a debian repository would look like:

```bash
curl -H 'X-JFrog-Art-Api: foo' -XPUT "https://foo.jfrog.io/boo/debian-packages-local/pool/azurefile-dockervolumedriver;deb.distribution=stable;deb.component=xenial;deb.architecture=amd64" -T azurefile-dockervolumedriver-0.5.1.deb
```
