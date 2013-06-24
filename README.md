flask-mongo-app
===============

A Python Flask Web App Development Skeleton using mongoDB

I'm a n00b, just getting started on this to learn some tools, so bear with me as I piece all of this together.  Currently the system provisions itself and starts running the hello world flask app.  I'll tie in the db stuf and js one day...

Try it out!
-----------
*Bring up the virtualmachine and provision the server*

    $ vagrant up

_Point your browser at_

    http://localhost:5000/

_Cleaning up_

    $ vagrant destroy

_If you accidently delete the dir before doing destroy_

    $ VBoxManage list vms
    $ VBoxManage unregistervm flask-app-server –delete

####Requires:
* [Vagrant](http://www.vagrantup.com/) -- `sudo apt-get install vagrant`
* [VirtualBox](https://www.virtualbox.org/wiki/Downloads/) -- `sudo apt-get install virtualbox-4.2`

####Built On:
* [ansible](https://github.com/ansible/ansible/) -- provisioner loaded up first
* [Flask](http://flask.pocoo.org) -- Python microframework web app engine
* [mongoDB](http://mongodb.org) -- noSQL database
* [Flask-PyMongo](http://flask-pymongo.readthedocs.org/en/latest/) -- bridges Flask and PyMongo
* [leafletjs] (http://leafletjs.com/) -- javascript mapping
* [bootstrap] (http://twitter.github.io/bootstrap/) -- pretty css

####TODO:
* Javascript Charts & Graphs:
    * https://github.com/mbostock/d3/wiki/Gallery
    * http://square.github.io/crossfilter/ 
    * http://bl.ocks.org/tjdecke/5558084
    * http://www.chartjs.org/
    * http://www.flotcharts.org/flot/examples/
* Mapping:
    * http://maps.stamen.com/#toner/12/37.7706/-122.3782

####Issues:
* sometimes have to vagrant ssh && sudo supervisorctl start flask-mongo-app

####Notes:
* bootstrap.sh does a one-time install of ansible to get the ball rolling
* mongodb stores its data files in /var/lib/mongodb/
* mongodb stores its log files in /var/log/mongodb/

####My workflow:
* git config --global user.name 'Your Name'
* git config --global user.email your@email
* git pull
* edit some code
* git add <new files>
* git commit -am 'fixed some bugs'
* git push -u origin master

####Thanks to:
* http://www.pixelmonkey.org/2013/03/13/rapid-web-prototyping-with-lightweight-tools
* http://ryaneshea.com/lightweight-python-apps-with-flask-twitter-bootstrap-and-heroku

Contributing
------------

1. Fork it.
2. Create a branch (`git checkout -b my_markup`)
3. Commit your changes (`git commit -am "Added Snarkdown"`)
4. Push to the branch (`git push origin my_markup`)
5. Open a [Pull Request][1]
6. Enjoy a few plumphelmets while you wait

[1]: http://github.com/github/markup/pulls

