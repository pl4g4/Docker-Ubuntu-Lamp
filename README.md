Docker-Ubuntu-lamp
=================

LAMP image (PHP+MySQL)

Usage
-----

To create the image, execute the following command:

	docker build -t pl4g4/ubuntu-lamp .

Running your LAMP docker image
------------------------------

Start your image binding the external ports 80 and 3306 in all interfaces to your container:

	docker run -d -p 80:80 -p 3306:3306 pl4g4/ubuntu-lamp

Working directory
-----------------

docker run -d -p 80:80 -p 3306:3306 -v /yourdirectory:/var/www/html/ pl4g4/ubuntu-lamp
