======
packer
======

Build an image by using Packer.

This elements copies over Packer template specified by DIB_PACKER_TEMPLATE_PATH
environment variable to the chroot, then installs Packer and kicks off a Packer qemu only build.

Image built by Packer is dropped outside the chroot as image.qcow2.

Packer template should not have ``output_directory`` defined, as it expects to find the built
image file under ``output-qemu``. Also, ``headless`` should be set to True, to allow remote
builds.


Environment Variables
---------------------

DIB_PACKER_TEMPLATE_PATH
  :Required: Yes
  :Description: Path to Packer template
  :Example: ``DIB_PACKER_TEMPLATE_PATH=~/packer/vyos.json``
