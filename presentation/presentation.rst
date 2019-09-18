:title: Spinnaker & k8s
:author: Thomas A. McGonagle
:keywords: Spinnaker, k8s, kubernetes
:skip-help: true
:css: presentation.css

.. header::
    .. image:: images/Armory_logo.gif 
        :height: 300px
        :width: 600px
        :align: center
        :target: https://armory.io

.. footer::
    .. image:: images/spinnaker.png 
        :height: 70px
        :width: 90px
        :align: center
        :target: https://www.spinnaker.io/

    

----

:id: title-slide

Spinnaker & k8s
===============
9/23/19 - 9/26/19
-----------------

.. note::

  * note


----

:id: agenda

Agenda
======

* whoami

* Administrvia

* Spinnaker and DevOps Overview

* CI/CD and Continuous Improvement

* Docker and k8s

.. note::

  * note

----

:id: who-am-i

/usr/bin/whoami
===============
Thomas A. McGonagle
-------------------
Solutions Architect
-------------------
thomas.mcgonagle@armory.io
--------------------------
@mcgonagle
----------

.. image:: images/thomas_mcgonagle.png
    :height: 400px
    :width: 500px

.. note::
  * note


----

:id: intro

Introductions
===================

* Name

* Role

* Favorite Terrible Movie 

.. note::

  * note

----

:id: spinnaker-metaphor

Spinnaker Metaphor
========================

.. image:: images/waterworld.jpg 
    :height: 600px
    :width: 400px

.. note::
  * note

----

:id: training-goals

Training Goals
==============

* Grok Spinnaker & k8s

* ??

.. image:: images/grok.png
    :height: 300px
    :width: 900px
    :align: right

.. note::

  * note

----

:id: workshop-philosophy

Training Philosophy
===================

.. image:: images/grampy.png 
    :height: 175px
    :width: 250px
    :align: left



.. image:: images/socrates.png 
    :height: 175px
    :width: 250px
    :align: right

----

:id: learning-fun 

Fun Learning Strategies
=======================

.. image:: images/fun_learning.png 
    :height: 800px
    :width: 800px

.. note::
  * note

----

:id: instrument 

Play your Computer Like an Instrument
=====================================

.. image::  https://cdn.shopify.com/s/files/1/0182/0563/products/MaestroVNTop_682x1800_7159c927-5752-43e0-9c2e-a19df87bf18b_800x.JPG?v=1551819005
    :height: 600px
    :width: 600px

.. note::
  * note

----

:id: devops-definition

DevOps Definition
=================

Technical and **Cultural** focus on **Teamwork** and the software delivery **Mission** 
--------------------------------------------------------------------------------------

.. note::

    * note


----

:id: devops-tenants

DevOps Tenants - ACAMS+
=======================

* Agile
* Culture
* Automation
* Metrics
* Sharing
* Plus...

.. note::

    * note

----

:id: devops-practices

DevOps Practices
=======================

.. image:: images/devops_playbook.png 
    :height: 600px
    :width: 1200px
    :align: left
    :target: https://www.dropbox.com/s/wj2jzq66oih030q/enterprise-devops-playbook.pdf?dl=0

.. note::

    * note

----

:id: hovercaft

hovercraft
==========

.. image:: https://www.hoverstream.com/wp-content/uploads/2016/01/Marlin-II_Main.png
    :height: 600px
    :width: 600px
    :align: center 
    :target: https://hovercraft.readthedocs.io/en/latest/index.html

 .. note::

    * note

 ----

:id: continuous-improvement 

Continuous Improvement
======================

.. image:: https://www.planview.com/wp-content/uploads/2018/09/what-is-continuous-improvement-leankit.jpg
    :height: 600px
    :width: 1000px
    :align: center

.. note::

    * note

----

:id: three-ways

Three Ways
==========

.. image:: images/three_ways.png 
    :height: 600px
    :width: 1200px
    :align: center

