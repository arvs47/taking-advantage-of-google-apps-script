# Taking Advantage of Google Apps Script (Tanaike's list)
<a name="TOP"></a>
Here, CLI tools, libraries, Add-ons, Reports, Benchmarks and Sample Scripts for taking advantage of Google Apps Script which are publishing in my [blog](https://tanaikech.github.io/), [Gists](https://gist.github.com/tanaikech) and [GitHub](https://github.com/tanaikech) are summarized. If these are useful for you, I'm glad.

<br>

# Index
- [CLI tools for GAS](#clitool)
- [GAS libraries](#gaslibraries)
- [Go libraries](#golibraries)
- [Node.js modules](#nodemodules)
- [Python library](#pythonlibrary)
- [Add-ons](#addons)
- [Reports](#reports)
- [Benchmarks](#benchmarks)
- [Sample Scripts](#samplescripts)
    - [Files in Google Drive](#filesingoogledrive)
    - [Projects](#projects)
    - [Spreadsheets](#spreadsheets)
    - [Documents](#documents)
    - [Slides](#slides)
    - [Gmail](#gmail)
    - [Chart](#chart)
    - [Slack](#slack)
    - [Virtual Currency](#virtualcurrency)
    - [Stackoverflow](#stackoverflow)
    - [Netatmo](#netatmo)
    - [Etc](#etc)
    - [Node.js](#nodejs)
    - [Golang](#golang)
    - [Python](#python)
    - [Curl](#curl)

<br>
<br>

<a name="clitool"></a>

CLI tools for GAS
=====
- [ggsrun](https://github.com/tanaikech/ggsrun) : Execute Google Apps Script (GAS) at own terminal on local PC.
- [gislack](https://github.com/tanaikech/gislack) : Submit files to both Gist and Slack.
- [goris](https://github.com/tanaikech/goris) : Search for images with Google Reverse Image Search (goris).
- [gogauth](https://github.com/tanaikech/gogauth) : Easily retrieve access token for using APIs on Google.
- [gorearrange](https://github.com/tanaikech/gorearrange) : Interactively rearrange a text data on a terminal.
- [goodls](https://github.com/tanaikech/goodls) : Download shared files from Google Drive.

<br>

<a name="gaslibraries"></a>

GAS libraries
=====
- [BatchRequest](https://github.com/tanaikech/BatchRequest) : This is a library for running Batch Requests using Google Apps Script (GAS).
- [ConvertNFDtoNFC](https://github.com/tanaikech/ConvertNFDtoNFC) : This is a script for converting strings from NFD (Normalization Form Decomposition) to NFC (Normalization Form Composition) using Google Apps Script.
- [FilesApp](https://github.com/tanaikech/FilesApp) : FilesApp is a GAS library for retrieving file and folder list in Google Drive using Google Apps Script (GAS). Also this can create a tree from all files and folders in Google Drive.
- [ImgApp](https://github.com/tanaikech/ImgApp) : This is a library of image tools for Google Apps Script.
- [ManifestsApp](https://github.com/tanaikech/ManifestsApp) : This is a Manifests library for Google Apps Scripts.
- [ProjectApp](https://github.com/tanaikech/ProjectApp) : This is a project library for Google Apps Script (GAS).
- [ProjectApp2](https://github.com/tanaikech/ProjectApp2) : This is a GAS project library for Google Apps Script (GAS). This library can be used for the projects of both standalone script type and container-bound script type.
- [OnedriveApp](https://github.com/tanaikech/OnedriveApp) : This is a library of Google Apps Script for using Microsoft OneDrive.
- [Resumable_Upload_For_WebApps](https://github.com/tanaikech/Resumable_Upload_For_WebApps) : This is a sample script for uploading files with large size (> 50 MB) at Web Apps using Google Apps Script (GAS). The resumable upload method is used for uploading files. This script can be also applied to the script using gapi of javascript.
- [RunAll](https://github.com/tanaikech/RunAll) : This is a library for running the concurrent processing using only native Google Apps Script (GAS).
- [SOUWA_GAS](https://github.com/tanaikech/SOUWA_GAS) : GAS library for summing string elements in an array at the high speed
- [ZipFolder](https://github.com/tanaikech/ZipFolder) : This is a library for zipping a folder using Google Apps Scripts.
- [RangeListApp](https://github.com/tanaikech/RangeListApp) : RangeListApp is a GAS library for retrieving, putting and replacing values for Spreadsheet by a range list with a1Notation using Google Apps Script (GAS).
- [DownloadLargeFilesByUrl](https://github.com/tanaikech/DownloadLargeFilesByUrl) : DownloadLargeFilesByUrl is a GAS library for downloading large files from URL to Google Drive using Google Apps Script (GAS).
- [ArrangeStackingOrder](https://github.com/tanaikech/ArrangeStackingOrder) : ArrangeStackingOrder is a GAS library for arranging the stacking order of page elements on Google Slides using Google Apps Script (GAS).

<br>

<a name="golibraries"></a>

Go libraries
=====
- [go-getfilelist](https://github.com/tanaikech/go-getfilelist) : This is a Golang library to retrieve the file list with the folder tree from the specific folder of Google Drive.

<br>

<a name="nodemodules"></a>
Node.js modules
=====
- [node-getfilelist](https://github.com/tanaikech/node-getfilelist) : This is a Node.js module to retrieve the file list with the folder tree from the specific folder of Google Drive.

<br>

<a name="pythonlibrary"></a>
Python library
=====
- [getfilelistpy](https://github.com/tanaikech/getfilelistpy) : This is a python library to retrieve the file list with the folder tree from the specific folder of Google Drive.

<br>

<a name="addons"></a>

Add-ons
=====
- [RearrangeScript](https://chrome.google.com/webstore/detail/rearrangescripts/ndaicidjkbcpajgejcclgfdcncpoekml) : Rearranging Google Apps Scripts (GAS) in a project which can be seen at the script editor. [GitHub](https://github.com/tanaikech/RearrangeScripts)
- [ShapeApp](https://chrome.google.com/webstore/detail/shapeapp/nmbimbgfafgmkhioolneofjchigbpkhf) : Manipulating shapes on Google Slide. It can create and update shapes by inputting parameters, and can arrange shapes. This is made of Google Apps Scripts (GAS). [GitHub](https://github.com/tanaikech/ShapeApp)

<br>

<a name="reports"></a>

Reports
=====
### [Improved Algorithms for Summation of Array](https://tanaikech.github.io/2016/10/13/improved-algorithms-for-summation-of-array-elements/)
> I considered an efficient algorithm for summation of array elements. All elements in an array are string. When those elements are summed using scripts, a standard method is to add each element in order. If the script is run without any optimize, the process becomes gradually sluggish, because the total amount of active data during the summation process is proportional to the square of the number of array elements. This leads directly to the high process-cost. Such phenomenon notably appears at Google Apps Script (GAS). This report says about the solution of this problem using a new algorithm of a pyramid method. The pyramid method achieves that the total amount of active data increases proportional to the linear of the number of array elements. By this, the processing time becomes much shorter than that of the process using the standard method. The pyramid method achieved the process-cost reduction of 99.7% compared with the standard method at GAS. I realized again that new discoveries are hidden into the familiar scenes of every-day life.

### [Taking Advantage of Manifests by GAS Library](https://gist.github.com/tanaikech/23ddf599a4155b66f1029978bba8153b)
> By recent Google update (Google update at October 24, 2017), various new winds to GAS developers were blown. There is "Manifests" as one of the new winds. "Manifests" makes us manage the project using JSON. Especially, the special scopes which have to use OAuth2 process can be used by only setting them to the Manifests. I think that this is the largest modification. However, when scopes are added to a project using Manifests, users who use the project can use only added scopes. This means that when users create scripts in the project, if there are some scopes which is required to be added, such scopes cannot be automatically added. So the error of "Insufficient Permission" occurs. In this report, I would like to introduce the workaround for avoiding this problem.

### [Difference Between Given Values and Retrieved Values for Shapes on Google Slides](https://gist.github.com/tanaikech/953e630855e65de55d8e5bd448ad764f)
> This is a document for explaining the difference between given values and retrieved values for shapes on Google Slides.

### [Taking advantage of Web Apps with Google Apps Script](https://github.com/tanaikech/taking-advantage-of-Web-Apps-with-google-apps-script)
> There is Web Apps as one of applications using Google Apps Script (GAS). I sometimes use this Web Apps. But I have only a little the information for the specification of Web Apps. So in order to take more advantage of Web Apps, I investigated and summarized about this. The aim of this report is to become one of the basic information for creating various applications using Web Apps with GAS.

### [Limitation of Images for Inserting to Spreadsheet using Google Apps Script](https://gist.github.com/tanaikech/825f1ebfe7822780316d7c15f89dea11)
> Here I would like to introduce about the limitation of images for inserting to Spreadsheet using Google Apps Script (GAS). When you want to insert the images to Spreadsheet using GAS, insertImage() of class Sheet is usually used for this situation. At this time, an error sometimes occurs. This indicates that there is the limitation for inserting images to Spreadsheet. So I investigated the limitation. As a result, it was found that the limitation depends on the image area (pixels^2) rather than the file size of it. The maximum area of image which can be inserted was 1,048,576 pixels^2.

### [Asynchronous Processing using Event Triggers](https://gist.github.com/tanaikech/88f7fd5ed14da5e9afde18310da61cb5)
> This is a report about the possibility of asynchronous process using event triggers. ``onEdit()`` which is a simple trigger is often used as a trigger when the values are modified on Spreadsheet. When users want to use the script including some methods which are required to be authorized as the onEdit event, a installable trigger of onEdit is used. If the trigger is installed for the function of ``onEdit()``, when the event trigger is run, ``onEdit()`` is run 2 times. In order to avoid this, the installable trigger is installed to the functions except for the functions of simple triggers. The functions of simple triggers which is the same events are not used in the project. When I thought about this situation, I thought that both ``onEdit()`` which is run by the simple trigger and the function which is run by the installable trigger might be able to be used, simultaneously. So I investigated about this situation. As the result, it was found that the following simple triggers and installable triggers work as the asynchronous process.

<br>

<a name="benchmarks"></a>

Benchmarks
=====
### [Event Objects for Google Apps Script](https://gist.github.com/tanaikech/4892c97df7ac0504ffd715c2dd6cd546)
> - It was found that the process cost of ``e.range.getA1Notation()`` was 20 % and 10 % for those of ``e.source.getActiveCell().getA1Notation()`` and ``SpreadsheetApp.getActiveSheet().getActiveCell().getA1Notation()``, respectively.

### [Loop for Array Processing using Google Apps Script](https://gist.github.com/tanaikech/848aeafaac1ec676900bb78e3ce220b6)
> - In the case of the sample script for retrieving the multiple of 5 from the array, the loop using "map, filter" is the most suitable way.
> - Ascending order of cost for each method is "map, filter", "Comprehension", "forEach", "for in", "for loop" and "while".
> - Cost for "forEach", "Comprehension" and "map, filter" is lower than that for "for in", "for loop" and "while".
> - Cost of push() and new Array() is almost the same.
> - When the array is changed from 1 dimensional array to 2 dimensional array, the increasing ratio of the cost for "Comprehension", "forEach" and "map, filter" is much lower than that for "for in", "for loop" and "while".
> - For the conventional method using "for loop", a new method could be proposed using the result of this report.
> - For "reduce", the process costs between 1 and 2 dimensional array are almost the same.


### [fetchAll method in UrlFetch service for Google Apps Script](https://gist.github.com/tanaikech/c0f383034045ab63c19604139ecb0728)
> - It was found that the fetchAll method is worked by the asynchronous processing.
> - After it worked by the asynchronous processing, the returned values is reordered by the order of requests.
> - It was also found that if you want to retrieve the data from the several URL, the process cost of ``UrlFetchApp.fetchAll()`` is much lower than that of ``UrlFetchApp.fetch()`` using for loop.

### [Search for Array Processing using Google Apps Script](https://gist.github.com/tanaikech/eda9234822b5dec80549216a43c52652)
> - Process cost of search by indexOf() was the lowest of all methods.
> - 2nd and last one were the search by for loop and the search by the hash, respectively.
> - About the search by hash, although the cost of search by the hash from the object is very low, the cost for creating the object to search the hash was the highest of all. By this, the search by hash became the lowest rank. If the object for searching has already been created, the cost of search by the hash will be the lowest of all.
> - Search using indexOf can reduce the process cost of more than 99 % from the linear search and the search using hash.
> - From these results, it is considered that the scan for indexOf() may be different from the general for loop.

### [Conditional Branch using Google Apps Script](https://gist.github.com/tanaikech/cef47530a58f2d8692cdb1a9d257907b)
> - It was found that the cost of "Ternary operator" was the lowest of all methods and conditions.
> - For the single conditional branch, 2nd one was "If". But for the multiple conditional branches, "Switch" was the 2nd one. This indicates that "If" and "Switch" are suitable for the single and multiple conditional branches (more than 2 branches), respectively.
> - In the case of the multiple conditional branches, the process cost can be reduced by put the condition with the high possibility of "true" to the fore.
> - "Logical operator" was the lowest rank for the single and multiple conditional branches. It is considered that "Logical operator" is not suitable for the general use, because of the high cost and low readability.

### [Decreasing Loop for Array Processing using Google Apps Script](https://gist.github.com/tanaikech/fdd8462a46179efb156cfa0550695c6e)
> - "filter using reversed array" makes the process cost be 43 % lower compare with "Decreasing for loop".
>    - "reversed array" was obtained using "Array.prototype.reverse()" for the created a sample array.
> - "Decreasing for loop" is almost the same with "Increasing for loop".
> - Cost of "reverse()" is sufficiently small for "for loop" and "filter".

### [Reading and Writing Spreadsheet using Google Apps Script](https://gist.github.com/tanaikech/d102c9600ba12a162c667287d2f20fe4)
> In this report, the process cost for reading and writing Spreadsheet has been investigated. From this investigation, the following results were obtained.

> - For the process costs for reading values from Spreadsheet
>     1. Process costs of getValues() and getSheetValues() of Spreadsheet Service are almost the same.
>     1. Process costs of values.get and values.batchGet of Sheets API are almost the same.
>     1. Methods of Sheets API can reduce the process costs from those of Spreadsheet Service by about 35 %.
> - For the process costs for writing values from Spreadsheet
>     1. Process costs of values.update, values.batchUpdate and values.append of Sheets API are almost the same.
>     1. Methods of Sheets API can reduce the process costs from those of Spreadsheet Service by about 19 %.
>     1. There is the inversion point between setValues() of Spreadsheet Service and the methods of Sheets API.
>         - When the data size is small, setValues() is suitable for writing values.
>         - When the data size becomes large, the methods of Sheets API are suitable for writing values.

> From these results, it is considered that the methods for reading and writing Spreadsheet of Sheets API are using the different algorithm and/or process from those of Spreadsheet service.

<br>

<a name="samplescripts"></a>

Sample Scripts
=====

<a name="filesingoogledrive"></a>
#### Files in Google Drive
- [File upload using doPost on Google Web Apps](https://tanaikech.github.io/2017/02/05/file-upload-using-dopost-on-google-web-apps/)
- [Retrieving Access Token for Google Drive API using GAS](https://gist.github.com/tanaikech/64175178489d1d72a6090b79be901c23)
- [Create Folder Tree on Google Drive](https://tanaikech.github.io/2017/03/13/create-folder-tree-on-google-drive/)
- [Download Files Without Authorization From Google Drive](https://tanaikech.github.io/2017/03/20/download-files-without-authorization-from-google-drive/)
- [How to use "fields" of Drive APIs](https://tanaikech.github.io/2017/03/30/how-to-use-fields-of-drive-apis/)
- [File Transfer for Google Drive Without Authorization](https://github.com/tanaikech/FileTransfer)
- [Converting PDF to TXT](https://gist.github.com/tanaikech/825f4b848a8cbff7018f71d33399e99b)
- [Retrieving Access Token for Google APIs](https://gist.github.com/tanaikech/247e4db66098e94f9e7da1b857f0a9be)
- [Downloading Files From Google Drive Under No Authorization Using Browser](https://gist.github.com/tanaikech/c5b2811bce01cbcc26ffa357df496379)
- [(NEW) Retrieve old revision file from Google Drive](https://gist.github.com/tanaikech/9ab6683e78de0044b4f670ff3761af19)
- [Get File List Under a Folder on Google Drive](https://gist.github.com/tanaikech/8e9b6fd667efcb483c9c742da9cd4e19)
- [Retrieving Access Token From OneDrive using Google Apps Script](https://gist.github.com/tanaikech/d9674f0ead7e3320c5e3184f5d1b05cc)
- [Interconversion Between Google Docs and Microsoft Docs](https://gist.github.com/tanaikech/8d639542577a594f6104b7f6fb753064)
- [Retrieving Files with Filename Included Special Characters using Google Apps Script](https://gist.github.com/tanaikech/e74ead2537b7b3718fc824b6ca60a531)
- [Selecting Files in Google Drive using Select Box for Google Apps Script](https://gist.github.com/tanaikech/96166a32e7781fee22da9e498b2289d0)
- [Uploading Local Files to Google Drive without Authorization using HTML Form](https://gist.github.com/tanaikech/2f16f467c94612dc83920a3158614d95)
- [Retrieving latest created file from PDF files on Google Drive](https://gist.github.com/tanaikech/0f452b2f951dddb57363dbb816487c33)
- [Downloading File Using Button of Dialog Box on Google Docs](https://gist.github.com/tanaikech/0f1fd11b7e4d45b016d45bbeeb06aa46)
- [Which of Drive API v2 or v3 is used for DriveApp.searchFiles()?](https://gist.github.com/tanaikech/242f644026837dd071f0ce95b2fd107a)
- [Resumable Conversion from CSV File with Large Size (> 50 MB) to Several Spreadsheets by Splitting File](https://gist.github.com/tanaikech/3e44c779f05374d19333444c9a4dd5ba)
- [Upload Files to Google Drive using Javascript](https://gist.github.com/tanaikech/bd53b366aedef70e35a35f449c51eced)
- [Enhanced makeCopy() using Google Apps Script](https://gist.github.com/tanaikech/ac1b0d50fe1ffaa40e95bbe9faf908b9)
- [Retrieving file list with folder structure under a specific folder in Google Drive](https://gist.github.com/tanaikech/4fca197b8ec45c8ac6300b1531c2489d)

<a name="projects"></a>
#### Projects
- [Retrieving ClientId using Google Apps Script](https://gist.github.com/tanaikech/4656b1b01128d27f291cee317553ea6d)
- [Copying and Overwriting GAS Project](https://gist.github.com/tanaikech/3e7608bd8ba87dd6019aedbd09224bd3)
- [Remove Third-party Apps with Account Access using Google Apps Script](https://gist.github.com/tanaikech/608e65fee105989df1a7b645c20572c2)
- [Retrieving Reformatted Scripts without Comments in a Project using Google Apps Script](https://gist.github.com/tanaikech/61f69fd2ce181865d3430c260c6a5d0b)

<a name="spreadsheets"></a>
#### Spreadsheets
- [Making charts at spreadsheet](https://tanaikech.github.io/2017/02/13/making-charts-at-spreadsheet/)
- [Download a CSV File from Spreadsheet Using Google HTML Service](https://tanaikech.github.io/2017/02/16/download-a-csv-file-from-spreadsheet-using-google-html-service/)
- [Send E-mail with Excel file converted from Spreadsheet](https://tanaikech.github.io/2017/02/16/send-e-mail-with-excel-file-converted-from-spreadsheet/)
- [Export CSV File from Spreadsheet and Make Download Button](https://tanaikech.github.io/2017/02/20/export-csv-file-from-spreadsheet-and-make-download-button/)
- [Creating Downloaded Excel file as Spreadsheet](https://tanaikech.github.io/2017/04/14/creating-downloaded-excel-file-as-spreadsheet/)
- [Creating Spreadsheet from Excel file](https://tanaikech.github.io/2017/04/15/creating-spreadsheet-from-excel-file/)
- [Converting Spreadsheet to PDF](https://tanaikech.github.io/2017/04/20/converting-spreadsheet-to-pdf/)
- [Overwriting Spreadsheet to Existing Excel File](https://tanaikech.github.io/2017/04/21/overwriting-spreadsheet-to-existing-excel-file/)
- [Retrieving User Information with Shared Spreadsheet](https://gist.github.com/tanaikech/a4a23d66134a900ddcb1652a4d420a58)
- [Embedding a Map to a Cell using Custom Function on Spreadsheet](https://gist.github.com/tanaikech/408f0eb58b18b08c4aa3783e5ee7463e)
- [Embedding Animation GIF in A Cell on Spreadsheet](https://gist.github.com/tanaikech/9b540220a9f408c05213c82e085c891a)
- [Search Route and Embedding Map using Custom Function on Spreadsheet](https://gist.github.com/tanaikech/e2d49b88b5d45cf2f26e6aaa14eafe91)
- [Pseudo Browser with Google Spreadsheet](https://gist.github.com/tanaikech/a290509e3d3f6997d248b88763fc69b9)
- [Retrieving Images on Spreadsheet](https://gist.github.com/tanaikech/d6594dc5c6c49a015c7d408c90e58bdc)
- [Converting a1Notation to GridRange for Google Sheets API](https://gist.github.com/tanaikech/95c7cd650837f33a564babcaf013cae0)
- [Retrieving Values By Header Title for Spreadsheet](https://gist.github.com/tanaikech/3036ee0199e2261f377aacbd7e458d1c)
- [Retrieving Spreadsheet ID from Range using Google Apps Script](https://gist.github.com/tanaikech/d4b033014c36c3506ad3ec38ce1eae4f)
- [Enhanced onEdit(e) using Google Apps Script](https://gist.github.com/tanaikech/73edaed1268a6d07118aed538aa5608d)
- [Measuring Execution Time of Built-In Functions for Google Spreadsheet](https://gist.github.com/tanaikech/1e7df0d6991d4e39330cd2b353573e72)
- [Retrieving Instance of User-Interface Environment](https://gist.github.com/tanaikech/f05e7d82b754b0348463b8dec1c741ad)
- [Automatic Recalculation of Custom Function on Spreadsheet](https://gist.github.com/tanaikech/b8ea7bd7fd87bcd7bb28ddede1781889)
- [Open Site with New Window using Google Apps Script](https://gist.github.com/tanaikech/9115c70eb83558d3af2eea656e4d9c67)
- [Append Values by Inserting Rows using Google Sheets API](https://gist.github.com/tanaikech/7846ebcafbab8318ff74c9955a99e06b)
- [Retrieves All Named Ranges in Spreadsheet as a1Notation](https://gist.github.com/tanaikech/aa744c9a15818c002d90eaea6b4efd03)
- [CLEAN method for Google Apps Script](https://gist.github.com/tanaikech/585597adda7954ba1cde3e724582bac5)
- [Retrieve Last of Specific Row and Column](https://gist.github.com/tanaikech/044d8651aed41c886f3379fdf5165aa2)
- [Parsing A1Notations using Google Apps Script](https://gist.github.com/tanaikech/c59b90324c90935b13f9e7b26cbf436a)

<a name="documents"></a>
#### Documents
- [Retrieving Number of Lines of Google Document](https://gist.github.com/tanaikech/37def8eeeaf7780bb99d3289ee32385e)
- [Replacing Text to Image for Google Document using Google Apps Script](https://gist.github.com/tanaikech/f84831455dea5c394e48caaee0058b26)

<a name="slides"></a>
#### Slides
- [Retrieving Size of Tables in Google Slides using Google Apps Script](https://gist.github.com/tanaikech/3143be7e7df8cc595d73427d22ae2e0e)

<a name="gmail"></a>
#### Gmail
- [How to Retrieve Replied Emails for Gmail](https://gist.github.com/tanaikech/a047e5f67f30b93482986039daa16dbc)
- [Adding a Label to a Message using Message ID for Gmail](https://gist.github.com/tanaikech/69c7daf910fdad0d6a296ea19f612089)

<a name="chart"></a>
#### Chart
- [Embedding a Chart to a Cell using Custom Function on Spreadsheet](https://gist.github.com/tanaikech/52da88484851ce2e0dea9881bf49f6fa)
- [Changing Line to Bars for Combo Chart using GAS](https://gist.github.com/tanaikech/bff89176cd269e392c45500274b40810)

<a name="slack"></a>
#### Slack
- [Changing Slack Status using Google Apps Script](https://tanaikech.github.io/2017/05/09/changing-slack-status-using-google-apps-script/)
- [Uploading Image Files to Slack Using Incoming Webhooks by Google Apps Script](https://gist.github.com/tanaikech/159cec05583c6f206e144f33b4042559)
- [Using Dialog Box of Slack by Google Apps Script](https://gist.github.com/tanaikech/c111f5560d21a07529e0da870af06a7d)

<a name="virtualcurrency"></a>
#### Virtual Currency
- [Bitfinex API for Google Apps Script](https://gist.github.com/tanaikech/1104d039341f198f95eee66af57c0abf)
- [Binance API for Google Apps Script](https://gist.github.com/tanaikech/175067567819577fd8eba9b82eabd1a6)
- [Bittrex API for Google Apps Script](https://gist.github.com/tanaikech/07fb768cf6d8256b3a72716a72e99f91)
- [Zaif API for Google Apps Script](https://gist.github.com/tanaikech/77481c2621dc7429449194c0f1dbd58c)
- [Cryptopia API for Google Apps Script](https://gist.github.com/tanaikech/58f092a544eb1cfbb19bc0252f36e4cb)

<a name="stackoverflow"></a>
#### Stackoverflow
- [Notifying Comments at Stackoverflow by Email using Google Apps Script](https://github.com/tanaikech/Notifying-Comments-at-Stackoverflow-by-Email)

<a name="netatmo"></a>
#### Netatmo
- [Notifying with email when Netatmo was down](https://github.com/tanaikech/Notifying-with-email-when-Netatmo-was-down)

<a name="etc"></a>
#### Etc
- [OCR using Google Drive API](https://gist.github.com/tanaikech/8c808bf8c060455fe5401ecacad07b94)
- [Multipart-POST Request Using Google Apps Script](https://gist.github.com/tanaikech/d595d30a592979bbf0c692d1193d260c)
- [Changing Values by Checking Duplicated Values of JSON for Javascript](https://gist.github.com/tanaikech/4c659fbb7cf8df0bc2c063dafa10e36c)
- [Straightening Elements in 2 Dimensional Array using Google Apps Script](https://gist.github.com/tanaikech/6a8b169cdcbda5a84f19964b81e447d9)
- [Batching Requests for Google Apps Script](https://gist.github.com/tanaikech/f167b9280a8e710804e4061571b53fb9)
- [Transposing JSON Object using Google Apps Script](https://gist.github.com/tanaikech/806fe728f8cf964078ef1354307a433d)
- [Retrieve Difference Between 2 Dimensional Arrays using Google Apps Script](https://gist.github.com/tanaikech/2abf57eefc667d6c71310db6aa95a44d)
- [About Updated Utilities.computeHmacSignature()](https://gist.github.com/tanaikech/9e9ab42ad225e127c59ae8ae598aacac)
- [Retrieving a Key with Maximum Value from Object](https://gist.github.com/tanaikech/fcbc0204e92d8f1cdde74dc5ac820753)
- [Adding Query Parameters to URL using Google Apps Script](https://gist.github.com/tanaikech/70503e0ea6998083fcb05c6d2a857107)
- [Retrieving Screen Shots of Sites using Google Apps Script](https://gist.github.com/tanaikech/a434b4ed50d91fe5f56fffcf6bcb3f78)

<a name="nodejs"></a>
#### Node.js
- [Downloading Files Under Specific Folder using Node.js](https://gist.github.com/tanaikech/38b536923b1765da052c21aab093649d)
- [Send mails from Gmail using Nodemailer](https://gist.github.com/tanaikech/d225c7adab818a6dc1dfd7783f8c8e4d)
- [Create Folder Tree of Google Drive using Node.js](https://gist.github.com/tanaikech/97b336f04c739ae0181a606eab3dff42)
- [Directly Using Access Token by googleapis for Node.js](https://gist.github.com/tanaikech/ca11c53356c5466e60109f79d9e4d9c9)

<a name="golang"></a>
#### Golang
- [spreadsheets.values.batchUpdate using Golang](https://gist.github.com/tanaikech/0f5b15fec7f409cdb568b0c2904fccb2)
- [Uploading CSV File as Spreadsheet and Modifying Permissions using Golang](https://gist.github.com/tanaikech/7ee103c80759a8297da198a5d1e92fc8)
- [Using String Values to []googleapi.Field for Golang](https://gist.github.com/tanaikech/27d27a1ac7fa99503e0737c28db53056)

<a name="python"></a>
#### Python
- [Updating Thumbnail of File on Google Drive using Python](https://gist.github.com/tanaikech/731c412c271828276bf3e24a25235aab)
- [Uploading Files From Local To Google Drive by Python without Quickstart](https://gist.github.com/tanaikech/8cdfd23807372657dc63d81e25e35153)

<a name="curl"></a>
#### Curl
- [File Upload and Download with File Convert For curl using Drive API](https://tanaikech.github.io/2017/02/08/file-upload-and-download-with-file-convert-for-curl-using-drive-api/)
- [Downloading Shared Files on Google Drive Using Curl](https://gist.github.com/tanaikech/f0f2d122e05bf5f971611258c22c110f)

[TOP](#TOP)
