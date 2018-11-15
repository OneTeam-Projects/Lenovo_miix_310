# Lenovo Ideapad Miix 310 10ICR
A set of fixes for Lenovo MIIX 310 Tablet/Laptop to be able to run current
build of ElementaryOS Juno (2018) and another Ubuntu based distros:
1. Fix for orientation of the display (iio-sensor-proxy udev config)
2. Fix for proper order of kernel modules load (pwm_lpss before i915)
3. Fix for early boot framebuffer rotation to landscape (grub)
4. Fix for Bluetooth (soon)
5. Fix for Webcam (soon)

# For install:
Soon.......

## Workaround for the backlight at earlier boot in Ubuntu liveCD installer.
At the boot time when grub just started and shows the menu press e
to enable editing. Update linux kernel like with: acpi_backlight=vender
in this case Linux will keep the state of backlight and will not reset
the backlight to 0, you shall be also able to change backlight with HW
keys.
