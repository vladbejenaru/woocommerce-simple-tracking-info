# woocommerce-simple-tracking-info
Wordpress / Woocommerce plugin for adding tracking info to orders in a simple way

as of 28.01.2018

INTRODUCTION:
The plugin intends to be a very simple one without integration with shipping partners and so on. As shop manager you will have the possibility to add traking info for the order (at this moment one traking info per order) and to send this info to the customer.
At this moment the plugin is not "soft customizable" with a lot of information hardcoded: shipping partners, the way how the direct traking link is handled, text that is included in the email to the customer.

Please excuse my coding style, I am new to this and still learning!


WHAT THE PLUGIN DOES:
1. Inside woocommerce orders on the dashboard you can specify the shipping partner, tracking number and tracking link for the order. (at this moment only one set of info per order)
2. In the confirmation email sent to the customer the traking info (based on the information filled in in the order) is sent to the customer. The paragraph with the shipping info is included only when (minimum) a traking number is defined in the order

3. (to do) In the order view page (on customer side), the traking information is displayed.


TO DO LIST:
1. add traking info in the order diplay page (my account -> orders -> view)
2. build plugin settings page including:
  - definition of shipment partners: Name, traking link, direct traking link logic
  - definition of the shipping info text that will be used in the customer email and on the orders page
  
INSTALLATION:

Download zip file and install it as a new wordpress plugin.

CUSTOMIZATION:

The main actual subject of customization is the message sent to the customer. Edit with a text editor the main file and customize your message inside add_trackinginfo_to_email($order) function (starting on line 84 in woocommerce-add-tracking-info.php).
Basic HTML, PHP knowledge is required.
