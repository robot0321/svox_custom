# SVOX custom: customize the rendering method following NeRF and NeuS

Folked from the repository <https://github.com/sxyu/svox>

* I customize the `trace_ray` function in `svox/csrc/rt_kernel.cu` file.
https://github.com/robot0321/svox_custom/blob/4d923d506dd3e54085136964888513e7b28463fe/svox/csrc/rt_kernel.cu#L222-L321

* This code is not complete since I only fixed the forward function (**only for customized rendering, not training**)

* Whenever you change the library code, do uninstall and re-install. (There is dev-mode but I did not use it)

* `svox/csrc/rt_kernel_neus.cu` is for NeuS and `svox/csrc/rt_kernel.cu` is for NeRF

* Note that the file named `svox/csrc/rt_kernel.cu` is used in this library. If you want to change, swap the name of files.

### Install
~~~sh
python setup.py install
~~~

### Uninstall
~~~sh
pip uninstall svox
~~~

### Documentation
Please see <https://svox.readthedocs.io>
