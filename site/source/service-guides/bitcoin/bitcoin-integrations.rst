.. _bitcoin-integrations:

====================
Bitcoin Integrations
====================

.. contents::
  :depth: 2
  :local:

Here you will find guides on how to connect different kinds of Bitcoin wallets (hardware and software) to your server's node, to complete your sovereign Bitcoin stack!

.. _bitbox-app:

BitBoxApp
---------

**Available For**

 - Android
 - Linux
 - macOS
 - Windows
 
**Instructions**
 
#. In the BitBoxApp sidebar, select Settings > Enable tor proxy.
#. Enable the proxy and confirm the proxy address (127.0.0.1:9050).
#. Restart BitBoxApp in order for the new settings to take effect.
#. In the BitBoxApp sidebar, select Settings > Advanced settings > Connect your own full node
#. In the field “Enter the endpoint”, paste the Tor address and port from your server's Electrs > Properties page. For example: gwdllz5g7vky2q4gr45zGuvopjzf33czreca3a3exosftx72ekppkuqd.onion:50001
#. Click “Check,” and you will be prompted with the message “Successfully established a connection.”
#. Click “Add” to add your node to the node list at the top of the page.
#. Remove the other servers if you want to exclusively connect to your own node.

Guide adapted from `Shiftcrypto <https://shiftcrypto.support/help/en-us/14-privacy/29-how-to-connect-the-bitboxapp-to-my-own-full-node>`__.


.. _blockstream-green:

Blockstream Green
-----------------

**Available For**

 - Android
 - iOS
 - Linux
 - macOS
 - Windows
 
**Instructions**
 
 Follow the `guide <https://github.com/Start9Labs/electrs-wrapper/blob/master/docs/integrations/blockstreamgreen/guide.md>`__.


.. _blue-wallet-bitcoin:

BlueWallet
----------

 **Available For**

  - Android
  - iOS
 
 **Instructions**

  Follow the `guide <https://github.com/Start9Labs/electrs-wrapper/blob/master/docs/integrations/bluewallet/guide.md>`__.


.. _electrum:

Electrum
--------

 **Available For**

  - Android
  - Linux
  - macOS
  - Windows
 
 **Instructions**
  
  Follow the `guide <https://github.com/Start9Labs/electrs-wrapper/blob/master/docs/integrations/electrum/guide.md>`__.


.. _fully-noded:

FullyNoded
----------

 **Available For**

  - iOS
  - macOS

 **Instructions**
 
  #. In Fully Noded, go to `Settings > Node Manager > +`
  #. Enter your Bitcoin Core credentials. You can do this in one of two ways:

    (A) Use Fully Noded to scan your QuickConnect QR code (located in `Services > Bitcoin Core > properties`); or 
    (B) copy/paste your Bitcoin Core Tor Address (located in `Services > Bitcoin Core > Interfaces`) with :8332 appended, as well as you rpc username and password (located in `Services > Bitcoin Core > Config > RPC Settings`).


.. _ledger-live:

.. Ledger Live
.. ===========

.. .. tip:: Built for use with Ledger hardware devices

.. .. warning:: UNTESTED

.. _nunchuk:

Nunchuk
-------

 **Available For**

   - Android
   - iOS
   - Linux
   - macOS
   - Windows
 
 **Instructions**
 
   #. Install the `Electrs` service from the Start9 Marketplace
   #. Follow the `guide <https://github.com/Start9Labs/electrs-wrapper/blob/master/docs/integrations/nunchuk/guide.md>`__.


.. _samourai:

Samourai
--------

 .. note:: Not Possible at this time - Requires Dojo Stack
 
 .. _sparrow:

Sparrow
-------

 **Available For**

  - Linux
  - macOS
  - Windows
 
 **Instructions**

  Connect Sparrow directly to your `Bitcoin Core`:
  
  * Follow this `guide <https://github.com/Start9Labs/bitcoind-startos/blob/v25.0.0.3/docs/integrations/sparrow/guide.md>`__.

  **CAUTION** Until we get per-user rpc restrictions built into Bitcoin Core, this is technically more dangerous than using the electrum server method, because it requires createwallet and similar RPC calls.  However, exploiting it relies on there being a vulnerability in Bitcoin Core.  Likely there isn't, but if this makes you uneasy, please use the electrs method below.
 
  **OPTIONAL** (but less reliable) -- Connect Sparrow to Electrs via Tor:

  #. Install the `Electrs` service from the Start9 Marketplace
  #. Follow this `guide <https://github.com/Start9Labs/electrs-wrapper/blob/master/docs/integrations/sparrow/guide.md>`__.


.. _specter-wallet:

Specter
-------

 **Available For**

  - Linux
  - macOS
  - StartOS
  - Windows
 
 **Instructions**

  Follow the guide for `macOS <https://github.com/Start9Labs/bitcoind-startos/blob/v25.0.0.3/docs/integrations/specter/macos.md>`__ or `Windows <https://github.com/Start9Labs/bitcoind-startos/blob/v25.0.0.3/docs/integrations/specter/windows.md>`__.


.. _trezor-suite:

Trezor Suite
------------

 .. tip:: Built for use with Trezor hardware devices
 
 **Available For**

  - Linux
  - macOS
  - Windows
 
 **Instructions**
  
  Follow the `guide <https://github.com/Start9Labs/electrs-wrapper/blob/master/docs/integrations/trezor/guide.md>`__.
  
