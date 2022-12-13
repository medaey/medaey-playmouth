# medaey-playmouth

Is simple playmouth to custom boot screen

![penguen1](https://user-images.githubusercontent.com/16074153/207321631-f12f5067-d7b1-40cd-b7e3-da98e2e55b18.png)

# Install

- Dowload files
```bash
git clone https://github.com/medaey/medaey-playmouth.git
```
- Move folder to '/usr/share/plymouth/themes/medaey-logo'
```bash
sudo mv ./medaey-playmouth/medaey-logo/ /usr/share/plymouth/themes/medaey-logo/
```
- Add theme in plymouth
```bash
sudo update-alternatives --install /usr/share/plymouth/themes/default.plymouth default.plymouth /usr/share/plymouth/themes/medaey-logo/medaey-logo.plymouth 170
```
- Select the plymouth
```bash
sudo update-alternatives --config default.plymouth
```
- Update initramfs
```bash
sudo update-initramfs -u
```
