#####################
Rigging for Animation
#####################

The process of creating a control structure that allows us to easily pose and animate our models is called *rigging*. The final product is a model with controllers that allow us to easily manipulate and animate the model.

The rigging process is twofold: First we want to create a virtual skeleton and controls for the model and set it up to be manipulated easily. Second we want to attach or *'bind'* our model to that skeleton.

**************
Basic concepts
**************

Attributes and Channels
=======================

Which channels should I show?
-----------------------------

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


