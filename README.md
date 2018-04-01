# Project 7 - WordPress Pentesting

Time spent: 5 hours spent in total

> Objective: Find, analyze, recreate, and document **five vulnerabilities** affecting an old version of WordPress

## Pentesting Report

1. Vulnerability Name or ID: Authenticated Stored Cross-Site Scripting (XSS) in YouTube URL Embeds
  - [X] Summary: An embedded YouTube link with a script in the URL creates a XSS attack
    - Vulnerability types: XSS
    - Tested in version: 4.2
    - Fixed in version: 4.2.13
  - [X] GIF Walkthrough: <img src="https://github.com/mattcc1398/CodePath-Week7/blob/master/YouTube%20XSS.gif" width="800">
  - [X] Steps to recreate: Embed a YouTube link with XSS in a page or post. Update/post the changes, and then view the post/page. A XSS alert will appear once the page or post is opened.
  - [X] Affected source code:
    - https://github.com/WordPress/WordPress/commit/419c8d97ce8df7d5004ee0b566bc5e095f0a6ca8
 
2. Vulnerability Name or ID: Authenticated Shortcode Tags Cross-Site Scripting (XSS) 
  - [X] Summary: A XSS attack is executed upon hovering the mouse over a caption
    - Vulnerability types: XSS
    - Tested in version: 4.2
    - Fixed in version: 4.2.5
  - [X] GIF Walkthrough: <img src="https://github.com/mattcc1398/CodePath-Week7/blob/master/Shortcode%20tags.gif" width="800">
  - [X] Steps to recreate: Embed a caption with a link that contains an onMouseOver script. Upload the post, and upon hovering over the caption a XSS alert will appear. 
  - [X] Affected source code: 
    - https://blog.checkpoint.com/2015/09/15/finding-vulnerabilities-in-core-wordpress-a-bug-hunters-trilogy-part-iii-ultimatum/
3. Vulnerability Name or ID: Unauthenticated Genericons Cross-Site Scripting (XSS)
  - [X] Summary: Embedding a link to 2015 genericon theme with a script in the URL allows for a XSS attack
    - Vulnerability types: XSS
    - Tested in version: 4.2 
    - Fixed in version: 4.2.2
  - [X] GIF Walkthrough: <img src="https://github.com/mattcc1398/CodePath-Week7/blob/master/Theme%20XSS.gif" width="800">
  - [X] Steps to recreate: Embed a link to a 2015 generic theme with a script in the URL. Once the page is posted, a XSS alert will appear when it is opened. 
  - [X] Affected source code:
    - https://codex.wordpress.org/Version_4.2.2

## Resources

- [WordPress Source Browser](https://core.trac.wordpress.org/browser/)
- [WordPress Developer Reference](https://developer.wordpress.org/reference/)

GIFs created with [LiceCap](http://www.cockos.com/licecap/).


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
