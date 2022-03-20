# SimpleSAMLphp module RedIRIS skin

This is a twig-only SimpleSAMLphp theme used for the RedIRIS identity provider.

The theme does not support a language menu yet (although supports translated strings).

This code is released under a Creative Commons Zero v1.0 Universal license. 

The repository contains different logos that are trademarks, and images under creative commons license, whose authors are listed in the CREDITS file.

## Install

1. Drop the folder in your SimpleSAMLphp `modules` folder.

2. Edit `config.php` and be sure to uncomment/add these lines:

```
    'theme.use' => 'theme-rediris:RedIRIS',
    'usenewui' => true,    
```

3. Copy your institution logo under these paths:

   -  `simplesamlphp-module-skin-rediris/www/assets/images/logo.svg` is the organization logo in full color
   -  `simplesamlphp-module-skin-rediris/www/assets/images/logo-white.svg` is the organization logo in white, to be used on top of a darker color.

4. Edit the following files, to fit your organization color:

   - `simplesamlphp-module-skin-rediris/www/assets/css/main.css` 

5. Finally, do any changes to the login skin under this file:

   - `simplesaml-module-skin-rediris/themes/RedIRIS/core/loginuserpass.twig`

This probably includes changing the vegas slider images, near the end of the file.

You can also add a link to the tool to recover credentials, if you have one, just uncomment and modify the relevant lines.
