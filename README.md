# indi-focuserlink
indi_focuserlink INDI driver supports FocuserLInk telescope focuser motor.

# Installing INDI server and libraries
To start you need to download and install INDI environment. See [INDI page](http://indilib.org/download.html) for details. 

Then FocuserLink INDI driver needs to be fetched and installed:

```
git clone https://github.com/astrojolo/focuserlink.git
cd focuserlink
mkdir build
cd build
cmake -DCMAKE_INSTALL_PREFIX=/usr ..
make
sudo make install
```

Then indiserver needs to be started with FocuserLink drivers:

```
indiserver -v indi_focuserlink
```

Now FocuserLink can be used with any software that supports INDI drivers, like KStars with Ekos.
