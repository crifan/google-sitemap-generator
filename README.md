# google-sitemap-generator

Crifan customized google-sitemap-generator (a WordPress plugin to generate sitemap) to support add customized link

* core update part
  * `sitemap-ui.php`
    ```php
    <?php $this->HtmlPrintBoxHeader('sm_paths',__('Additional paths', 'sitemap')); ?>

      <?php
      _e("Here you can specify folder/path/directory which should be included in the sitemap, but do not belong to your Blog/WordPress database.<br />such as http://www.crifan.com/files/doc/docbook/ which not belong to the site's wordpress database.<br />",'sitemap');

    ...
    ```
  * `lang/sitemap-zh_CN.po`
    ```bash
    "Last-Translator: crifan <admin@crifan.com>\n"

    #: D:\usr\www\wp-content\plugins\google-sitemap-generator/sitemap-ui.php:875
    msgid "Here you can specify folder/path/directory which should be included in the sitemap, but do not belong to your Blog/WordPress database.<br />such as http://www.crifan.com/files/doc/docbook/ which not belong to the site's wordpress database.<br />"
    msgstr "你可以在此处添加一些特殊的但并不存在于你 Blog/WordPress 的地址。<br />比如，http://www.crifan.com/files/doc/docbook/，其并不属于该wordpress网站的数据库。"
    ```

* Note
  * original (latest) Code: [XML Sitemap Generator for Google – WordPress plugin | WordPress.org](https://wordpress.org/plugins/google-sitemap-generator/)
