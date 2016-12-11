## AYNY Deployment

- Requires Ansible 2
- OS : Ubuntu 14

These playbooks deploy an AYNY stack which contains Nodejs, Sails, Nginx, php-fpm, MongoDB and Odoo.

Then run the playbook, like this:

	ansible-playbook -i hosts site.yml

The playbooks will configure MySQL, WordPress, Nginx, and PHP-FPM. When the run
is complete, you can hit access server to begin the WordPress configuration.

### Ideas for Improvement

Here are some ideas for ways that these playbooks could be extended:

- Parameterize the WordPress deployment to handle multi-site configurations.
- Separate the components (Nodejs, MongDB, Nginx) onto separate hosts and 
handle the configuration appropriately.

We would love to see contributions and improvements.