Oci_cloud_init_script
=====================

Install lxd to test cloud-init
------------------------------

- https://cloudinit.readthedocs.io/en/latest/topics/tutorial.html#

lxc launch ubuntu:focal my-test --config=user.user-data="$(cat ./easy-one.cfg)"
lxc shell my-test
lxc stop my-test
lxc rm my-test

cloud-init status --wait
cloud-init query userdata
cloud-init schema --system --annotate

