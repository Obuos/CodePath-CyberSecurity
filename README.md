# Project 7 - WordPress Pentesting

Time spent: 4 hours spent in total

> Objective: Find, analyze, recreate, and document **five vulnerabilities** affecting an old version of WordPress

## Pentesting Report

1. (Required) XSS Unauthenticated Genericons Cross-Site Scripting
  - [x] Summary: 
    - Vulnerability types: XSS
    - Tested in version: 4.1
  - [x] GIF Walkthrough: ![](https://github.com/Obuos/CodePath-CyberSecurity/blob/master/week7a.gif)
  - [x] Steps to recreate: 
        
       Add xss code to end of the url
        
        <img src=1 onerror="alert(1)">
        
       Use url: wp-content/themes/twentyfifteen/genericons/example.html#1
  - [x] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)
2. (Required) Large File Upload Error
  - [x] Summary: 
    - Vulnerability types: XSS
    - Tested in version: 4.2.2![](https://github.com/Obuos/CodePath-CyberSecurity/blob/master/week7b.gif)
  - [x] Steps to recreate: 
        Make a file over 20mb and name it Dinosaurs secret life img src=x onerror=alert(1)>.png
        Upload file into media
  - [x] Affected source code:
    - [Link 1](https://hackerone.com/reports/203515)
3. (Required) User Enumeration
  - [x] Summary: 
    - Vulnerability types: User Enumeration from User Login
    - Tested in version :4.7.1
  - [x] GIF Walkthrough: ![](https://github.com/Obuos/CodePath-CyberSecurity/blob/master/week7c.gif)
  - [x] Steps to recreate: 
        Use login id: admin and any password; the system will say the password for user is incorrect
        Use login id: joe and any password; the system will say invalid username
  - [x] Affected source code:
    - [Link 1](https://www.exploit-db.com/exploits/41497/)

## Assets

List any additional assets, such as scripts or files

## Resources

- [WordPress Source Browser](https://core.trac.wordpress.org/browser/)
- [WordPress Developer Reference](https://developer.wordpress.org/reference/)

GIFs created with [LiceCap](http://www.cockos.com/licecap/).

## Notes

Describe any challenges encountered while doing the work

## License

    Copyright [yyyy] [name of copyright owner]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
