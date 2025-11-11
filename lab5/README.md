# Lab Assignment 5 - Data Privacy

This lab assignment studies data privacy issues using a tool called ARX on a SEED VM. In this lab, you will learn data anonymization by applying the k-anonymity model.

### Acknowledgement

This lab is adopted with some minor revisions from the material by Dr. Mengjun Xie at the University of Tennessee at Chattanooga and Dr. Na Li at Prairie View A&M University.

## Lab Manual and Datasets

The lab manual and several datasets are available on Canvas. You will find a set of questions and tasks in the lab manual.


## Environment Setup
> [!IMPORTANT]
> If your laptop runs into VM issues, you can always do the lab on the **MSSI Lab** computers. First **activate your ISI/MSSI account**: https://wiki.isi.jhu.edu/index.php/MSSI_Accounts. For details, see Christopher Venghaus’s email titled **“MSSI Account Information.”**


### 1. Intel/AMD Machines x86-64 (Using VM)
Please reuse the VM/environment from **Lab 1**. If you already finished Lab 1 setup, you can skip this section. Otherwise, follow: [Lab 1 – Environment Setup](../lab1/README.md#environment-setup).

#### Install ARX on the SEED VM:

1. Open the VM.
2. In your VM, go to the ARX download website: https://arx.deidentifier.org/downloads/.
3. From Anonymization Tool -> Installer, download the `Linux/GTK 64bit` version of the ARX.
4. After download the ARX, in you VM file folder, open the terminal.
5. Use the command `chmod +x ARX-3.9.2-linux-x64-installer.run` to make your RUN file executable.
6. Use the command `./ARX-3.9.2-linux-x64-installer.run` to execute your RUN file for downloading the ARX tools on your SEED VM.
7. Downbload the zip file containing the datasets to be used and save them on the VM.

### Apple Machines (ARM chips)

#### Install ARX locally:

1. Go to the ARX download website: https://arx.deidentifier.org/downloads/.
2. From Anonymization Tool -> Installer, download the `MacOS 64-Bit` version of the ARX.
3. After download the ARX, open the folder where the ARX zip file is downloaded. (If it’s already unzipped, skip the next step.)
4. Use the command `unzip ARX-3.9.2-osx-installer.app.zip` to unzip the file.
5. Use the command `cd ARX-3.9.2-osx-installer.app/Contents/MacOS` to get find the installer file `installbuilder.sh`.
6. Use the command `chmod +x installbuilder.sh` to make your SH file executable. If there is no response after running this command, continue with Step 8.
7. An alert will then pop up, stating:

```
Apple could not verify “ARX-3.9.2-osx-installer” is free of malware that may harm your Mac or compromise your privacy.
```

8. Open the `System Preferences` -> `Privacy & Security`. Scroll to the bottom, and you will see a message: “ARX-3.9.2-osx-installer.app was blocked.” Click **Open Anyway / Allow** to proceed with the installation.
9. After the installation, you can find the ARX tool in the Applications folder.

### 2. Continue to Lab Experiment

After successfully installing ARX (on either the SEED VM or an Apple ARM machine):

1. **Download the provided dataset zip file** from this repository.
2. **Extract** the zip file and **open ARX** to import the dataset.
3. You can now **start the anonymization experiment** following the lab instructions.

## Submission Details

- Each group only needs to submit one report in PDF format.
- Please list group members in your report clearly.
- Only typed reports are accepted.
- Make sure to include screenshots, explanations, and all your answers to all the questions in your report.

## Grading

- Completeness (30 pts): All the steps as instructed in the lab manual must be included in the report with adequate evidence.
- Presentation (20 pts): The report must be clear and correct in organization and writing with adequate explanation.
