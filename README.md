# Codepath-Security-Week-7
Week 7 Project: WordPress vs. Kali

# Challenge 7
# WordPress 2.5-4.6 - Authenticated Stored Cross-Site Scripting via Image Filename

WordPress version tested in: 4.2.2
Vulnerability type: XSS

Steps in order to recreate:
1) Rename an image to have the following name img src= a onerror= alert(document.cookie) .jpg
2) Upload the image to WordPress
3) Create a post and add this image into the post
4) Change the attachment display settings to "Attachment page"

GIF Walkthrough:
https://gfycat.com/gifs/detail/PastDishonestLeafbird

Source:
https://sumofpwn.nl/advisory/2016/persistent_cross_site_scripting_vulnerability_in_wordpress_due_to_unsafe_processing_of_file_names.html

# Vulnerability 1
# WordPress 3.3-4.7.4 - Large File Upload Error XSS

WordPress version tested in: 4.2.2
Vulnerability type: XSS

Steps in order to recreate:
1) Find/create a file and name it Dinosaurs secret life img src=x onerror=alert(1)>.png
2) Go to add media and try to upload this file into media

GIF Walkthrough:
https://gfycat.com/gifs/detail/BlindBlindBellsnake

Source:
https://hackerone.com/reports/203515

# Vulnerability 2
# WordPress 3.6.0-4.7.2 - Authenticated Cross-Site Scripting (XSS) via Media File Metadata

WordPress version tested: 4.2.2
Vulnerability type: XSS

Steps in order to recreate:
1) Download the xss.mp3 file from the source located in source.
2) Upload that mp3 file into WordPress media.
3) Create a post and insert a playlist into the post containing the xss.mp3 file

GIF Walkthrough:
https://gfycat.com/gifs/detail/WhirlwindRealisticHochstettersfrog

Source: 
https://sumofpwn.nl/advisory/2016/wordpress_audio_playlist_functionality_is_affected_by_cross_site_scripting.html


