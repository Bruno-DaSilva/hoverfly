.. _simulations_io:

Creating and exporting a simulation
===================================

Start Hoverfly and set it to Capture mode

.. code:: bash

    hoverctl start
    hoverctl mode capture

Make a request with cURL, using Hoverfly as a proxy server:

.. code:: bash

    curl --proxy http://localhost:8500 http://time.jsontest.com

View the Hoverfly logs

.. code:: bash

    hoverctl logs

Export the simulation to a JSON file

.. code:: bash

    hoverctl export simulation.json

Stop hoverfly

.. code:: bash

    hoverctl stop

You'll now see a ``simulation.json`` file in your current working directory, which contains all your simulation data.

In case you are curious, the sequence diagram for this process looks like this:

.. figure:: exportingsimulations.mermaid.png
