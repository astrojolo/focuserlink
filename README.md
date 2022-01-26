# indi-focuserone
indi_focuserone INDI driver supports FocuserOne telescope focuser controller.

# Installing INDI server and libraries
To start you need to download and install INDI environment. See [INDI page](http://indilib.org/download.html) for details. 

Then FocuserOne INDI driver needs to be fetched and installed:

```
git clone https://github.com/astrojolo/focuserone.git
cd focuserone
mkdir build
cd build
cmake ..
make
make install
```

Then indiserver needs to be started with FocuserOne drivers:

```
indiserver -v indi_focuserone
```

Now FocuserOne can be used with any software that supports INDI drivers, like KStars with Ekos.
