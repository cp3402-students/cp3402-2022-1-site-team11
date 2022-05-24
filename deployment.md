Development of the new Townsville Jazz Club website will begin.

All files are to be managed and version controlled via Github, begin by pulling files from the repository
and preparing to link them to a local Wordpress development setup, using your preferred hypervisor such as Docker or Vagrant and your preferred IDE such as VSCode or PhpStorm.
In our group, we had different local setups for running WordPress. This was on account of the fact that each person had a different computer, and therefore had different requirements. Since the output of all these are simply wordpress files it was decided that identical local environments weren't needed.

   One hypervisor that was used was Mamp. Mamp was downloaded from https://www.mamp.info/en/downloads/  
   After that, the surver was set up, wordpress was installed, and the website was created.
   Docker was also used. XAMPP was another environment used by one member for local development.

A trello board was created to keep track of all tasks that need doing and manage the workflow. Tasks were assigned to each member at meetings to ensure that everyone knew what they had to do by the next meeting.

In local development the only automation done was using grunt for easy css editing via sass. All updates to the site were pushed to the shared github repo so team members could keep their local environments up to date at all times.

The staging site was set up on cloudaccess. Using FTP all files could be easily uploaded to the site for testing. The FTP info is easily visible on the cloudaccess control panel for ease of use.
   
Once things were finalised on the staging site, the plugin all-in-one WP migration was used to transfer everything over to the production site hosted on Azure. The transfer limit on this plugin is small so only the database and plugins were directly migrated this way. Media files were uploaded directly to Azure through the wordpress console.