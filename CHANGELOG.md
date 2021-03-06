# EPS Release History

## 1.0.0 (2019-04-13)

 * Escape consecutive double quotes in EXPRESSIONs [Kenneth Cochran]
 * Add custom helper support [Jakub Pawłowski]

## 0.5.1 (2018-02-25)

 * Removed dead code (could not be called) [Dominique Broeglin]
 * Fixed #25 and other edge cases around literal `<%%` and `%%>` [Dominique Broeglin]

## 0.5.0 (2018-01-20)

 * Allow Get-OrElse to use pipeline input [Dominique Broeglin]
 * Improved README documentation [Dominique Broeglin]
 * Added test in context of #20 [Dominique Broeglin]
 * Added Get-OrElse function (optimized function loading when using -Safe) [Dominique Broeglin]
 * Better unit testing of the 'Each' helper function [Dominique Broeglin]
 * Allow relative path to 'Invoke-EpsTemplate -Path' [kimura wataru]

## 0.4.0 (2017-03-26)

 * Added an 'Each' function for iteration joining [Dominique Broeglin]

## 0.3.3 (2017-03-11)

 * Also fixed and issue when concatenating two code blocks [Dominique Broeglin]
 * #14 Fixed EOL trimming [Dominique Broeglin]
 * Optimized generated code (trimming spaces around code blocks)

## 0.3.2 (2017-01-27)

 * Fixed safe mode [Dominique Broeglin]
 * Added tests for the -safe paramter [Dominique Broeglin]
 * Meta tests should work on PS v2.0 too [Dominique Broeglin]

## 0.3.1 (2016-12-12)

 * Added module loading test and corrected PSM1 issue [Dominique Broeglin]
 * Added a note about backward compatibility [Dominique Broeglin]

## 0.3.0 (2016-12-09)

 * Ensure compatibility with PS 2.0 [Dominique Broeglin]
 * Alternative way to inject variables without changing current scope [Dominique Broeglin]
 * Refactored template engine to add multiline tags and trimming [Dominique Broeglin]
 * Added test for multiline expression tag [Dominique Broeglin]

Note: This release breaks backward compatibility to behave more like ERB:

 * No more output from a <% ... %> tags
 * No more line breaks added at the end of the template output
 * Refactored the cmdlet name to : Invoke-EpsTemplate

## 0.2.0 (2016-08-29)

 * Update README.md [Dave Wu]
 * Added proper escaping for ` and $ [Dominique Broeglin]
 * Fixed test suite when $A is defined [Dominique Broeglin]
 * Corrected style issues to satisfy Visual Studio Code [Dominique Broeglin]
 * Added PrivateData (re-encoded in UTF8) [Dominique Broeglin]
 * Changing base box name to eval-win2012r2-standard-nocm-1.0.4 [Dominique Broeglin]
 * Test various PowerShell versions with Appveyor. [Dominique Broeglin]
 * Added appveyor CI and corrected error on RootModule [Dominique Broeglin]
 * Update README.md [Dave Wu]
 * Aligning version number with upstream [Dominique Broeglin]
 * Reorganized the code in a more module like layout [Dominique Broeglin]
 * Update README.md [Dave Wu]
 * Cleaned up Vagrantfile and added provisioning [Dominique Broeglin]
 * Replaced EPS.ps1 by module EPS.psm1 [Dominique Broeglin]
 * Added a Vagrantfile to help developing on non Windows environment [Dominique Broeglin]

## 0.1.0 (2016-10-02)

 * First functional version
