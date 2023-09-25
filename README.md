# Wordpress Template for OCP4 Catalog

How to use:
oc create -f wordpress-template.yml
oc process --parameters wordpress-nginx-php
oc process wordpress-nginx-php -p NAME=wordpress -p NAMESPACE=[YOU_PROJECT_NAME] -p ROUTER_CANONICAL_HOSTNAME=apps.your_domain.example -p MYSQL_ROOT_PASSWORD=nKatIcTRIToR -p MYSQL_PASSWORD=eSoiDenThicO | oc create -f -
