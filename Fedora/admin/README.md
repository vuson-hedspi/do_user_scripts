# Admin Scripts

## swap.sh
This script will create and activate a swap file at /swapfile on your new droplet, there are two different modes, automatic mode based on RedHat Enterprise Linux Storage Guide (https://goo.gl/kFGdnO) and manual mode, using the size you specify.  An entry in /etc/fstab will also be made to automatically enable the swap file on boot.

**Required input**:
* `<%MODE%>` - Possible values will be "automatic" or "manual"

**Optional input**:
if <%MODE%> is set to "manual" then <%SWAP_FILE_SIZE%> where represents the size of the swap file to create. E.g. "1G"

### Tested on
* Fedora 22
* Fedora 23
