Step by step install python-env

1.  env python master can be downloaded on the [[web python]](https://pypi.python.org/pypi/virtualenv#downloads)
2.  If you use Ubuntu operating system, check the Download folder, and then extract the files <b>virtualenv-15.0.1.tar.gz</b>
3.  run a terminal in ubuntu, run a terminal in ubuntu, go to the directory <b>virtualenv-15.0</b> , then check the directory if there is an <b> setup.py </b>
    <pre>
    bertopeng17@bertopeng17-ThinkPad-T520:~/Downloads$ <b>cd virtualenv-15.0.1/</b>
    </pre>

    <pre>
    bertopeng17@bertopeng17-ThinkPad-T520:~/Downloads/virtualenv-15.0.1$ <b>ls</b>
    AUTHORS.txt  LICENSE.txt  README.rst  <b>setup.py</b>             virtualenv_embedded
    bin          MANIFEST.in  scripts     tests                virtualenv.py
    docs         PKG-INFO     setup.cfg   virtualenv.egg-info  virtualenv_support

    </pre>
4.  then, for the installation run the command:
    <pre>
    bertopeng17@bertopeng17-ThinkPad-T520:~/Downloads/virtualenv-15.0.1$ <b>sudo python setup.py install</b>
    [sudo] password for bertopeng17: <b>*********</b>
    running install
    running bdist_egg
    running egg_info
    writing virtualenv.egg-info/PKG-INFO
    writing top-level names to virtualenv.egg-info/top_level.txt
    writing dependency_links to virtualenv.egg-info/dependency_links.txt
    writing entry points to virtualenv.egg-info/entry_points.txt
    reading manifest file 'virtualenv.egg-info/SOURCES.txt'
    reading manifest template 'MANIFEST.in'
    warning: no previously-included files matching '*' found under directory 'docs/_templates'
    warning: no previously-included files matching '*' found under directory 'docs/_build'
    writing manifest file 'virtualenv.egg-info/SOURCES.txt'
    installing library code to build/bdist.linux-i686/egg
    running install_lib
    running build_py
    creating build
    creating build/lib.linux-i686-2.7
    copying virtualenv.py -> build/lib.linux-i686-2.7
    creating build/lib.linux-i686-2.7/virtualenv_support
    copying virtualenv_support/__init__.py -> build/lib.linux-i686-2.7/virtualenv_support
    copying virtualenv_support/pip-8.1.1-py2.py3-none-any.whl -> build/lib.linux-i686-2.7/virtualenv_support
    copying virtualenv_support/wheel-0.29.0-py2.py3-none-any.whl -> build/lib.linux-i686-2.7/virtualenv_support
    copying virtualenv_support/setuptools-20.3-py2.py3-none-any.whl -> build/lib.linux-i686-2.7/virtualenv_support
    copying virtualenv_support/argparse-1.4.0-py2.py3-none-any.whl -> build/lib.linux-i686-2.7/virtualenv_support
    creating build/bdist.linux-i686
    creating build/bdist.linux-i686/egg
    creating build/bdist.linux-i686/egg/virtualenv_support
    copying build/lib.linux-i686-2.7/virtualenv_support/pip-8.1.1-py2.py3-none-any.whl -> build/bdist.linux-i686/egg/virtualenv_support
    copying build/lib.linux-i686-2.7/virtualenv_support/wheel-0.29.0-py2.py3-none-any.whl -> build/bdist.linux-i686/egg/virtualenv_support
    copying build/lib.linux-i686-2.7/virtualenv_support/__init__.py -> build/bdist.linux-i686/egg/virtualenv_support
    copying build/lib.linux-i686-2.7/virtualenv_support/setuptools-20.3-py2.py3-none-any.whl -> build/bdist.linux-i686/egg/virtualenv_support
    copying build/lib.linux-i686-2.7/virtualenv_support/argparse-1.4.0-py2.py3-none-any.whl -> build/bdist.linux-i686/egg/virtualenv_support
    copying build/lib.linux-i686-2.7/virtualenv.py -> build/bdist.linux-i686/egg
    byte-compiling build/bdist.linux-i686/egg/virtualenv_support/__init__.py to __init__.pyc
    byte-compiling build/bdist.linux-i686/egg/virtualenv.py to virtualenv.pyc
    creating build/bdist.linux-i686/egg/EGG-INFO
    copying virtualenv.egg-info/PKG-INFO -> build/bdist.linux-i686/egg/EGG-INFO
    copying virtualenv.egg-info/SOURCES.txt -> build/bdist.linux-i686/egg/EGG-INFO
    copying virtualenv.egg-info/dependency_links.txt -> build/bdist.linux-i686/egg/EGG-INFO
    copying virtualenv.egg-info/entry_points.txt -> build/bdist.linux-i686/egg/EGG-INFO
    copying virtualenv.egg-info/not-zip-safe -> build/bdist.linux-i686/egg/EGG-INFO
    copying virtualenv.egg-info/top_level.txt -> build/bdist.linux-i686/egg/EGG-INFO
    creating dist
    creating 'dist/virtualenv-15.0.1-py2.7.egg' and adding 'build/bdist.linux-i686/egg' to it
    removing 'build/bdist.linux-i686/egg' (and everything under it)
    Processing virtualenv-15.0.1-py2.7.egg
    creating /usr/local/lib/python2.7/dist-packages/virtualenv-15.0.1-py2.7.egg
    Extracting virtualenv-15.0.1-py2.7.egg to /usr/local/lib/python2.7/dist-packages
    Adding virtualenv 15.0.1 to easy-install.pth file
    Installing virtualenv script to /usr/local/bin
    
    Installed /usr/local/lib/python2.7/dist-packages/virtualenv-15.0.1-py2.7.egg
    Processing dependencies for virtualenv==15.0.1
    Finished processing dependencies for virtualenv==15.0.1
    bertopeng17@bertopeng17-ThinkPad-T520:~/Downloads/virtualenv-15.0.1$ ls
    </pre>
    
    ![alt img](https://github.com/syaifulahdan/MCWT/blob/master/Python-virtualenv/image/Screenshot%20from%202016-04-16%2002:30:59.png)    
5.  
