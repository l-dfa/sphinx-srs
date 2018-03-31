.. srs documentation master file, created by
   sphinx-quickstart on Sat Mar 31 21:53:13 2018.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

System requirement specification template
===========================================

.. toctree::
   :maxdepth: 1
   :caption: Table of Contents:
   :numbered:

   introduction                 <01_introduction>
   assumptions and constraints  <02_assumptions_and_constraints>
   context                      <03_context>
   functional requirements      <04_functional_requirements>
   interface requirements       <05_interface_requirements>
   data requirements            <06_data_requirements>
   operational requirements     <07_operational_requirements>
   user classes and modes of operation     <08_user_classes_and_modes_of_operation>
   guideline for requirements development  <09_guideline_for_requirements_developments>
   requirements traceability matrix        <10_requirements_traceability_matrix>
   attachments or appendices    <11_attachments_or_appendices>


   
Prerequisite
-------------

A computer with:

* **git**;
* **Python** ver. *3.6.4*;
* **virtualev** ver. *15.1.0*;
* Internet connection.

How prepare the initial environment
------------------------------------

To create an empty initial project environment
we can follow these instructions::

  mkdir project_dir                  # dir.root
  cd project_dir
  virtualenv venv                    # create python virtual environment
  source venv/bin/activate           # activate python virtual environment;
                                     #   in windows: venv\scripts\activate
  pip install sphinx
  git init
  mkdir docs
  cd docs
  sphinx-quickstart ...
  
Notes about copyright
-----------------------

This template derives from
`United States Department of Agricolture - System Requirements Specification (SRS) <https://www.unc.edu/~stotts/comp523/USDA-funcSpecs.pdf>`_.

The last is a work of the United States government, so it is intended to be in the 
`public domain <https://en.wikipedia.org/wiki/Public_domain>`_.

About this work, the author releases it under the terms of the 
Simplified BSD License, as follows::

  Copyright (c) 2018, ldfa
  All rights reserved.
  
  Redistribution and use in source and binary forms, with or without
  modification, are permitted provided that the following conditions are met:
  
  1. Redistributions of source code must retain the above copyright notice, this
     list of conditions and the following disclaimer.
  2. Redistributions in binary form must reproduce the above copyright notice,
     this list of conditions and the following disclaimer in the documentation
     and/or other materials provided with the distribution.
  
  THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
  ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
  WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
  DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR CONTRIBUTORS BE LIABLE FOR
  ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
  (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
  LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
  ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
  (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
  SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  
  The views and conclusions contained in the software and documentation are those
  of the authors and should not be interpreted as representing official policies,
  either expressed or implied, of the FreeBSD Project.



Indices and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`
