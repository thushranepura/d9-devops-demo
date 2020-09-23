# Drupal 9 with Azure DevOps 

This is Drupal 9 configured  with AzureDevops  Build Pipelines  and Release Pipelines where deploying to master branch trigger a 
build and release to Azure Linux VM's Apache webroot

# Enviroment based Configuration Structure  

1. Azure pipeline variables attached to a Variable group (i.e Dev/QA/Prod)  are replaced in the settings.php  file at the release pipeline

2. Drupal's Enviormnet based configuration are refreshed based on Web Server Envriorment variables.

# Drupal modules used:

Configuration Split : https://www.drupal.org/project/config_split \
Drush CLI 

More info : https://www.drupal.org/docs/contributed-modules/configuration-split


Drupal Configuration directory structure

 ../config/ \
├── sync \
│    \
│    \
└── splits \
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── dev \
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│    \
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│    \
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;└── test 
        
