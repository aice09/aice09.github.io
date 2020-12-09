---
layout: articles
title: "Install and Activate Office 2019 for FREE Legally Using Volume License"
author: Carl Angelo Nievarez
readingduration: 5 minutes
date: 2020-10-21
tags: "productivity office "
categories: software
image: http://www.mediafire.com/convkey/8e26/24w2wur3rysimxhzg.jpg?size_id=8
keywords: microsoft microsoft-office microsoft-office-2019 microsoft-office-activation
---

Microsoft Office is a suite of desktop productivity applications that is designed specifically by Microsoft for business use. It is a proprietary product of Microsoft Corporation and was first released in 1990. For decades, MS Office has been a dominant model in delivering modern office-related document-handling software environments.

Microsoft Office has become a leading platform to drive productivity at home and in the workplace. Whether it's managing email in Outlook, or building analysis spreadsheets in Excel, Office has made carrying out many computer based tasks easier for all of us.

## How to download Office 2019 from Microsoft Homepage?

To download Microsoft office application just click the following link below:

- [Microsoft Office Professional Plus 2019 (32&64)](http://officecdn.microsoft.com/pr/492350f6-3a01-4f97-b9c0-c7c6ddf67d60/media/en-us/ProPlus2019Retail.img)
- [Microsoft Office Professional Plus 2016 (32&64)](https://msguides.com/microsoft-software-products/install-office-2016-multilanguage.html)
- [Microsoft Office Project Professional (32&64)](#!)
- [Microsoft Office Visio Professional (32&64)](#!)

## Activating Office 2019 using KMS License Key

### A. Running commands one by one manually

1. Open command prompt as administrator
2. Open location of the Office installed on your PC. Most of the time the location of your Microsoft office application is Program Files depends also in your architecture.
   ```
   cd /d %ProgramFiles%\Microsoft Office\Office16
   cd /d %ProgramFiles(x86)%\Microsoft Office\Office16
   ```
3. Convert your retail license to volume one
   ```
   for /f %x in ('dir /b ..\root\Licenses16\ProPlus2019VL*.xrm-ms') do cscript ospp.vbs /inslic:"..\root\Licenses16\%x"
   ```
   If your Office is got from Microsoft, this step is required. On the contrary, if you install Office from a Volume ISO file, this is optional so just skip it if you want.
4. Activate your Office using KMS client key

   Make sure your PC is connected to the internet, then run the following command.

   ```
   cscript ospp.vbs /setprt:1688
   cscript ospp.vbs /unpkey:6MWKP >nul
   cscript ospp.vbs /inpkey:NMMKJ-6RK4F-KMJVX-8D9MJ-6MWKP
   cscript ospp.vbs /sethst:kms8.msguides.com
   cscript ospp.vbs /act
   ```

   Here is all the text you will get in the command prompt window.

   ```
   C:\Windows\system32>cd /d %ProgramFiles%\Microsoft Office\Office16
   C:\Program Files\Microsoft Office\Office16>cd /d %ProgramFiles(x86)%\Microsoft Office\Office16
   The system cannot find the path specified.
   C:\Program Files\Microsoft Office\Office16>for /f %x in ('dir /b ..\root\Licenses16\ProPlus2019VL*.xrm-ms') do cscript ospp.vbs /inslic:"..\root\Licenses16\%x"
   C:\Program Files\Microsoft Office\Office16>cscript ospp.vbs /inslic:"..\root\Licenses16\ProPlus2019VL_KMS_Client_AE-ppd.xrm-ms"
   Microsoft (R) Windows Script Host Version 5.812
   Copyright (C) Microsoft Corporation. All rights reserved.
   ---Processing--------------------------
   Installing Office license: ..\root\licenses16\proplus2019vl_kms_client_ae-ppd.xrm-ms
   Office license installed successfully.
   ---Exiting-----------------------------
   C:\Program Files\Microsoft Office\Office16>cscript ospp.vbs /inslic:"..\root\Licenses16\ProPlus2019VL_KMS_Client_AE-ul-oob.xrm-ms"
   Microsoft (R) Windows Script Host Version 5.812
   Copyright (C) Microsoft Corporation. All rights reserved.
   ---Processing--------------------------
   Installing Office license: ..\root\licenses16\proplus2019vl_kms_client_ae-ul-oob.xrm-ms
   Office license installed successfully.
   ---Exiting-----------------------------
   C:\Program Files\Microsoft Office\Office16>cscript ospp.vbs /inslic:"..\root\Licenses16\ProPlus2019VL_KMS_Client_AE-ul.xrm-ms"
   Microsoft (R) Windows Script Host Version 5.812
   Copyright (C) Microsoft Corporation. All rights reserved.
   ---Processing--------------------------
   Installing Office license: ..\root\licenses16\proplus2019vl_kms_client_ae-ul.xrm-ms
   Office license installed successfully.
   ---Exiting-----------------------------
   C:\Program Files\Microsoft Office\Office16>cscript ospp.vbs /inslic:"..\root\Licenses16\ProPlus2019VL_MAK_AE-pl.xrm-ms"
   Microsoft (R) Windows Script Host Version 5.812
   Copyright (C) Microsoft Corporation. All rights reserved.
   ---Processing--------------------------
   Installing Office license: ..\root\licenses16\proplus2019vl_mak_ae-pl.xrm-ms
   Office license installed successfully.
   ---Exiting-----------------------------
   C:\Program Files\Microsoft Office\Office16>cscript ospp.vbs /inslic:"..\root\Licenses16\ProPlus2019VL_MAK_AE-ppd.xrm-ms"
   Microsoft (R) Windows Script Host Version 5.812
   Copyright (C) Microsoft Corporation. All rights reserved.
   ---Processing--------------------------
   Installing Office license: ..\root\licenses16\proplus2019vl_mak_ae-ppd.xrm-ms
   Office license installed successfully.
   ---Exiting-----------------------------
   C:\Program Files\Microsoft Office\Office16>cscript ospp.vbs /inslic:"..\root\Licenses16\ProPlus2019VL_MAK_AE-ul-oob.xrm-ms"
   Microsoft (R) Windows Script Host Version 5.812
   Copyright (C) Microsoft Corporation. All rights reserved.
   ---Processing--------------------------
   Installing Office license: ..\root\licenses16\proplus2019vl_mak_ae-ul-oob.xrm-ms
   Office license installed successfully.
   ---Exiting-----------------------------
   C:\Program Files\Microsoft Office\Office16>cscript ospp.vbs /inslic:"..\root\Licenses16\ProPlus2019VL_MAK_AE-ul-phn.xrm-ms"
   Microsoft (R) Windows Script Host Version 5.812
   Copyright (C) Microsoft Corporation. All rights reserved.
   ---Processing--------------------------
   Installing Office license: ..\root\licenses16\proplus2019vl_mak_ae-ul-phn.xrm-ms
   Office license installed successfully.
   ---Exiting-----------------------------
   C:\Program Files\Microsoft Office\Office16>cscript ospp.vbs /setprt:1688
   Microsoft (R) Windows Script Host Version 5.812
   Copyright (C) Microsoft Corporation. All rights reserved.
   ---Processing--------------------------
   Successfully applied setting.
   ---Exiting-----------------------------
   C:\Program Files\Microsoft Office\Office16>cscript ospp.vbs /unpkey:6MWKP >nul
   C:\Program Files\Microsoft Office\Office16>cscript ospp.vbs /inpkey:NMMKJ-6RK4F-KMJVX-8D9MJ-6MWKP
   Microsoft (R) Windows Script Host Version 5.812
   Copyright (C) Microsoft Corporation. All rights reserved.
   ---Processing--------------------------

   ---Exiting-----------------------------
   C:\Program Files\Microsoft Office\Office16>cscript ospp.vbs /sethst:kms8.msguides.com
   Microsoft (R) Windows Script Host Version 5.812
   Copyright (C) Microsoft Corporation. All rights reserved.
   ---Processing--------------------------
   Successfully applied setting.
   ---Exiting-----------------------------
   C:\Program Files\Microsoft Office\Office16>cscript ospp.vbs /act
   Microsoft (R) Windows Script Host Version 5.812
   Copyright (C) Microsoft Corporation. All rights reserved.
   ---Processing--------------------------
   Installed product key detected - attempting to activate the following product:
   SKU ID: 85dd8b5f-eaa4-4af3-a628-cce9e77c9a03
   LICENSE NAME: Office 19, Office19ProPlus2019VL_KMS_Client_AE edition
   LICENSE DESCRIPTION: Office 19, VOLUME_KMSCLIENT channel
   Last 5 characters of installed product key: 6MWKP


   ---Exiting-----------------------------
   C:\Program Files\Microsoft Office\Office16>
   ```

### B. Activating MS Office 2019 Using Batch Scripts

This method is activation using a batch file

1. Copy the following code into a new text document.
   ```
   @echo off
   title Activate Microsoft Office 2019 ALL versions for FREE!&cls&echo ============================================================================&echo #Project: Activating Microsoft software products for FREE without software&echo ============================================================================&echo.&echo #Supported products:&echo - Microsoft Office Standard 2019&echo - Microsoft Office Professional Plus 2019&echo.&echo.&(if exist "%ProgramFiles%\Microsoft Office\Office16\ospp.vbs" cd /d "%ProgramFiles%\Microsoft Office\Office16")&(if exist "%ProgramFiles(x86)%\Microsoft Office\Office16\ospp.vbs" cd /d "%ProgramFiles(x86)%\Microsoft Office\Office16")&(for /f %%x in ('dir /b ..\root\Licenses16\ProPlus2019VL*.xrm-ms') do cscript ospp.vbs /inslic:"..\root\Licenses16\%%x" >nul)&(for /f %%x in ('dir /b ..\root\Licenses16\ProPlus2019VL*.xrm-ms') do cscript ospp.vbs /inslic:"..\root\Licenses16\%%x" >nul)&echo.&echo ============================================================================&echo Activating your Office...&cscript //nologo slmgr.vbs /ckms >nul&cscript //nologo ospp.vbs /setprt:1688 >nul&cscript //nologo ospp.vbs /unpkey:6MWKP >nul&cscript //nologo ospp.vbs /inpkey:NMMKJ-6RK4F-KMJVX-8D9MJ-6MWKP >nul&set i=1
   :server
   if %i%==1 set KMS=kms7.MSGuides.com
   if %i%==2 set KMS=kms8.MSGuides.com
   if %i%==3 set KMS=kms9.MSGuides.com
   if %i%==4 goto notsupported
   cscript //nologo ospp.vbs /sethst:%KMS% >nul&echo ============================================================================&echo.&echo.
   cscript //nologo ospp.vbs /act | find /i "successful" && (echo.&echo ============================================================================&echo.&echo #My official blog: MSGuides.com&echo.&echo #How it works: bit.ly/kms-server&echo.&echo #Please feel free to contact me at msguides.com@gmail.com if you have any questions or concerns.&echo.&echo #Please consider supporting this project: donate.msguides.com&echo #Your support is helping me keep my servers running everyday!&echo.&echo ============================================================================&choice /n /c YN /m "Would you like to visit my blog [Y,N]?" & if errorlevel 2 exit) || (echo The connection to my KMS server failed! Trying to connect to another one... & echo Please wait... & echo. & echo. & set /a i+=1 & goto server)
   explorer "http://MSGuides.com"&goto halt
   :notsupported
   echo.&echo ============================================================================&echo Sorry! Your version is not supported.&echo Please try installing the latest version here: bit.ly/aiomsp
   :halt
   pause >nul
   ```
2. Save the text file as a batch file with **.cmd** or **.bat** extension.
3. Run this batch file with admin rights or **Run as administrator**.
4. Check activation status again and wait for the product to be activated.

Done! You Office has been activated successfully.

**Reference:**

- [https://www.techopedia.com/definition/20737/microsoft-office](https://www.techopedia.com/definition/20737/microsoft-office)
- [https://www.e-careers.com/connected/8-benefits-of-microsoft-office](https://www.e-careers.com/connected/8-benefits-of-microsoft-office)
- [https://msguides.com/microsoft-software-products/office-2019.html](https://msguides.com/microsoft-software-products/office-2019.html)
