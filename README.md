# windows-autounattended
Windows Server setup with Windows unattended install.

## autounattend.xml

I used the Windows System Image Manager to create an unattended Windows Setup answer file.

I also used Windows Setup reference that describes all of the unattended settings that can be set in Windows Server 2016. Link below for references.

https://docs.microsoft.com/en-us/windows-hardware/customize/desktop/unattend/components-b-unattend

It was a lengthy process based on trial and error.

## Add autounattend.xml to ISO

Use ImgBurn to create an ISO file from a directory. Navigate to "Advanced > Bootable Disk" and tick the box to "Make Image Bootable".

Set "Source" as `C:\SRC\`. Set "Destination" as `C:\OUTPUT\win2k16_autounattend.iso`.

Use `boot\etfsboot.com` file from the DVD for "Boot Image".

Set "Sectors To Load" to 8 when setting up a Windows Server 2016.
