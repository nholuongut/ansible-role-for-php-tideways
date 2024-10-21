# Ansible Role: PHP-Tideways

![](https://i.imgur.com/waxVImv.png)
### [View all Roadmaps](https://github.com/nholuongut/all-roadmaps) &nbsp;&middot;&nbsp; [Best Practices](https://github.com/nholuongut/all-roadmaps/blob/main/public/best-practices/) &nbsp;&middot;&nbsp; [Questions](https://www.linkedin.com/in/nholuong/)
<br/>

Installs the [Tideways PHP Profile Extension](https://github.com/tideways/php-xhprof-extension) on Linux servers.

## Requirements

None.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

    workspace: /root

Where Tideways setup files will be downloaded and built.

    tideways_download_url: https://github.com/tideways/php-xhprof-extension/archive/master.zip
    tideways_download_folder_name: php-xhprof-extension-master

The URL from which Tideways will be downloaded, and the resulting folder into which it is downloaded.

    tideways_extension_name: tideways_xhprof.so

The extension name for the Tideways PHP extension.

    tideways_api_key: ''

If you use the Tideways UI, set this variable to your API key. Otherwise the extension can be used along with the XHProf UI to view profiles.

    tideways_install_xhprof_ui: true

Tideways data-format is 100% compatible with XHProf so you can use the XHProf UI to browse profiles reports and the `XHProfRuns_Default` class to write the profile data to disk. If you use the Tideways UI, set this variable to `no`.

    xhprof_download_url: https://github.com/phacility/xhprof/archive/master.tar.gz
    xhprof_download_folder_name: xhprof-master

The URL from which XHProf will be downloaded.

    php_xhprof_lib_dir: /usr/share/php/xhprof_lib

Directory where the XHProf PHP library is stored.

    php_xhprof_html_dir: /usr/share/php/xhprof_html

Directory where the XHProf UI is stored.

## Dependencies

  - nholuong.php

## Example Playbook

    - hosts: webservers
      roles:
        - nholuong.php-tideways

# 🚀 I'm are always open to your feedback.  Please contact as bellow information:
### [Contact ]
* [Name: nho Luong]
* [Skype](luongutnho_skype)
* [Github](https://github.com/nholuongut/)
* [Linkedin](https://www.linkedin.com/in/nholuong/)
* [Email Address](luongutnho@hotmail.com)

![](https://i.imgur.com/waxVImv.png)
![](Donate.png)
[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/nholuong)

# License
* Nho Luong (c). All Rights Reserved.🌟
