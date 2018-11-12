# CodePath-Assignments
# Project 7 - WordPress Pentesting

Time spent: **6** hours spent in total

> Objective: Find, analyze, recreate, and document **five vulnerabilities** affecting an old version of WordPress

## Pentesting Report

1. CVE 2015-5622 Wordpress 4.3 - Authenticated Shortcode Tags Cross-Site Scripting
  - [ ] Summary: 
    - Vulnerability types: XSS
    - Tested in version: 4.2
    - Fixed in version: 4.3.1
  - [ ] GIF Walkthrough: ![](https://github.com/Calberrycoder/CodePath-Assignments/blob/master/XSS%20%20ShortCode.gif)
  - [ ] Steps to recreate: 1) Use social engineering to gain access to post level permissions. 2) Create a new page/post or modify an existing one. 3) Use HTML editor to insert the following code: ![](https://github.com/Calberrycoder/CodePath-Assignments/blob/master/Shortcode.JPG)
  - [ ] Affected source code:
    - [Link 1](https://github.com/WordPress/WordPress/commit/f72b21af23da6b6d54208e5c1d65ececdaa109c8)
2. CVE 2015-5622 Wordpress 4.2.3 Stored Cross-Site Scripting
  - [ ] Summary: 
    - Vulnerability types: XSS
    - Tested in version: 4.2
    - Fixed in version: 4.2.3
  - [ ] GIF Walkthrough: ![](https://github.com/Calberrycoder/CodePath-Assignments/blob/master/Stored%20XSS.gif) 
  - [ ] Steps to recreate: 1)Utilize social engineering to gain access to admin console. 2)Create or modify new page/post. 3)Using HTML editor insert code like this: ![](https://github.com/Calberrycoder/CodePath-Assignments/blob/master/stored.JPG)
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/changeset/33359)
3. CVE 2017-6817: Authenticated Stored Cross-Site Scripting (XSS) in YouTube URL Embeds
  - [ ] Summary: 
    - Vulnerability types: XSS
    - Tested in version: 4.2
    - Fixed in version: 4.7.3
  - [ ] GIF Walkthrough: ![](https://github.com/Calberrycoder/CodePath-Assignments/blob/master/XSS%20YouTube.gif)
  - [ ] Steps to recreate: 1)Get access to an account with at least post level permissions utilizing social engineering 2)Create a new page or post/modifying existing. 3)Use HTML editor to embed code similar to this: ![](https://github.com/Calberrycoder/CodePath-Assignments/blob/master/yotube.JPG)
  - [ ] Affected source code:
    - [Link 1](https://github.com/WordPress/WordPress/commit/419c8d97ce8df7d5004ee0b566bc5e095f0a6ca8)
4. CVE 2016-7168: Authenticated Stored Cross-Site Scripting via Image Filename
  - [ ] Summary: 
    - Vulnerability types: XSS  
    - Tested in version: 4.2
    - Fixed in version: 4.2.10
  - [ ] GIF Walkthrough: ![](https://github.com/Calberrycoder/CodePath-Assignments/blob/master/XSS%20Word%20Press.gif)
  - [ ] Steps to recreate: 1)Utlize social engineering to gain access to admin console. 2)Create/Modify post or page. 3)Insert an "image" using HTML editor and code like this: ![](https://github.com/Calberrycoder/CodePath-Assignments/blob/master/image.JPG)
  - [ ] Affected source code:
    - [Link 1](https://sumofpwn.nl/advisory/2016/persistent_cross_site_scripting_vulnerability_in_wordpress_due_to_unsafe_processing_of_file_names.html)
5. (Optional) Vulnerability Name or ID
  - [ ] Summary: 
    - Vulnerability types:
    - Tested in version:
    - Fixed in version: 
  - [ ] GIF Walkthrough: 
  - [ ] Steps to recreate: 
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php) 

## Assets

List any additional assets, such as scripts or files: None used

## Resources

- [WordPress Source Browser](https://core.trac.wordpress.org/browser/)
- [WordPress Developer Reference](https://developer.wordpress.org/reference/)

GIFs created with [LiceCap](http://www.cockos.com/licecap/).

## Notes

The non XSS assignments required significant amounts of setup. 

## License

    Copyright [2018] [Cody Berry]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
