sudo /etc/init.d/apache2 restart
sudo /etc/init.d/elasticsearch restart

php composer.phar create-project --repository-url=https://repo.magento.com/ magento/project-community-edition=2.4.6 TestMagento246

===> Install command<====

# first check if elastic server is installed 
# using curl elastic-server-ip:port
# for example
curl localhost:9200
# will output server info if started otherwise start the server

# now download Magento2.4 using composer
mkdir DIRECTORY_WHERE_YOU_WANT_TO_INSTALL
cd DIRECTORY_WHERE_YOU_WANT_TO_INSTALL
composer create-project --repository-url=https://repo.magento.com/ magento/project-community-edition:2.4.0 .

Adobe commerce 

php ../composer.phar create-project --repository-url=https://repo.magento.com/ magento/project-enterprise-edition=245 <install-directory-name>



# after downloading Magento now use below command to install it 
php bin/magento setup:install --base-url=http://localhost/mage246/TestMagento246/pub/ \
--db-host=localhost --db-name=TestMagento246 --db-user=root --db-password=Saark@1992 \
--admin-firstname=Magento --admin-lastname=User --admin-email=user@example.com \
--admin-user=admin --admin-password=admin123 --language=en_US \
--currency=USD --timezone=America/Chicago --use-rewrites=1 \
--search-engine=elasticsearch7 --elasticsearch-host=localhost \
--elasticsearch-port=9200 --backend-frontname=admin
# now your magento is ready for development


php bin/magento module:disable Magento_AdminAdobeImsTwoFactorAuth  Magento_TwoFactorAuth

php bin/magento module:disable Magento_TwoFactorAuth


===>Rabbit Mq<====

http://localhost:5672/#/  (url)

Installation guide

sudo apt install -y rabbitmq-server

rabbitmq-plugins enable rabbitmq_management

Then you need to go to http://127.0.0.1:5672/ and login with default data: guest/guest. Or you can make an ssh tunnel for remote access:

ssh -L 5672:localhost:5672 user@remote.host


=================================
Stop Commands

sudo service apache2 stop
sudo service elasticsearch stop
sudo service rabbitmq-server stop
sudo service mysql stop


mysqldump -hdatabase.internal -uuser -p --single-transaction main | gzip > var/main.sql.gz

scp jjjo5g63c52zc-integration-5ojmyuq--mymagento@ssh.az-westeurope-1.magento.cloud:/app/var/main.sql.gz  .
@collapsible-nav-background: @sidebar__background-color;
@collapsible-nav-item-hover: @color-gray91;

php ../composer.phar global config http-basic.repo.magento.com 5a1b1da2df8dcf00f829b7e409181ee3 4f8aa70450d47a06430dc2a9ebb955b7


php ../composer.phar  global config http-basic.repo.magento.com d44d53e337ed642d5c6ebfa11bf48c06 8430b6053ec934f4af83a13e170df006


https://confluence.atlassian.com/bbkb/the-authenticity-of-host-bitbucket-org-104-192-143-1-can-t-be-established-1168865389.html


EMPTY CLSER IN ELASTIC SEARCH 

curl -X DELETE 'http://localhost:9200/_all'


/home/medline/www/html


https://www.autify.co.uk/blog/how-to-install-magento-2-on-ubuntu/#:~:text=1%20Step%201%3A%20Enable%20the%20Windows%20subsystem%20for,Step%208%3A%20Install%20Magento%202%20...%20More%20items

Ensure you have +x on all of the directories in the path leading to the site's root. For example, if the site root is /home/username/siteroot:

sudo chmod +x /home/
sudo chmod +x /home/magento
sudo chmod +x /home/magento/www/
sudo chmod +x /home/magento/www/html

sudo systemctl restart nginx.service

sudo /etc/init.d/elasticsearch restart
sudo /etc/init.d/apache2 restart

sudo chmod -R 777 pub/* generated/ var/

https://www.youtube.com/watch?v=2GD4BR8F77g

gzip -d file.gz

https://devdocs.mage-os.org/docs/main/cache-management

https://webkul.com/blog/php-unit-test-in-magento-open-source/

https://webkul.com/blog/php-unit-test-in-magento-open-source/
