# Reproducible workshop materials

This repository contains the materials and resources you need to create a reproducible workshop.

To get started with your own reproducible workshop, clone this repo and make sure your put all the required resorces into your own clone.

The repository contains the following contents: 

* a [`doc`](./doc) folder, containing two files:
    1. [`for-presenters.md`](./doc/for-presenters.md) should contain information to aid the presenter of the workshop - from background material adding context, to more general information on the structure and flow of the workshop, detailed information about the workshop content and any other suggestions for the presenter. 
    2. [`abstract.md`](./doc/abstract.md) should contain the workshop abstract.

* a [`deploy`](./deploy) folder, containing: 
    1. [`deploy.md`](./deploy/deploy.md) gives clear instructions on how to deploy the workshop both within and outside of RHPDS.
    2. a [`templates`](./deploy/templates) folder, containing any OpenShift templates required to deploy the workshop, as well as any Ansible roles and playbooks.

Your workshop repository should contain:
* a `README.md` file, containing basic, high-level information about the lab. It should contain the lab title, abstract, keywords, intended workshop length(s) and any other relevant information. 
* a `source` folder, containing any Jupyter notebooks or other source material
* `images`: metadata and source to create necessary images, if these are hosted or developed with the workshop
* `sildes`: either in the form of a gdocs link, keynote presentation file, powerpoint presentation or html, in addition to a pdf and a rendered video of any demos needed for the presentation 
* a `workshop.yaml` file, holding the following machine readable metadata:
    - name
    - authors
    - workshop duration
    - source repo
    - keywords
* a `presenters.txt` file to guide the workshop presenter, including:
    - any relevant background content 
    - suggestions for presenters
    - an abstract, suitible for resubmission of the workshop
    - speakers notes (unless included in the slides)
    - notes on modularity of the workshop (optional)
    - notes on ways to extend the length of the material (optional)
* a `deploy.md` file, containing documentation on how to deploy the lab. The file must contain:
    - a RHPDS link
    - instructions to deploy the workshop on RHDPS (in a single command)
    - instructions to deploy the workshop outside of RHPDS (in a single command)
* `templates` 
    - for all OpenShift templates necessary to deploy the workshop _and/or_
    - for all Ansible roles and playbooks necessary to deploy the workshop