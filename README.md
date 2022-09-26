# FOUC - Prevents Flash Of Unstyled Content

This module prevents flashing of unstyled content for projects which use critical.css and async CSS loading

## Installation

Assuming You have access to Growcode's 'Magento 2 Modules' project on bitbucket and that You are using composer based Magento installation You just need to:

1. Navigate to Your's project root directory and issue following commands:

   ```bash
   composer config repositories.growcode/module-fouc vcs git@bitbucket.org:conversion-ecommerce-development/growcode-module-fouc.git
   ```
   ```bash
   composer req growcode/module-fouc
   ```

2. You need to perform manual action in Backend -> Content -> Design -> Configuration -> here You need to choose desired scope and append following code:
   ```css
    <style type="text/css">
    .no-fouc {display: none;}
    </style>
   ```

under 'Other Settings' -> 'HTML Head' -> 'Scripts and Style Sheets' field. 

3. From the Magento root directory, run the `setup:upgrade` command to install and enable the module:

   ```bash
   bin/magento setup:upgrade
   ```
