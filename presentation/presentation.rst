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

    docker build --tag=mcgonagle/103 . 
    
    docker run -it --rm -p "9000:9000" mcgonagle/103

.. note::

    * note

----

:id: k8s

k8s
===

.. code:: python

    docker build --tag=mcgonagle/103 .

    docker push mcgonagle/103:latest

    kubectl -n default run 103 --image=mcgonagle/sharkhack 

    kubectl -n default expose deployment/103 --port=9000 --target-port=9000

    kubectl -n default port-forward services/103 9000:9000

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

:id: migrating-to-the-cloud

Migrating to the Cloud
======================

.. image:: images/migrating_to_the_cloud.png
    :height: 640px
    :width: 1080px
    :align: center

.. note::
    * note

----

:id: rigid-tooling

Rigid and Intertwined Tooling
=============================

.. image:: images/rigid_tooling.png
    :height: 640px
    :width: 1080px
    :align: center

.. note::
    * note

----

:id: unified-approach

A Unified Approach to Migrating
===============================

.. image:: images/unified_approach.png
    :height: 640px
    :width: 1080px
    :align: center

.. note::
    * note

----

:id: deploy-dependencies

Deploy without Dependencies
===========================

.. image:: images/deploy_dependencies.png
    :height: 640px
    :width: 1080px
    :align: center

.. note::
    * note

----

:id: single-pane-glass

Spinnaker is a Single Pane of Glass
===================================

.. image:: images/single_pane_glass.png
    :height: 640px
    :width: 1080px
    :align: center

.. note::
    * note

----

:id: open-source

Spinnaker: The Open Source Standard 
===================================

.. image:: images/open_source.png
    :height: 640px
    :width: 1080px
    :align: center

.. note::
    * note

----

:id: pluggable

Spinnaker is a Pluggable, Cloud Native Platform 
===============================================

.. image:: images/pluggable.png
    :height: 640px
    :width: 1080px
    :align: center

.. note::
    * note

----


:id: before-we-start

Before We Start...
==================

.. note::
    * note

----

:id: cover-today

What are we going to cover today?
=================================

* Intro, Goals, Assumptions
* Background & Philosophy & Terminology
* Spinnaker Archtecture 
* Creating a Spinnaker Application

.. note::
    * note

----

:id: cover-today-cont

What are we going to cover today cont.?
=======================================

* Introductions to Pipelines
* Working with Helm
* Pipeline Strategies
* Introduction to Spring Expression Language (SpEL)
* Deploying Stateful Applications
* Debugging Pipelines

.. note::
    * note

----

:id: spinnaker-fundamentals

Spinnaker - The Fundamentals
============================

.. note::
    * note

----

:id: why-spinnaker

Why Spinnaker was created
=========================

* A brief history of Deployments at Netflix

* A need for end to end orchestration

*  When deploying to the cloud, your development platform should understand the cloud

.. note::
    * note

----

:id: spinnaker-philosophy

Spinnaker Philosophy
====================

* Make all of your infrastructure immutable
* Make the deployment tool aware of infrastructure
* Minimize the possibility of errors in deployments
* Make deployments easy and repeatable
* When deployments fail, make it easy to roll back 
* Make it possible to deploy where you want, when you want 

.. note::
    * note

----

:id: armory-adds

What Armory Adds
================

* Observability through the collection, correlation and presentation of data and metrics
* Enterprise class OSS software integration
* Pipeline as Code
* *Your* line into ongoing OSS development
* Experience running Spinnaker at scale

.. note::
    * note

----

:id: terminology

Terminology
===========

* CI - Continuous Integration
* CD - Continous Delivery
* Continuous Deployment
* Pipeline - all stages of the SDLC
* ServerGroup - Spinnaker term for ASG/ReplicaSet
* Application - Collection of Related Apps
* Project - Collection of related Applications
* Stack - Anything that you want to be integrated together, i.e. environments

.. note::
    * note

----

:id: spinnaker-architecture

Spinnaker Architecture
======================

* 10 micro services
* Written in SpringBoot (Deck is Angular 1/ReactJS)
* Redis/SQL/(Cassandra)
* S3/GCS
* Kubernetes/AWS/GCP

.. note::
    * note

----

:id: spinnaker-diagram

Spinnaker Architecture
======================

.. image:: images/spinnaker_architecture.png
    :height: 640px
    :width: 1080px
    :align: center

.. note::
    * note

----

:id: projects-applications

Projects & Applications
=======================

.. note::
    * note

----

:id: projects

Projects
========

What is a Project?
- A Collection of Applications

Think of this as your Product

.. image:: images/project.png
    :height: 640px
    :width: 1080px
    :align: center

.. note::
    * note

----

:id: applications

Applications
============

Applications are deployable artifacts

Applications map to a single repo

.. image:: images/application.png
    :height: 640px
    :width: 1080px
    :align: center


.. note::
    * note

----

:id: exercise-1

Exercise 1
============

Create a project and an application
 - Project name should be ${username}Project1
 - Applications should be named ${username}UI
 - Applications must include the cloud providers
   - kubernetes
   - AWS
 - Leave the “Repo Type” BLANK
 - Check -> Instance Health: Consider only cloud provider health...
 - Add your application to the project

.. note::
    * note

----

:id: introduction-to-pipelines

Introduction to Pipelines
=========================

.. note::
    * note

----


:id: creating-a-pipeline   

Creating a Pipeline
===================

Pipeline names are freeform

.. image:: images/pipeline.png
    :height: 640px
    :width: 1080px
    :align: center

