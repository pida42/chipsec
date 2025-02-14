# Build

_(as root)_

```
apt-get install build-essential python-dev python gcc linux-headers-$(uname -r) nasm
git clone https://github.com/chipsec/chipsec.git
pip install setuptools
cd chipsec/
python setup.py build_ext -i
```

Result in `du -h chipsec/helper/linux/chipsec.ko`.

Build tested on:

```
# uname -a
Linux preissler-mint 5.4.0-91-generic #102-Ubuntu SMP Fri Nov 5 16:31:28 UTC 2021 x86_64 x86_64 x86_64 GNU/Linux

# cat /etc/lsb-release 
DISTRIB_ID=LinuxMint
DISTRIB_RELEASE=20.2
DISTRIB_CODENAME=uma
DISTRIB_DESCRIPTION="Linux Mint 20.2 Uma"
```

---

CHIPSEC: Platform Security Assessment Framework
===============================================

[![Build Status](https://travis-ci.org/chipsec/chipsec.svg?branch=master)](https://travis-ci.org/chipsec/chipsec)

CHIPSEC is a framework for analyzing the security of PC platforms including hardware, system firmware (BIOS/UEFI), and platform components. It includes a security test suite, tools for accessing various low level interfaces, and forensic capabilities. It can be run on Windows, Linux, Mac OS X and UEFI shell. Instructions for installing and using CHIPSEC can be found in the [manual](chipsec-manual.pdf).

NOTE: This software is for security testing purposes. Use at your own risk. Read [WARNING.txt](chipsec/WARNING.txt) before using.

First version of CHIPSEC was released in March 2014:
[Announcement at CanSecWest 2014](https://cansecwest.com/slides/2014/Platform%20Firmware%20Security%20Assessment%20wCHIPSEC-csw14-final.pdf)

Recent presentation on how to use CHIPSEC to find vulnerabilities in firmware, hypervisors and hardware configuration, explore low level system assets and even detect firmware implants:
[Exploring Your System Deeper](https://www.slideshare.net/CanSecWest/csw2017-bazhaniuk-exploringyoursystemdeeperupdated)

Release Convention
------------------

  * CHIPSEC uses a major.minor.patch release version number
  * Changes to the arguments or calling conventions will be held for a minor version update


Projects That Include CHIPSEC
-----------------------------

 * [Linux UEFI Validation (LUV)](https://01.org/linux-uefi-validation)
 
 * [ArchStrike](https://archstrike.org)
 
 * [BlackArch Linux](https://www.blackarch.org/index.html)

Contact Us
----------

For any questions or suggestions please contact us at: chipsec@intel.com

Mailing lists:

 * CHIPSEC users: [chipsec-users](https://groups.google.com/forum/#!forum/chipsec-users)
 * [CHIPSEC discussion list on 01.org](https://lists.01.org/hyperkitty/list/chipsec@lists.01.org/)

Twitter:

 * For CHIPSEC release alerts: Follow us at [CHIPSEC Release](https://twitter.com/ChipsecR)
 * For general CHIPSEC info: Follow [CHIPSEC](https://twitter.com/Chipsec)

For AMD related questions or suggestions please contact Gabriel Kerneis at: Gabriel.Kerneis@ssi.gouv.fr