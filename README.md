# Seattle GiveCamp WordPress Docker Image

Simple WordPress development environment to help Seattle GiveCamp volunteers get up and running quickly.

Visit our website at:

http://seattlegivecamp.org

## How to access site files

Website files live in the `html` folder

MySQL databases live in the `mysql` folder

## Quick Start

- Install Docker: https://docs.docker.com/get-docker/
- Clone the repository: `git clone git@github.com:SeattleGiveCamp/seattle-givecamp-wordpress-docker.git`
- Bring up the environment: `docker-compose up`

## Full install instructions

Here are details instructions that will get your environment up and running. 

_Important Note:_ This development environment requires ports 80 and 3306 be available. If there is another service running on your machine it will need to be stopped before starting this environment.

### Install Docker

Docker is a container engine- essentially software that runs mini-computers inside of yours. These mini-compupters are called containers.

The Docker manual contains full instructions to get Docker installed and running. The manual can be found at: https://docs.docker.com/get-docker/

### Install Docker Compose

Docker Compose is an easy to use Docker orchestration tool. Most likely it was installed with Docker, however in the case you need to install it manually you may do so at https://docs.docker.com/compose/install/

### Get the development environment

Next up is getting a copy of the development environment locally. That is the files in this repository. Use your favorite too to clone the repository, or download the ZIP archive.

### Bring up the development environment

Finally, time to fire up the site! 

It is easiest to use the Terminal app to start the Docker environment.

- Open Terminal
- `cd` to the directory containing the development environment
- Run `docker-compose up`

E.G. - Given the development environment is on a Mac and the Desktop folder:

Open Terminal
`cd ~/Desktop/seattle-givecamp-wordpress-docker`
`docker-compose up`

### Access the site

The running site can be accessed at http://localhost

### Adding a domain

If you would like to use a domain with your development environment, simply add the domain to the system hosts file.

On a Mac:
- Edit `/etc/hosts`

On Windows:
- Edit `C:\Windows\System32\Drivers\etc\hosts`

Add the following line:
`127.0.0.1 	MYSITEDOMAIN.COM`

### Accessing the database

Direct database access is available on `localhost` via port `3306`

User: `root`
Password: `SeattleGiveCampRocks1!`

**PLEASE NOTE:** The database password is hardcoded into this development environment. _DO NOT_ deploy the site without changing the password to something secure and non-public!

### DEVELOP! 

All the site files can be found in the `html` folder. Edit to your hearts content!

### Deploying to the non-profit's server

When you are ready to deploy code to the non-profit's server, consult your team's tech lead for deployment information.

# Qeustions?

Reach out to Ben Lobaugh or Josh Holmes via Microsoft Teams
