# PyControls
OS-agnostic modules to control the host machine

[//]: # (![Python]&#40;https://img.shields.io/badge/pypi_pynotification-passing-brightgreen&#41;)
[//]: # (![Python]&#40;https://img.shields.io/badge/pypi_volume_control-passing-brightgreen&#41;)

### Sub-Modules
- [volume-control](https://github.com/thevickypedia/volume-control)&nbsp;&nbsp;&nbsp;&nbsp;[![pypi-publish](https://github.com/thevickypedia/volume-control/actions/workflows/python-publish.yml/badge.svg)](https://github.com/thevickypedia/volume-control/actions/workflows/python-publish.yml)
- [pynotification](https://github.com/thevickypedia/pynotification)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[![pypi-publish](https://github.com/thevickypedia/pynotification/actions/workflows/python-publish.yml/badge.svg)](https://github.com/thevickypedia/pynotification/actions/workflows/python-publish.yml)

## Installation
```shell
python -m pip install pycontrols
```

## Usage
### Volume
```python
from pyvolume import pyvolume

pyvolume(level=30)
```
###### Optional arguments
- **debug:** Display logs in the form of `info`, `warnings` and `errors` messages.
- **logger:** Bring your own [`Logger`](https://docs.python.org/3/library/logging.html#logging.Logger) for custom logging.

### Notification
```python
from pynotification import pynotifier

pynotifier(title="Test Title", message="Test Message")
```
###### Optional arguments
- **icon:** Custom icon to be used for `Linux` and `Windows` operating systems.
  - Linux: Choose any [pre-defined icons](https://wiki.ubuntu.com/Artwork/BreatheIconSet/Icons) or a `.png` file as icon.
  - Windows: Choose any `.ico` file as icon. Defaults to [notification.ico](https://github.com/thevickypedia/pynotification/tree/main/pynotification/notification.ico)
- **destroy:** Boolean value to destroy the notification box on `Windows` operating system after notifying.
- **debug:** Display logs in the form of `info`, `warnings` and `errors` messages.
- **logger:** Bring your own [`Logger`](https://docs.python.org/3/library/logging.html#logging.Logger) for custom logging.

## License & copyright

&copy; Vignesh Rao

Licensed under the [MIT License](https://github.com/thevickypedia/pycontrols/blob/main/LICENSE)
