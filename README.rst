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

* Set proper values for `inverter_ip` and `broker_address` in ``kostal-modbusquery.py``.
* Set proper `WorkingDirectory` in ``kostal-modbusquery.service``.


Run as a service
----------------

* Create symlink::

    sudo ln -s <path-to-working-directory>/kostal-modbusquery.service /lib/systemd/system/kostal-modbusquery.service

* Restart service daemon::

    sudo systemctl daemon-reload

* Enable and start service::

    sudo systemctl enable kostal-modbusquery.service
    sudo systemctl start kostal-modbusquery.service


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
