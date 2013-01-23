tbx_theme
=========

d7 sky subtheme


http://adaptivethemes.com/documentation/footheme

However, if you want to subtheme Pixture Reloaded or Sky, or you really want to change the name from Footheme, then read on.

Copy this entire theme and change the name of the folder. Currently the name of the folder is "footheme", so you might choose "bartheme". In the next step we will use this name for the info file so this is very important because as far as Drupal is concerned the name of the info file is the "machine name" of your theme. Don't use spaces or any punctuation other than underscores. E.g "bar_theme" is OK, but "bar theme" is not OK.
footheme.info - first rename this file to match the folder name you chose in step one. Next you can change the "name", "description" and "version" to whatever you want. Then you need to copy and paste in some stuff from your base themes info file - the "regions list" and "theme settings list" from your chosen base theme. The ones there now are from Corolla so just replace them. If you're using Corolla then you can do nothing, or just change the name and description.
Color module stuff - using Corolla? No issue, do nothing. If you're using Pixture Reloaded or Sky then you need to delete the color folder from this theme and copy/paste in the color folder from your chosen base theme.
Pixture Reloaded uses images as part of the color process - they are all in the /images folder in Pixture Reloaded - you should copy and paste that folder in as well.

template.php - open up this file and make some changes - search and replace "footheme" for your themes name.
In footheme_preprocess_html() you will find some stuff about responsive stylesheets and IE conditional stylesheets - follow those instructions carefully - they are easy and involve renaming some CSS files to match your theme name.