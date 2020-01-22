=======
Windows
=======

Warning :This installation procedure is not fully tested, We strongly
recommand to install openalea.phenomenal with miniconda.

.. contents::

-----------------------
1. Install dependencies
-----------------------

.. code:: shell

    # Basic
    pip install numpy matplotlib scipy scikit-image

    # Download Scipy, OpenCv, VTK, ... wheels on http://www.lfd.uci.edu/~gohlke/pythonlibs/ and install it like this :
    pip install *.whl

    # Optional
    pip install ipython ipython[notebook] nose

    # OpenAlea.Deploy
    git clone https://github.com/openalea/deploy
    cd deploys; python setup.py install; cd ..

    # OpenAlea.Core
    git clone https://github.com/openalea/core
    cd core; python setup.py install; cd ..

------------------------------
2. Install openalea.phenomenal
------------------------------

.. code:: shell

    git clone https://gitlab.inria.fr/phenome/phenomenal.git
    cd phenomenal; python setup.py install; cd ..

------------------------------------------------------------------
3. Test if installation is well installed (with nosetests package)
------------------------------------------------------------------

.. code:: shell

    cd phenomenal
    nosetests test
