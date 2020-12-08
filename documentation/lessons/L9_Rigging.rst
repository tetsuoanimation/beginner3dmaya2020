#####################
Rigging for Animation
#####################

The process of creating a control structure that allows us to easily pose and animate our models is called *rigging*. The final product is a model with controllers that allow us to easily pose and animate.

The rigging process is twofold: First we want to create a virtual skeleton and controls for the model and set it up to be manipulated easily. This includes technical setups for easier manipulation. 
Second we want to attach or *'bind'* our model to that skeleton.

**************
Basic concepts
**************

Rigging aims to make animation as easy as possible by creating simple and easy controls to an animator. If possible, we want to try to hide and simplify complexity and make it easy to grasp all functions of our rig at a glance.

Attributes and Channels
=======================

Most animation in Maya relies on changing the values in different channels and attributes over time. In Maya, you can expose any channel on a node to be animated in the channelbox. By default, the most important animation channels are visible and keyable: Translate, Rotate, Scale and Visibility.

If you want to change which channels are shown, you can add channels to the visible and keyable list in the Channel Editor.
You can find the Channel Editor in the Channel Box's *Edit > Channel Control*.
Select attributes and use the 'Move' buttons to change the attributes state.

.. image:: ./images/channelControl.png

You set the status of shown channels by selecting them in the Channel Box and *Right-Clicking* to open the context menu. To the bottom of the menu, you can find the options to 'Hide Selected', 'Make Selected Non-Keyable', 'Make Selected Keyable'.

Channels can also be 'locked'. Locking keeps a channel from being manipulated. Choose 'lock selected' to lock a channel.

.. note::
    It is a good idea to lock channels that should not be changed after the rig is built. Examples are the transformations of anything but controls or driven channels.

You can find more information in the official manual:

    * `Channel Control Editor <https://help.autodesk.com/view/MAYAUL/2020/ENU/?guid=GUID-5636D755-8FA3-4E72-83AD-A67956727D55>`_
    * `Making a channel keyable or non-keyable <https://help.autodesk.com/view/MAYAUL/2020/ENU/?guid=GUID-1C07D176-C4DD-4B2C-BE39-9341A3326DFD>`_
    * `Lock Attributes <https://help.autodesk.com/view/MAYAUL/2020/ENU/?guid=GUID-ECD85CE0-EFBB-4787-9233-E0BB0C1BA3C3>`_
    * `Hiding Manipulators for channels <https://help.autodesk.com/view/MAYAUL/2020/ENU/?guid=GUID-28CDE5C9-59AD-47D3-8DAA-BD1B7D8A1227>`_

Which channels should I show?
-----------------------------

A rig should be simple - this means it should only show channels that we want to animate. If you want a control to only be rotated, hide the scale and translate channels by selecting them in the channelbox, rightclicking and selecting '*Hide*' or '*Lock and Hide*'.
Sometimes it is a good idea to show more channels than the basic ones. It could,for example, be beneficial to give the animator control over a controller's rotation order by showing the 'rotation order' channel and making it keyable.

.. hint::
    Show as little channels as needed, but think of unconventional animation that might need more channels than strictly realistic movement would do.

Custom Attributes
-----------------

Connecting Attributes
---------------------

Set Driven Keys
---------------

Constraints
===========

Parent
------

Point
-----

Orient
------

Scale
-----

Combining Constraints
---------------------

Blendshapes
===========

The Shape Editor
----------------

Blendshapes or Joints?
----------------------

Joints and Skeleton
===================

Joints Basics
-------------

Rotation Order
--------------

Joint Align
-----------

Controllers
===========

What makes a good controlshape
------------------------------

* Small visual impact but easy to discern
* Easy to see how it is oriented
* Attributes locked and hidden if not available
* Attributes on the controller

Using offset groups
-------------------

FK & IK
=======

Forward Kinematics (FK)
-----------------------

Inverse Kinematics (IK)
-----------------------

FK / IK - A word on Animation
-----------------------------

Local and Global Rigging
========================

Setting Up a Local Rig
----------------------

Connecting the Local and Global Rigs
------------------------------------

* Base, Skinned and Deformed Mesh
* Blendshapes
* Deformation Order
* Doesn't work for games!

*****************************
Example of setting up modules
*****************************

Basic Control
=============

* Perfect for everything
* Multiple World Controllers

Arm / Leg
=========

Arm / Leg: Basic Setup
----------------------

FK Setup
--------

IK Setup
--------

Connecting FK and IK
--------------------

Hand & Fingers
==============

Hand: Basic Setup
-----------------

Control all fingers at once
---------------------------

Spine
=====

FK over IK
----------

Foot
====

Foot: Basic Setup
-----------------

Footroll and Reverse Footroll
-----------------------------

*************************
Connecting Rig and Meshes
*************************

Basic structures
================

Joint-in-controls
-----------------

Separate joint hierarchy
------------------------

Connecting Meshes and Joints
============================

Constraining
------------

Soft Skinning
-------------

Add in hierarchy
----------------

* Don't

*************************
Rig Finishing and Cleanup
*************************

* Lock and Hide 
* Set up layers
* Make sure animators can't break the rig
* TEST THE RIG


