# passthrough-proxmox
#update grub
update-grub
#check
dmesg | grep -e DMAR -e IOMMU
#update modules
update-initramfs -u -k all
#check
dmesg | grep -i vfio
