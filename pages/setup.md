---
layout: default
title: Set-up
nav_order: 2
permalink: setup
---
# Set-up (general)
## Software

Download and install the following software on a HIPPA compliant device. If you are on a University of Minnesota computer, you may need to contact IT to install the software for you if it is not already installed. Check the Self-Service app to see if the software is available for download.

| Software        | Download link          | Notes |
|:-------------|:------------------|:------|
| Box Drive  | [Box.com](https://www.box.com/resources/downloads) |   |
| Praat | [fon.hum.uva.nl](https://www.fon.hum.uva.nl/praat/)   | |
| R           | [cran.rstudio.com](https://cran.rstudio.com/)      |    |
| RStudio           | [posit.co](https://posit.co/download/rstudio-desktop/) | Optional  |
| Python           | [python.org](https://www.python.org/downloads/) |   |

### Box Drive
Box Drive is a cloud storage service that allows you to access Box files on your local machine. Any folder or file shared with you when visiting [box.umn.edu](https://box.umn.edu) will be accessible. You will need to install and mount Box Drive to run the speech data through the pipeline. 

After installing Box Drive, you should see a new drive on your computer. You can access the drive by opening Finder and clicking on the Box icon in the systems tray under 'Locations'. If you don't see the 'Locations' header, you can open Box Drive from your Applications folder.

<img src="{{ site.baseurl }}/img/mac-mount-box.png" alt="im" style="height: 75%;"/>

### Praat
Praat is a software package for the analysis of speech in phonetics. The software should install on your computer and be available to open from the Applications folder. The logo looks like a pair of lips and an ear.

<div style="display: flex; justify-content: left;">
  <figure>
    <img src="{{ site.baseurl }}/img/praat-mac.png" style="width: 75%;">
    <figcaption>Mac logo</figcaption>
  </figure>
  <figure>
    <img src="{{ site.baseurl }}/img/praat-wind.png" style="width: 64%;">
    <figcaption>Windows logo</figcaption>
  </figure>
</div>

### Python
Python is a programming language that will be used to run the pipeline. You will need to install Python 3.7 or later. After installing Python, you should be able to open the terminal or command prompt and type `python` to open the Python interpreter. You should see something like the following:

```bash
Python 3.11.5 (main, Sep  1 2023, 16:14:00) [Clang 14.0.3 (clang-1403.0.22.14.1)] on darwin
Type "help", "copyright", "credits" or "license" for more information.
>>>
```

Type `exit()` and press Enter to close the Python interpreter.

### R and RStudio
R is a programming language and free software environment. RStudio is an integrated development environment (IDE) for R. R will be used to clean and merge the data after the processing pipeline is complete. RStudio is not necessary, but it is recommended for ease of use.


# Set-up (DBS in ET study)
## Access

{: .note }
Personnel must have completed HIPAA/CITI training and be approved by the IRB as a member of *this* study to access the data.

In order to access the speech data, you will need to have access to the `ETC_private` folder on Box. This folder contains the speech data and other files necessary for processing the data. This folder contains PHI and must be handled according to [HIPAA guidelines](https://www.hhs.gov/hipaa/for-professionals/security/laws-regulations/index.html).

If at any point, you do not have access to a folder or drive, please contact Rebecca Butler (**butle821@umn.edu**) for access. You may still need to finish training to be added to the protocol and granted access. If your protocol status is unknown, you can contact Peter Grund (**grund130@umn.edu**) to determine your status.

## Box Drive
Once you've installed and opened Box Drive, you can navigate to the folder where the speech data is stored. The folder is called `Assessment_Speech` and is located in the `ETC_private` folder. Your Box Drive will look different depending on how many folders you have access to. 

<img src="{{ site.baseurl }}/img/mac-box-home.png" alt="im" />


# Set-up (CR-DBS study)
## Access

{: .note }
Personnel must have completed HIPAA/CITI training and be approved by the IRB as a member of *this* study to access the data.

In order to access the speech data, you will need to have access to the `CR DBS for ET - UH3` folder on Box. This folder contains the speech data and other files necessary for processing the data. This folder contains PHI and must be handled according to [HIPAA guidelines](https://www.hhs.gov/hipaa/for-professionals/security/laws-regulations/index.html).

If at any point, you do not have access to a folder or drive, please contact Peter Grund (**grund130@umn.edu**) for access. You may still need to finish training to be added to the protocol and granted access. 
