PDK structure
======================

Process Design Kit (PDK) is a tool for designated users to generate circuit layouts based on CORNERSTONE design rules and technology settings.

``corner_stone_pdk_SOI500nm`` package includes four subfolders: ``components``, ``examples``, ``technology``, and ``util``.

* ``components``

    * Fixed cells: All fixed cells, including ``Bend``, ``Packaging``, ``Design Area``,``Flip Chip Bonding``, ``Heater``, ``MultiMode Interferometer`` and ``Waveguide`` are named and designed by **CORNERSTONE** and cannot be changed.

    * Parametrized cells (PCells): Designed by **LDA**, including ``Bend``, ``Straight``, etc and by **CORNERSTONE**, including ``Waveguide`` and ``Taper``. Please see ``gpdk > components`` for more designed components by **LDA**.

* ``examples``

    * ``link.py`` : Test circuit to test if the cell (``SOI500nm_1550nm_TE_RIB_2x1_MMI``), auto routing, and auto link function works normally under the PDK setting. Please see ``gpdk > examples`` for more circuit examples.

* ``technology``

    * Store the technology setting which matched the CORNERSTONE design rules. We recommend users not to change the settings in technology folder.

    * See chapter ``Technology setting`` for more specific definition.

* ``util``

    * Useful functions when generating circuit layouts.

    * Please see **PhotoCAD** online manual for more information.

* ``layers.lyp`` : This file allows layout tools e.g. Klayout to recognize the layer information when displaying gds file to the layout tool.

    .. image:: ../images/lyp.png

