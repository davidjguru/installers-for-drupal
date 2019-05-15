# Installers For Drupal 
Installers For Drupal is a collection of craft scripts  for launch various types of processes creating environments and installing a Drupal ready-to-work codebase. 


## Recipe 1: Angular & Drupal & DDEV
1. *Resource:* /installers/install_angular_drupal_ddev
2. *Description:* Download and install a Drupal codebase project inside a new environment based in docker - ddev with node, npm, Angular and Drupal 8. 
3. *Use:* Just for create Debian - based environments to work in Drupal - Headless projects (In this case, using Angular for the frontend). 
4. *Characteristics:* 
- Search for older versions of Docker and uninstall it.
- Stop your Apache main server, to free the port 80. 
- Update your package list.
- Install all the basic resources in your host system: docker-ce, docker.compose, linuxbrew and ddev.
- Create a new ddev environment with containers for Drupal, database, etc. (See 5 to see the container specifications). 
- Build a new Drupal-based project using ddev, Composer and Drush. 
- Install and enable some basic modules needs to work like devel, webprofiler, admin_toolbar and masquerade. 
- Install some more packages in the container: sqlite3, node, npm and Angular. 
- Open the new Drupal in Browser and goes to the container prompt. 
- Ready to work. 
5. *Specifications:*
 - OS in Container: Debian 9.8 Stretch
 - PHP in Container: 7.3.3
 - Apache in Container: 2.4.25
 - Database: MariaDB, version 10.2.22
 - Node in Container: 8.15.1
 - npm in Container: 6.4.1
 - Angular CLI in Container: 7.3.9
 - TypeScript in Container: 3.2.4
 6. *Important:*
 - Be aware with the prompt, It's possible that the script ask you for something like the name of the project and other stuff. 
