# Simpler-Released

## Overview
Simpler is a tool which helps you to translate your CAIE IGCSE Pseudocode into actually Python Code

## Installation
1. Go to the [Releases Page](https://github.com/shixingzeya/Simpler-Released/releases). 
2. Download the latest version of Simpler execludable file for your operating system

## Anti-Virus Setting
Since the public testing version of Simpler is not assigned a DSA certificate, the system's anti-virus application or other anti-virus applications downloaded on your computer may refuse to open Simpler or attempt to delete the execludable file of Simpler. Your will need to temporarily disable these anti-virus applications to download and execute Simpler. This problem may soon be recovered after the releasing of the official version of Simpler

## Usage
1. Execute the execludable file downloaded in the [Installation Section](#installation) (MacOS users may need to decompress the `.zip` file firstly)
2. Choose or type in the path of the `.cpc` file CAIE IGCSE Pseudocode 
3. Click the run button
4. A file with the same of the `.cpc` file will be created under the same directory of it, but with a suffix of `.py`. The translated Python content will be stored in this `.py` file

## Status
This project is still in developing stage. Unexpected errors may occur during using. If you meet any problem during using, please report the problem according to [Issue Section](#issue).

Some functions have not been implemented currently. However, we are devoting to implement these functions as soon as possible, and these functions may soon be available in future versions. 

1. Nesting functions is not currently supported  
   For example:  
   `SUBSTRING(UCASE(my_string), 2, 5)`

2. File managing statements are not currently supported  
   For example:
   ```
   OPENFILE "abc.txt" FOR READ
   READFILE "abc.txt", file
   CLOSEFILE "abc.txt"
   ```

## Log Entries

### [March 03, 2025] - v0.1-alpha 
Initial project setup and core functionality.  

### [March 06, 2025] - v0.2.0
The first official public testing version  

* Added: Support for `RAND()` and `INT()` functions.
* Changed: Refactored `<-` handler for better compatibility
* Fixed: The bug that `CASE OF` indenting incorrectly
* Fixed: The bug that 2D Array handler functions in some unexpected situations
* Fixed: The bug that `OUTPUT` handler behaves wrongly

### [March 07, 2025] - v0.2.1
Fix several bugs existed in [v0.2.0](#march-06-2025---v020)

* Fixed: The bug that `FOR` loop behaves wrongly
* Fixed: The bug that substatements are not translated in `FOR` loop statement
* Fixed: The bug that `<-` handler fails in some situations

### [March 11, 2025] - v0.2.2
Fix several bugs existed in [v0.2.1](#march-07-2025---v021), add some functions

* Added: Translate-time detection for whether all the complex statements are enclosed
* Changed: Updates the GUI
* Fixed: The bug that `SUBSTRING` handler sometimes triggers unexpected errors

### [March 12, 2025] - v0.2.3
Add support to `REPEAT UNTIL` loop

* Added: Handler for `REPEAT UNTIL` loop

### [March 13, 2025] - v0.2.4
Fix a bug existed in [v0.2.3](#march-12-2025---v023)

* Fixed: The bug that `REPEAT UNTIL` loop behaves wrongly

### [March 26, 2025] - v0.3.0
Updates the main interface and change several implement

* Added: Night mode for the main interface
* Changed: Updates the GUI
* Changed: Refactored general `DECLARE` handler

## Issue
If you encounter a problem or find that the translation includes unexpected results, please open an issue in the [Issue Page](https://github.com/shixingzeya/Simpler-Released/issues), report and explain the problem you encountered. This will help us improve Simpler and make it even better. We deeply appreciate your efforts and contribution to Simpler

## Future Plans
1. Implement handler for nesting functions
2. Add support to file managing statements
3. Add support to A Level CAIE Pseudocode