.. note::
    * note

----

:id: pipeline-configuration

Pipeline Configuration
======================

.. image:: images/pipeline_configuration.png
    :height: 640px
    :width: 1080px
    :align: center


.. note::
    * note


----

:id: pipeline-triggers

Pipeline Triggers
=================

Triggers tell Spinnaker when to start a pipeline
    - Code Commits
    - CI Builds
    - New package or container versions
    - WebHooks
    - Scheduled
    - Other Pipelines

.. note::
    * note

----

:id: git-trigger

The Git Trigger
===============

It's just a webhook!
But its a special webhook.


.. image:: images/git_trigger.png
    :height: 640px
    :width: 1080px
    :align: center


.. note::
    * note

----

:id: stages-overview

Stages Overview
===============

Stages are automated steps of your SDLC
    - Software builds in your CI tool
    - Automated tests
    - Manual tests or judgments
    - Deployments
    - Scaling activities
    - Baking (creating) a new image
    - Evaulations
    - Wait stage
    - Much more...


.. note::
    * note

----

:id: wait-stage

Wait Stage
==========

Introduces an arbitrary wait
Why might we want this?

.. image:: images/wait_stage.png
    :height: 640px
    :width: 1080px
    :align: center

.. note::
    * note


----

:id: manual-judgement-stage

Manual Judgment Stage
=====================

Use a Manual Judgment as a human gate to your next stage


.. image:: images/manual_judgement.png
    :height: 640px
    :width: 1080px
    :align: center


.. note::
    * note


----

:id: execution-options

Execution Options
=================

These are common to all stages

.. image:: images/execution_options.png
    :height: 450px
    :width: 1080px
    :align: center

.. note::
    * note

----

:id: executing-a-pipeline

Executing a Pipeline
====================

.. image:: images/executing_pipeline.png
    :height: 640px
    :width: 1080px
    :align: center

.. note::
    * note


----

:id: demo-working-github

Demo - Working with the GitHub UI
=================================

.. image:: images/demo_github.png
    :height: 450px
    :width: 1080px
    :align: center

.. note::
    * note

----

:id: exercise-2

Exercise 2
==========

1. Clone the GitHub repo https://github.com/armory-training/spintroui

2. Create and push a new branch to the repo called “dev-${username}”

3. Create a pipeline in your ${username}UI application
    - Pipeline should be called “Bake and Deploy”
    - Add a GitHub trigger for your branch of the spintroui repo
    - Add a Wait stage to your pipeline

 4. Add a Manual Judgement stage to your pipeline
    - Provide the user with a custom prompt

    Update the Readme with your username in your branch and git push; 
    Don’t forget to click Save!

.. note::
    * note

----

:id: working-with-helm

Working with Helm
=================

.. note::
    * note

----

:id: helm-chart-artifacts

Helm Chart Artifacts
====================

.. note::
    * note

----


:id: baking-manifests

Baking Manifests
================

.. note::
    * note

----

:id: deploying-manifests

Deploying Manifests
===================

.. note::
    * note

----

:id: working-with-services

Working with Services
=====================

.. note::
    * note

----

:id: health-checks-kubernetes

Kubernetes Health Checks
========================

.. note::
    * note

----

:id: pipeline-strategies 

Pipeline Strategies
===================

.. note::
    * note

----

:id: promotional-pipelines 

Promotional Pipelines
=====================

.. note::
    * note

----

:id: branching-pipelines 

Branching Pipelines
=====================

.. note::
    * note

----

:id: halting-pipelines 

Halting Pipelines
=================

.. note::
    * note

----

:id: multicluster-pipelines 

Multi-Cluster Pipelines
=======================

.. note::
    * note

----

:id: spel-introduction

Spring Expression Language(SpEL) Introduction
=============================================

.. note::
    * note

----

:id: about-spel

About SpEL
==========
* Add logic to pipelines
* Used mostly to eval variables
    * Set vars from build systems
    * Pass image names between stages
    * Retrieve and eval manual judge responses
* Can do much more
    * Embed java/groovy

.. note::
    * note

----

:id: spring-expressions

Spring Expressions
==================
What does a Spring Expression look like?
* A shell variable
Where can I use them?
* Any place in the UI where you can enter free-form text
* In the "Edit Pipeline JSON" tool
When are they evaulated?
* At stage execution time
Any exceptions?
* Yes, can't use during pipeline configuration stage

.. note::
    * note
----

:id: expression-tool 

Expression Tools - Helper Functions
===================================

.. image:: images/expression_tool.png
    :height: 450px
    :width: 1080px
    :align: center

.. note::
    * note
----

:id: expression-tool-helper

Expression Tools - Helper Properties
====================================

.. image:: images/expression_tool_helper.png
    :height: 450px
    :width: 1080px
    :align: center


.. note::
    * note

----

:id: conditional-spel

Conditional SpEL
================

.. image:: images/conditionally_run.png
    :height: 450px
    :width: 1080px
    :align: center

.. note::
    * note

----

:id: stateful-apps

Deploying Stateful Applications
===============================

.. note::
    * note

----

:id: debugging-pipelines

Debugging Pipelines
===================

.. note::
    * note

----

:id: debugging-bakes

Debugging Bakes
===============

.. note::
    * note

----

:id: debugging-deployments

Debugging Deployments
=====================

.. note::
    * note

----


:id: questions

Questions?
==========

Presentation available at: https://github.com/mcgonagle/103

.. note::

    * note

----

:id: thank-you

Thank You Very Much
===================
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