======
packer
======

Build an image by using Packer.

This elements copies over Packer template specified by DIB_PACKER_TEMPLATE_PATH
environmt variable to the chroot, then installs Packer and kicks off a Packer qemu only build.

Image built by Packer is dropped outside the chroot as image.qcow2.

Environment Variables
---------------------

DIB_PACKER_TEMPLATE_PATH
  :Required: Yes
  :Description: Path to Packer template
  :Example: ``DIB_PACKER_TEMPLATE_PATH=~/packer/vyos.json``
