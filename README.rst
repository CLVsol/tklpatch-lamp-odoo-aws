tklpatch-lamp-odoo-aws
======================

This project will help you install **PostgreSQL** over a `TurnKey LAMP <http://www.turnkeylinux.org/lamp>`_ appliance, using the Amazon Web Services (AWS) EC2 infrastructure.

#. Apply the patch "clvsol_tklpatch-lamp-odoo-aws":

	::

		cd /root
		tklpatch-apply / clvsol_tklpatch-lamp-odoo-aws

#. Change manually, using Webmin, the passwords for the accounts:

	* postgres (Linux)
	* postgres (PostgreSQL)
	* openuser (PostgreSQL)

#. Change manually, editing the Odoo configuration files (/opt/openerp/odoo/**openerp-server.conf**, /opt/openerp/odoo/**openerp-server_man.conf**), the passwords for the accounts:

	* openuser (account on PostgreSQL - db_password)
