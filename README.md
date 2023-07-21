# Roland Digital DXY-1100

https://www.python.org/download/releases/2.6/
http://sites.music.columbia.edu/cmc/chiplotle/manual/install.html
https://pypi.org/project/Chiplotle/

https://pip.pypa.io/en/latest/installation/#


https://www.youtube.com/watch?v=6_pwzqPk6Gg


alternative

https://www.youtube.com/watch?v=nx7SYgibg20



## Chiplotle for python 3

My setup 
Laptop: `Windows 11` `Roland Digital DXY-1100` `USB to SERIAL`</br>
Use windows `Command Prompt` for all command line installation.

> The whole process is based on the instructions from here, with minor adjustments</br>
> [github.com/cyprienh/chiplotle3](https://github.com/cyprienh/chiplotle3/tree/main)

1. Install curent version of Python 3.x.
2. Chceck if Python is added to System `PATH` in Environment Variable</br>
    `Win` + `R` type: `cmd` and press `OK`</br>
    in `cmd.exe` terminal type ```python --version```</br>
    the version displayed should match installed version.

>   Add manulay python to system PATH on Windows:
>   1. `Win` + `R` and type `sysdm.cpl`
>   2. `Advanced` Tab `Environment Variables`
>   3. chceck if is added to `PATH` 
>   4. if not `Add` path to pathon istalation directroy</br>
>   *example* - `C:\Users\"your user"\AppData\Local\Programs\Python\Python3xx`

3. Python package manager `pip`</br>
    Chceck if you have `pip` in yours system, in `cmd.exe` type `pip --version`, if not install `pip`.
    
> Install pip on Windows:</br>
> Open `Command Prompt` terminal and type *(line by line)*: 
> ```
> curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py
> python get-pip.py
> ```
 4. Install Chiplotle Dependences


    ```
    pip install numpy
    pip install pyserial
    ```

5. Install `setuptools`
6. Install `chiplotle`
    * Download `Chiplotle-0.4.1.tar.gz` file from this [webside](https://pypi.org/project/Chiplotle/#files) 
    * unpack `tar -xzvf Chiplotle-0.4.1.tar.gz` 
    * inside `Chiplotle-0.4.1` directory find and open `setup.py` file in text editor.
    * if you success in step `5` and install `setuptools`, remove or coment out line 4 and 5 of `setup.py` file.
    ```python
    3 ...
    4 # from ez_setup import use_setuptools
    5 # use_setuptools( ) # <-- this must come before setup import
    6 ...
    ```
    * save `setup.py` file and in `cmd` run this command `setup.py install`

7. Add `Chiplotle` do system `PATH`


chiplotle/scritps directory is in your PATH 

setuptools
`https://www.geeksforgeeks.org/how-to-set-up-setuptools-for-python-on-windows/`