.. note::

    * note

----

:id: dog-food

Dog Food
========

.. image:: https://images-na.ssl-images-amazon.com/images/I/81XPwF8NnAL._SL1500_.jpg
    :height: 600px
    :width: 800px
    :align: center

.. note::

    * note

----

:id: ci-cd

CI/CD
=====

.. image:: https://www.talend.com/wp-content/uploads/DevOps-Talend-1.png
    :height: 600px
    :width: 1200px
    :align: center

.. note::

    * note

----

:id: docker

docker
======

Make a Change and then....

.. code:: python

    docker build --tag=mcgonagle/sharkhack . 
    
    docker run -it --rm -p "9000:9000" mcgonagle/sharkhack

.. note::

    * note

----

:id: k8s

k8s
===

.. code:: python

    docker build --tag=mcgonagle/sharhack .

    docker push mcgonagle/sharkhack:latest

    kubectl -n default run sharkhack --image=mcgonagle/sharkhack 

    kubectl -n default expose deployment/sharkhack --port=9000 --target-port=9000

    kubectl -n default port-forward services/sharkhack 9000:9000

.. note::

    * note

----

:id: docker-desktop

Docker Desktop
==============

.. image:: https://www.docker.com/sites/default/files/d8/styles/large/public/2019-08/docker_desktop_enterprise_image.jpg?itok=KmkLTRBv
    :height: 600px
    :width: 800px
    :align: center 
    :target: https://www.docker.com/products/docker-desktop



.. note::

    * note

----

:id: github-desktop

GitHub Desktop
==============

.. image:: https://desktop.github.com/images/github-desktop-screenshot-mac.png 
    :height: 600px
    :width: 800px
    :align: center 
    :target: https://desktop.github.com/ 

.. note::

    * note

----

:id: visual-studio-code

Visual Studio Code
==================

.. image:: https://upload.wikimedia.org/wikipedia/commons/thumb/9/9a/Visual_Studio_Code_1.35_icon.svg/1200px-Visual_Studio_Code_1.35_icon.svg.png
    :height: 600px
    :width: 600px
    :align: center 
    :target: https://code.visualstudio.com/

.. note::

    * note

----

:id: homebrew

Home Brew
=========

.. image:: https://upload.wikimedia.org/wikipedia/commons/thumb/9/95/Homebrew_logo.svg/1200px-Homebrew_logo.svg.png
    :height: 600px
    :width: 600px
    :align: center 
    :target: https://brew.sh/

.. note::

    * note

----

:id: brew-install

brew install
============

.. code:: python

   brew install kubernetes-helm

   brew install kubectx

.. note::

    * note

----

:id: rst

reStructured Text
=================

.. image:: https://i1.wp.com/itsfoss.com/wp-content/uploads/2018/06/formiko-editor-800x449.jpeg?resize=800%2C449&ssl=1
    :height: 600px
    :width: 600px
    :align: center 
    :target: http://docutils.sourceforge.net/rst.html




.. note::

    * not

----

:id: headers

Headers
=======

.. code:: python
    
    This becomes a h1
    =================

    And this a h2
    -------------

.. note::

    * note

----

:id: bullets

bullets
=======

.. code:: python

    * Bullet 1

        * Bullet 1.1

    * Bullet 2

    * Bullet 3

.. note::

    * note

----

:id: lists

lists
=======

.. code:: python

    1. Item 1

        1.1. Item 1.1

    2. Item 2

    3. Item 3

.. note::

    * note

----

:id: images

images
======

.. code:: python

    .. image:: path/to/image.png
        :height: 600px
        :width: 800px

.. note::

    * note

----

:id: css

css
===

https://github.com/mcgonagle/sharkhack/blob/master/presentation/presentation.css

.. note::

    * note


----

:id: questions

Questions?
==========

Presentation available at: https://github.com/mcgonagle/103

.. note::

    * note
