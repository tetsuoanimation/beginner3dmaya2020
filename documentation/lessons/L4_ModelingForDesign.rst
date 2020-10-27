##############################
Modeling Techniques for Design
##############################

.. image:: ./images/lesson3_Crates.png

Modeling for design covers modeling techniques that allow you to create complex forms and
shapes quickly. These techniques can be used to design and ideate in 3D. They are - for the 
most part - non-destructive and help you to try different shapes without managing many of the
more complicated parts of creating 3D objects. 

.. warning::
    While you can get ideas out fast using the workflows explained in this lesson, the result
    is not production ready and must be modeled properly after a design decision has been made.
    You can think of these techniques like rough concept art or quickly sketching out ideas 
    before starting production.

************************
Scene management in Maya
************************

Up until now, we did not care to much about how objects are organized in our scene. To keep
our sanity, Maya gives us a wide range of possibilities to organize objects in hierarchical as
well as non-hierarchical ways.

Why you need to work cleanly
============================

Working in a clean manner while trying to design can be a chore at first. However, searching
for objects and digging trough a complicated mess while trying to hold that amazing design
idea in our minds is nearly impossible. Even a simple scene can be made up of hundreds of
objects while complete shots can be made up of thousands of single objects. Ensuring editability
of such a number of objects means you *must* work cleanly from the first pCube you create.

* Over the creation of a shot and scene, these short thoughs and actions you put into working
  cleanly will save you loads of time in a heavy and hard to navigate scene.

* Maya does not allow objects to share a name. This makes automation easier and let's you identify
  each object by its name without even looking at it. - On the other hand, this means you will
  need to name each node properly and with care.

* Most of the time, you will share your asset or scene with a team. Making someone else understand
  your asset quickly will save them time as well as make sure they do not need to break your flow
  to ask for an explanation of how to use the scene.


Tools for clean scenes
======================

Naming Objects
--------------

.. image:: ./images/hierachy_names.png

One of the most powerful tools to ensure easy understanding of the scene as well as mitigating 
name clashes is object / node naming. Find a clear name for each node you expose to the scene 
( esp. Geometry, Groups, Joints, Deformers, Materials, Textures, Shadinggroups, Layers ). If the 
same object appears a lot of time, numbering is a quick tool.
When naming your nodes, adding proper and consistent suffixes makes them easy to identify. It 
also shows how you intend to use them as well as making automation and selecting them by name 
possible.

.. hint::
    I suggest using short and recognizable suffixes. Personally, I like to tag all my meshes with
    '_MSH', joints with '_JNT', layers with '_LYR' and materials with '_MAT'. You can use your own
    suffixes or add other suffixes if you need them. (i.e. adding _EXP to stuff that needs to get 
    exported to a game engine)

Select by name
--------------

Proper naming gives you access to another often overlooked but very powerful tool: Select by name.
By typing the name of an object into the select by name box, you can quickly select an object, even
if you can't see it.

.. image:: ./images/selectByName.gif

Using the wildcard character '\*' you can select all objects that share some part of the name. If you
properly named your objects, you can, for example, select all objects with the suffix _JNT by typing
'\*_JNT' into the box.

.. image:: ./images/selectByNameWildCard.gif

Renaming a lot of objects
-------------------------

You can rename a selection, hierarchy or even all objects in the scene with the 'Search And Replace
Names' Tool. You can find this tool in **Modify > Search and Replace Names...**

.. image:: ./images/searchReplaceNames.png


The scene hierarchy
-------------------
Transforms vs. shapes ( and the weird stuff like pickwalk to shape )
Pivot management
Parent / Child relationship
Transforms in a parent child relationship


Display Layers
--------------
States
Why it makes sense to use them

Sets
----
Selection Sets
Shading sets 
Maya is strange

Managing visibility
-------------------
visibility
isolate Select
intermediate object

***************************
Constructive Solid Geometry
***************************

What is it?
===========

Booleans in Maya
================

*********
Deformers
*********

What is it?
===========

Intro to nonlinear deformers
============================

Painting influence maps
=======================

Baking Geometry
===============

Tweak Nodes
