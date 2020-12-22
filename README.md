# Redirect-After-Theme-Activation
If you have special instructions in your theme (eg. in your theme options page) that you’d like the user to see when they first activate the theme, you can use the following function
# Add below code to your functions.php
    if (is_admin() && isset($_GET['activated']) && $pagenow == "themes.php")
      wp_redirect('themes.php?page=themeoptionstab');
# Note
Pay special attention to the wp_redirect() function. Make sure to replace the themes.php?page=themeoptions with the URL of your page.
