# phpmysql01
Testing purpose of PHP and MySQL code used in Openshift v3.11

**Step by step for installing this code into Openshift:**
- Create new project in openshift you can create from GUI or from CLI
- Create new app in the project
- Select image catalog and choose MySQL from catalog
- Use all as default (except if you want proper name for database), all user,pass will be generated from secret key, and then deploy the image
- Create new app and select PHP from image catalog
- Once created, go to deployment, and open ENVIRONMENT tab
- Add new environment from secret key, select mysql and input this key:
	- MYSQL_USER
	- MYSQL_PASSWORD
	- MYSQL_DATABASE