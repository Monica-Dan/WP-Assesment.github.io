[New Text Document.txt](https://github.com/Monica-Dan/WP-Assesment.github.io/files/8196778/New.Text.Document.txt)
# Author: Monica Danial
# Description: I have created a Wordpress woocommerce store with products that have two new attributes showing up under each product on the shop page using local server             application: WordPress, WooCommerce and the default 2021 / 2022 Theme.

# Steps of downloading the server, database, and create the child theme:
Dowenload and install a local server, I used WampServer.
Dowenload WordPress from wordpress.org and follow steps to install it.
Create the database from the WAMP server (go to PhPMyAdmin). I created my database under monicadb.
continue installing WordPress after adding some information like username, password, and email.
Now, you will be able to open your WordPress dashboard and the Twenty-Twenty-Two theme is active.
In order to modify the theme, we should create a Child Theme.
install Child Themify plugin in Wordpress and create the Twenty Twenty Two child theme to make some changes.
Then, Install the Woocommerce plugin from the plugins section and activate it.
I used the dummy products from Woocommerce to display some products.
Inside the Products in the left menu I selecte attibutes to adde two attributes for the products like(color & size).
Install Variation Swatches for WooCommerce plugin to show the color in different way.
In order to show the size and the color attributes under the products, go to Twenty Twenty Two Child function.php file.
Inside the Twenty Twenty Two Child function.php file use the hook (add_action)

# Steps to write the code:
Use the hook tool like add_action to perform functions (actions) in specific places of the theme.
add_action accepts at least two parameters. First parameter is the hook (required), in this case we use 'woocommerce_after_shop_loop_item_title' to specify the action. 
The second parameter will be the call back function (required), which is the name of the function we want to be hooked, in our case we use 'display_product_size'.
The Third parameter is the priority (optional), whish is used to specify the order in which the functions associated with a particular action are executed.
Declare the “global $product” inside the function.
Create a size variable to get the size attribute.
Make an if condition to check if there is size attribute and show its div on the page.
Apply the previous logic of hooking the size to the color attribute but change the call back function name, the priority parameter, and the if condition parameter.

# Steps to upload the files and database.
create a new repository on github, I created two repositories:
https://github.com/Monica-Dan/WP-Assesment.github.io  This repository to upload the database, and I used (Git LFS) with some command lines to be able to upload the large files.
https://github.com/Monica-Dan/WP-assesment-2 This repository to upload the themes files because the first one is over its data quota, and I used the Github desktop programe to commit and push the files. 








