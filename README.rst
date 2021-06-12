kostal-modbusquery
==========



Introduction
------------

This library provides a pure Python interface to access Kostal Inverters via the Modbus Protocol and specification provided here:

https://www.kostal-solar-electric.com/de-de/download/-/media/document-library-folder---kse/2018/08/30/08/53/ba_kostal_interface_modbus-tcp_sunspec.pdf

It has been tested  with Python version 3.5, 3.6, 3.7 and 3.8.


Features
~~~~~~~~

* Provide Class that  reads documented  Registers
* Provide some sample calculations mimic´ing the Inverter´s home page output


Tested with 
~~~~~~~~~~~~~~~~

* Kostal Plenticore Plus 10 with connected BYD 6.4
* Kostal Plenticore Plus 8.5




Installation
------------
Clone / Download repo and use kostal-modbusquery.py 


Getting started
---------------

To use ``kostal-modbusquery`` in a project take a look at the __main__ section in kostal-modbusquery.py how to include it in your environment

Put the `kostal-modbusquery.service` in `/lib/systemd/system/`.

Reload the daemon:

```
sudo systemctl daemon-reload
```

Now enable the service to start on system boot, also start the service using the following commands.

```
sudo systemctl enable dummy.service
sudo systemctl start dummy.service
```

Disclaimer
----------

.. Warning::

   Please note that any incorrect or careless usage of this module as well as
   errors in the implementation may harm your Inverter !

   Therefore, the author does not provide any guarantee or warranty concerning
   to correctness, functionality or performance and does not accept any liability
   for damage caused by this module, examples or mentioned information.

   **Thus, use it on your own risk!**


License
-------

Distributed under the terms of the `GNU General Public License v3 <https://www.gnu.org/licenses/gpl-3.0.en.html>`_.
