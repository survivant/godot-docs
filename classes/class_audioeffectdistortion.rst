.. Generated automatically by doc/tools/makerst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the AudioEffectDistortion.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_AudioEffectDistortion:

AudioEffectDistortion
=====================

**Inherits:** :ref:`AudioEffect<class_audioeffect>` **<** :ref:`Resource<class_resource>` **<** :ref:`Reference<class_reference>` **<** :ref:`Object<class_object>`

**Category:** Core

Brief Description
-----------------

Adds a Distortion audio effect to an Audio bus.

Modify the sound to make it dirty.

Member Variables
----------------

  .. _class_AudioEffectDistortion_drive:

- :ref:`float<class_float>` **drive** - Distortion power. Value can range from 0 to 1. Default value: ``0``.

  .. _class_AudioEffectDistortion_keep_hf_hz:

- :ref:`float<class_float>` **keep_hf_hz** - High-pass filter. Frequencies higher than this value will not be affected by the distortion. Value can range from 1 to 20000. Default value: ``16000``.

  .. _class_AudioEffectDistortion_mode:

- :ref:`int<class_int>` **mode** - Distortion type. Default value: ``MODE_CLIP``.

  .. _class_AudioEffectDistortion_post_gain:

- :ref:`float<class_float>` **post_gain** - Increases or decreases the volume after the effect. Value can range from -80 to 24. Default value: ``0``.

  .. _class_AudioEffectDistortion_pre_gain:

- :ref:`float<class_float>` **pre_gain** - Increases or decreases the volume before the effect. Value can range from -60 to 60. Default value: ``0``.


Numeric Constants
-----------------

- **MODE_CLIP** = **0** --- Digital distortion effect which cuts off peaks at the top and bottom of the waveform.
- **MODE_ATAN** = **1**
- **MODE_LOFI** = **2** --- Low-resolution digital distortion effect. You can use it to emulate the sound of early digital audio devices.
- **MODE_OVERDRIVE** = **3** --- Emulates the warm distortion produced by a field effect transistor, which is commonly used in solid-state musical instrument amplifiers.
- **MODE_WAVESHAPE** = **4** --- Waveshaper distortions are used mainly by electronic musicians to achieve an extra-abrasive sound.

Description
-----------

Modify the sound and make it dirty. Different types are available : clip, tan, lofi (bit crushing), overdrive, or waveshape.

By distorting the waveform the frequency content change, which will often make the sound "crunchy" or "abrasive". For games, it can simulate sound coming from some saturated device or speaker very efficiently.

