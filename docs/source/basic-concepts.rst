==============
Basic Concepts
==============

.. _concept-project:

Project
=======

*Project* is the root top-level container for a software model. Its stored as a single ".mdj" file.

Modeling a software system requires describing multiple models, each with its own perspective, to provide a complete presentation of the Project. Each perspective has its own label,such as *Use-Case Model*, *Design Model*, *Component Model*, *Deployment Model*, or others in a *Project*. 

Typically the models in a *Project* follow UML specs, organized as a set of *UMLModels*, *UMLPackages*, or *UMLSubsystems*. If you want to know more about UML Elements, please refer to the OMG UML Specification.

.. seealso::
    :ref:`organizing-project`
        See the Organizing Project section.

.. _concept-element:

Model vs. Diagram
=================

Many users initially misunderstand the difference between *diagramming* or *drawing* tools such as Microsoft Visio and *modeling* tools such StarUML or Rational Software Architect. A *diagram* is not a *Model*. Think of it as the difference between a 2D object (ex. a sheet of paper) versus a 3D object (ex. a tall building). A *diagram* is 2D, a *Model*, 3D.

*Model* or *software model* can describe any aspect of a software system such as its structure, behavior, requirement, and so on. A software model can be represented in textual, mathematical or visual form. One or more *Model elements* are used to create a software model.

A *Diagram* is a visual geometric symbolic representation of a software model. A software model can be represented in one or more diagrams with different aspects . For example, a diagram can focus on a class hierarchy structure while another diagram can focus on interaction between objects. Diagrams consist of *view elements*, which are visual representations of a *model element*.

A *model element* typically has multiple corresponding *view elements*. A model element has its own properties (*name*, *stereotype*, *type*, etc). A view element renders the corresponding model element in a diagram. View elements may exist multiple times in diagram(s). If the *name* of a model element changes, all corresponding view elements reflect the change in their respective diagrams.

.. _concept-fragment:

Fragment
========

A fragment is a slice of a ".mdj" project saved as a separate file with the suffix ".mfj". Any element can be exported as a fragment, but typically *UMLPackage*, *UMLModel*, and *UMLSubsystem* are the candidates. Once a fragment is exported as a file, the fragment can be reused by importing it into another project.

.. seealso::
    :ref:`import-fragment`
        To import a fragment file.

    :ref:`export-fragment`
        To export an element to a fragment file.

.. _concept-profile:

Profile
=======

UML (Unified Modeling Language) is a general-purpose modeling language that can be used to express any kind of software-intensive systems. For this reason, using UML for a specific domain or platform may not be sufficient. However, you can extend and customize UML by defining a UML Profile. StarUML provides built-in UML Profiles which can be used to expand UML. For example, UML profiles can be used for the following purposes.

* Profiles for specific programming languages (C/C++, Java, C#, Python, etc.)
* Profiles for specific development methodologies (RUP, Catalysis, UML Components, etc.)
* Profiles for specific domains (EAI, CRM, SCM, ERP, etc.)


.. _concept-extension:

Extension
=========

An extension is a package which adds new features to StarUML. For example, an extension can extend menus, UIs, dialogs, modeling notations, preferences, etc. An extension can be written in JavaScript, CSS3, and HTML5 and can use Node.js integrated in StarUML. Extensions can be easily installed, uninstalled, and updated via the main extension registry.

.. seealso::
    :doc:`managing-extensions`
        To use extensions.
