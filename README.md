<div align="center">

# Simple Reproducible Python Discrete-Event Simulation (DES) Template

![python](https://img.shields.io/badge/-Python_3.13-blue?logo=python&logoColor=white)
![licence](https://img.shields.io/badge/Licence-MIT-green.svg?labelColor=gray)

A simple template for creating SimPy DES models in Python, within a **reproducible analytical pipeline (RAP)**. 🔄 <br>
Click on <kbd>Use this template</kbd> to initialise new repository.<br>A `README` template is provided at the **end of this file**.

</div>

<br>

> ⚠️ **Work in progress**

<br>

## 📌  Introduction

TBC. Notes:

* Purpose of template.
* Explanation of implementation (e.g. SimPy, cite).
* Link to STARS.
* Link to relevant publication.

<br>

## 🧐 What are we modelling?

A **simulation** is a computer model that mimics a real-world system. It allows us to test different scenarios and see how the system behaves. One of the most common simulation types in healthcare is **discrete-event simulation (DES)**.

In DES models, time progresses only when **specific events** happen (e.g., a patient arriving or finishing treatment). Unlike a continuous system where time flows smoothly, DES jumps forward in steps between events.

One simple example of a DES model is the **M/M/s queueing model**, which is implemented in this template. It is commonly used to represent systems where people (or tasks) arrive, wait for service, get served, and then leave.

![Simple DES Animation](simple_des.gif)
*Simple model animation created using web app developed by Sammi Rosser (2024) available at https://github.com/hsma-programme/Teaching_DES_Concepts_Streamlit and shared under an MIT Licence.*

For this model, you only need three inputs:

1. **Average arrival rate**: How often people typically arrive (e.g. patient arriving to clinic).
2. **Average service duration**: How long it takes to serve one person (e.g. doctor consultation time).
3. **Number of servers**: How many service points are available (e.g. number of doctors).

In a DES model, we use well-known **statistical distributions** to describe the behaviour of real-world processes. In an M/M/s model we use:

* **Poisson distribution** to model patient arrivals.
* **Exponential distribution** to model server times.

These can be referred to as Markovian assumptions (hence "M/M"), and "s" refers to the number of parallel servers available.

**Examples:**

| Queue | Server/Resource |
| - | - |
| Patients in a waiting room | Doctor's consultation
| Patients waiting for an ICU bed | Available ICU beds |
| Prescriptions waiting to be processed | Pharmacists preparing and dispensing medications |

For further information on M/M/s models, see: Green, L. (2011). Queueing theory and modeling. In *Handbook of Healthcare Delivery Systems*. Taylor & Francis. https://business.columbia.edu/faculty/research/queueing-theory-and-modeling.

<br>

## 🚀  Quickstart

```
# Clone project
git clone https://github.com/pythonhealthdatascience/rap_template_python_des
cd rap_template_python_des

# Create conda environment
conda env create --file environment.yaml
```

<br>

## 📝 Citation

| Contributor | ORCID | GitHub |
| --- | --- | --- |
| Amy Heather | [![ORCID: Heather](https://img.shields.io/badge/ORCID-0000--0002--6596--3479-brightgreen)](https://orcid.org/0000-0002-6596-3479) | https://github.com/amyheather |

<br>

## 📜 Licence

This template is licensed under the MIT License.

```
MIT License

Copyright (c) 2024 STARS Project Team

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

<br>

## 💰 Funding

This project was developed as part of the project STARS: Sharing Tools and Artefacts for Reproducible Simulations. It is supported by the Medical Research Council [grant number [MR/Z503915/1](https://gtr.ukri.org/projects?ref=MR%2FZ503915%2F1)].

<br>
<br>
<br>

**DELETE EVERYTHING ABOVE FOR YOUR PROJECT**

___

<div align="center">

# Your Project Name

[![Template](https://img.shields.io/badge/-rap__template__python__des-017F2F?style=flat&logo=github&labelColor=gray)](https://github.com/pythonhealthdatascience/rap_template_python_des)
![python](https://img.shields.io/badge/-Python_Version-blue?logo=python&logoColor=white)
![licence](https://img.shields.io/badge/Licence-Name-green.svg?labelColor=gray)

</div>

## Description

TBC. Provide instructions and basic example.

<br>

## Installation

TBC. Provide instructions and basic example.

<br>

## How to run

TBC. Provide instructions and basic example.

<br>

## Citation

TBC. Provide instructions and basic example for how to cite their project. Provide correct citation for this template.