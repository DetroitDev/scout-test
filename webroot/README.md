# magento_exam

A test of basic Magento systems administration skills. By completing this exercise,
you will show basic competency in:
- RHEL-based Linux administration
- LEMP stack configuration
- Magento site administration
The exercise should take no more than 4 hours. The specific steps/requirements are
listed below, but fill in any gaps using your best judgement.

## Steps

__NOTE__: Record all commands used/steps taken in the configuration of this server and
          site, and check in to the repository with the filename `docs/commands.txt`. (Bonus
          points for configuring the server in the form of an Ansible script!) Make sure
          to note the Magento admin username/password.

1. Obtain the latest Magento 1.x Community Edition source code, and check in to this
  repository under the `webroot/` directory.
2. Connect to the server at XXX.XXX.XXX.XXX using SSH:
  - Username: root
  - Password: changeme
3. Install the latest versions of the server stack supported by Magento, including:
  - PHP+FPM
  - Nginx
  - MySQL
4. Configure an Nginx virtual host for a standard Magento 1.x website, using a
  self-signed SSL certificate for HTTPS support.
5. Create a dedicated Magento MySQL user and database.
6. Deploy the site code checked into the git repository in Step 1, and install it
  using the virtual host and MySQL user/database created in Steps 4 and 5. Ensure it
  can be reached at http://XXX.XXX.XXX.XXX/
7. Check in the [Aoe_Scheduler module](https://github.com/AOEpeople/Aoe_Scheduler),
  deploy to the server, and install.
8. Configure the Magento cron, using the recommended Aoe_Scheduler settings.
9. Prepare a dummy "t-shirt" configurable product (i.e., multiple sizes), and ensure
  it can be purchased through the frontend using the "Credit on Delivery" payment
  method.
10. Purchase a t-shirt, then cancel the order in the Magento admin.
11. Provide a brief, written explanation of the steps taken and why you chose to take
  them. Check this into the repository as `docs/explanation.txt`
