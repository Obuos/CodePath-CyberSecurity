# Project 7 - WordPress Pentesting

Time spent: **X** hours spent in total

> Objective: Find, analyze, recreate, and document **five vulnerabilities** affecting an old version of WordPress

## Pentesting Report

1. (Required) XSS Unauthenticated Genericons Cross-Site Scripting
  - [ ] Summary: 
    - Vulnerability types: XSS
    - Tested in version: 4.1
  - [ ] GIF Walkthrough: ![](https://gfycat.com/TartEnchantedGallowaycow)
  - [ ] Steps to recreate: 
        Add <img src=1 onerror="alert(1)" /> to the end of the url: wp-content/themes/twentyfifteen/genericons/example.html#1
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)
1. (Required) XSS Authenticated Cross-Site Scripting with Media Files
  - [ ] Summary: 
    - Vulnerability types: XSS
    - Tested in version: 4.2.3
  - [ ] GIF Walkthrough: ![](https://gfycat.com/OrnateFluffyDeinonychus)
  - [ ] Steps to recreate: 
        Download mp3 file from source below
        Upload mp3 file to WP Media
        Insert a playlist with the mp3 file into a post
  - [ ] Affected source code:
    - [Link 1](https://sumofpwn.nl/advisory/2016/wordpress_audio_playlist_functionality_is_affected_by_cross_site_scripting.html)
1. (Required) XSS Authenticated Cross-Site Scripting
  - [ ] Summary: 
    - Vulnerability types: XDD
    - Tested in version: 4.0
  - [ ] GIF Walkthrough: ![](https://gfycat.com/ValuableInbornBrant)
  - [ ] Steps to recreate: 
        Make a comment on a post using a link
        Add an alert script at the end of the link: svg onload=alert(1)
  - [ ] Affected source code:
    - [Link 1](https://wpvulndb.com/vulnerabilities/8358)

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
