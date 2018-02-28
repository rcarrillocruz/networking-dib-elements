======
packer
======

Build an image by using Packer.
Specify a qemu compatible image file on the host which is copied over
to the chroot and build the image by running Packer within the chroot.

Environment Variables
---------------------

DIB_PACKER_TEMPLATE_PATH
  :Required: Yes
  :Description: Path to Packer template
  :Example: ``DIB_PACKER_TEMPLATE_PATH=~/packer/vyos.json``
