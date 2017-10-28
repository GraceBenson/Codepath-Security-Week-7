# Codepath-Security-Week-7
Week 7 Project: WordPress vs. Kali


Vulnerability 1
WordPress 3.3-4.7.4 - Large File Upload Error XSS

WordPress version tested in: 4.2.2
Vulnerability type: XSS

Steps:
1) Find/create a file and name it Dinosaurs secret life<img src=x onerror=alert(1)>.png
2) Go to add media and try to upload this file into media

GIF Walkthrough:
https://gfycat.com/gifs/detail/BlindBlindBellsnake

Source: https://hackerone.com/reports/203515
