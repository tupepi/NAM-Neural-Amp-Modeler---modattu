Training in the cloud with Google Colab
=======================================

If you don't have a good computer for training ML models, you use Google Colab
to train in the cloud using the pre-made Jupyter notebook at 
`bin/train/easy_colab.ipynb <https://github.com/sdatkinson/neural-amp-modeler/blob/main/bin/train/easy_colab.ipynb>`_, 
which is designed to be used with 
`Google Colab <https://colab.research.google.com/>`_.

Opening the notebook
--------------------

To open the notebook in Colab, follow 
`this link <https://colab.research.google.com/github/sdatkinson/neural-amp-modeler/blob/27c6a048025e7894e0d89579cfda6c59d93e0f20/bin/train/easy_colab.ipynb>`_.

.. note:: Most browsers work, but Firefox can be a bit temperamental. This isn't
    NAM's fault; Colab just prefers Chrome (unsurprisingly).

You'll be met with a screen like this:

.. image:: media/colab/welcome.png

Reamping: Getting data for your model
-------------------------------------

In order to train, you're going to need data, which means you're going to need 
an amp or a pedal you want to model, and you're going to need to have gear to 
reamp with it. Start by downloading the standardized test signal here:

.. image:: media/colab/get-input.png
    :scale: 20 %

If you need help with reamping, others 
`on YouTube <https://www.youtube.com/results?search_query=reamping+tutorial>`_
have made high-quality tutorials.

.. note:: You need to make sure that your exported file is the same length as 
    the input file. To help with this, the standardized input files are an 
    exact number of seconds long. If you drop them into a DAW session at 120 
    BPM, you can snap your guides to the beat and easily get the reamp of the 
    right length.

However, if you want to skip reamping for your first model, you can download 
these pre-made files:

* `v1_1_1.wav <https://drive.google.com/file/d/1CMj2uv_x8GIs-3X1reo7squHOVfkOa6s/view?usp=drive_link>`_, 
  a standardized input file.
* `output.wav <https://drive.google.com/file/d/1e0pDzsWgtqBU87NGqa-4FbriDCkccg3q/view?usp=drive_link>`_, 
  a reamp of the same overdrive used to make 
  `ParametricOD <https://www.neuralampmodeler.com/post/the-first-publicly-available-parametric-neural-amp-model>`_.

To upload your data to Colab, click the Folder icon here:

.. image:: media/colab/file-icon.png
    :scale: 50 %

and either drag and drop the files into the panel or select them after clicking 
the upload button.

.. image:: media/colab/upload.png

**Wait for the files to finish uploading before proceeding.** If you don't, then
strange errors will happen.

Training
--------

At this point, you can train your model with a single click: just click the Play
button and everything will finish in about 10 minutes.

.. image:: media/colab/1-click-train.png

However, there are a lot of options below that you can use to tweak the training
that are worth getting familiar with.

TODO: explain the options.

Downloading your model
----------------------

Once training is done, you can download your model as a .nam file from the file 
browser:

.. image:: media/colab/download.png
    :scale: 20 %

If you don't see it, you might have to refresh the file browser:

.. image:: media/colab/refresh.png
    :scale: 20 %
