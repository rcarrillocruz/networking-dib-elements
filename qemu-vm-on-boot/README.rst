===============
qemu-vm-on-boot
===============

Specify a qemu compatible image file on the host which is copied over
to the image and is started on boot with qemu via a systemd script.

Environment Variables
---------------------

DIB_QEMU_VM_IMAGE_PATH
  :Required: Yes
  :Description: Path to qemu image file on the build host which is copied
    under /var/lib/qemu/images on the built image
  :Example: ``DIB_QEMU_VM_IMAGE_PATH=~/images/vyos.qcow2`` will copy
    vyos.qcow2 from the host to path /var/lib/qemu/images on the image.
