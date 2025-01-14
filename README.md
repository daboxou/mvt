<p align="center">
     <img src="./docs/mvt.png" width="300" />
</p>

# Mobile Verification Toolkit

[![](https://img.shields.io/pypi/v/mvt)](https://pypi.org/project/mvt/)

Mobile Verification Toolkit (MVT) is a collection of utilities to simplify and automate the process of gathering forensic traces helpful to identify a potential compromise of Android and iOS devices.

[Please check out the documentation.](https://mvt.readthedocs.io/en/latest/)

## Installation

First you need to install dependencies, on Linux `sudo apt install python3 python3-pip libusb-1.0-0` or on MacOS `brew install python3 libusb`.

Then you can install mvt from pypi with `pip install mvt`, or directly form sources:
```bash
git clone https://github.com/mvt-project/mvt.git
cd mvt
pip3 install .
```

## Usage

MVT provides two commands `mvt-ios` and `mvt-android` with the following subcommands available:

* `mvt-ios`:
    * `check-backup`: Extract artifacts from an iTunes backup
    * `check-fs`: Extract artifacts from a full filesystem dump
    * `check-iocs`: Compare stored JSON results to provided indicators
    * `decrypt-backup`:  Decrypt an encrypted iTunes backup
* `mvt-android`:
    * `check-backup`: Check an Android Backup
    * `download-apks`: Download all or non-safelisted installed APKs

Check out [the documentation to see how to use them](https://mvt.readthedocs.io/en/latest/).

## License

The purpose of MVT is to facilitate the ***consensual forensic analysis*** of devices of those who might be targets of sophisticated mobile spyware attacks, especially members of civil society and marginalized communities. We do not want MVT to enable privacy violations of non-consenting individuals. Therefore, the goal of this license is to prohibit the use of MVT (and any other software licensed the same) for the purpose of *adversarial forensics*.

In order to achieve this, MVT is released under an adaptation of [Mozilla Public License v2.0](https://www.mozilla.org/MPL). This modified license includes a new clause 3.0, "Consensual Use Restriction" which permits the use of the licensed software (and any *"Larger Work"* derived from it) exclusively with the explicit consent of the person/s whose data is being extracted and/or analysed (*"Data Owner"*).

[Read the LICENSE](https://github.com/mvt-project/mvt/blob/main/LICENSE)
