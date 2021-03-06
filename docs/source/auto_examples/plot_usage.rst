.. note::
    :class: sphx-glr-download-link-note

    Click :ref:`here <sphx_glr_download_auto_examples_plot_usage.py>` to download the full example code
.. rst-class:: sphx-glr-example-title

.. _sphx_glr_auto_examples_plot_usage.py:


Basic usage
===========

This example presents the basic usage of brokenaxes




.. image:: /auto_examples/images/sphx_glr_plot_usage_001.png
    :class: sphx-glr-single-img





.. code-block:: default



    import matplotlib.pyplot as plt
    from brokenaxes import brokenaxes
    import numpy as np

    fig = plt.figure(figsize=(5,2))
    bax = brokenaxes(xlims=((0, .1), (.4, .7)), ylims=((-1, .7), (.79, 1)), hspace=.05)
    x = np.linspace(0, 1, 100)
    bax.plot(x, np.sin(10 * x), label='sin')
    bax.plot(x, np.cos(10 * x), label='cos')
    bax.legend(loc=3)
    bax.set_xlabel('time')
    bax.set_ylabel('value')


.. rst-class:: sphx-glr-timing

   **Total running time of the script:** ( 0 minutes  12.282 seconds)


.. _sphx_glr_download_auto_examples_plot_usage.py:


.. only :: html

 .. container:: sphx-glr-footer
    :class: sphx-glr-footer-example



  .. container:: sphx-glr-download

     :download:`Download Python source code: plot_usage.py <plot_usage.py>`



  .. container:: sphx-glr-download

     :download:`Download Jupyter notebook: plot_usage.ipynb <plot_usage.ipynb>`


.. only:: html

 .. rst-class:: sphx-glr-signature

    `Gallery generated by Sphinx-Gallery <https://sphinx-gallery.readthedocs.io>`_
