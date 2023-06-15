# FOUC - Prevents Flash Of Unstyled Content

This module prevents flashing of unstyled content for projects which use critical.css and async CSS loading

## Installation

1. Navigate to Your's project root directory and issue following commands:

   ```bash
   composer config repositories.growcode/module-fouc github git@github.com:grwcd/growcode-module-fouc.git
   ```
   ```bash
   composer req growcode/module-fouc
   ``` 

2. From the Magento root directory, run the `setup:upgrade` command to install and enable the module:

   ```bash
   bin/magento setup:upgrade
   ```
