# TA-Lib-whl-Files
TA-LIB Files

Source:
https://www.lfd.uci.edu/~gohlke/pythonlibs/

### Python whl TA-Lib 

precompiled whl files

---

TA_Lib-0.4.19-cp38-cp38-linux_armv7l

#### Tested on :
- Raspberry PI 3 B+
- Orange PI Zero
- Orange PI One


my step:
```
1: install ta-lib-0.4.0-src.tar.gz
./configure --prefix=/usr && make && sudo make install
2: install python3.8 from source
3: install numpy
3.1: pip3.8 install numpy
3.2: or install it from source ( recommended for device with low ram)
4: pip3.8 install wheel
5: git clone this ta-lib repo
6: create whl file from this source

    python3.8 setup.py bdist_wheel

7: install whl (in folder dist) to another device with pip3.8 install TA_Lib-0.4.19-cp38-cp38-linux_armv7l.whl
```

with this command i create wheel file

```
python3.8 -m pip wheel --wheel-dir=/tmp/wheelhouse numpy
python3.8 -m pip wheel --wheel-dir=/tmp/wheelhouse pandas
```

