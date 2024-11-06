# Scenario
In this scenario, we need to investigate whether two files are identical or different.

Here’s how you'll do this task: First, you’ll display the contents of two files and create hashes for each file. Next, you’ll examine the hashes and compare them.

## 1. Generate hashes for files
- The lab starts in your home directory, /home/analyst, as the current working directory. This directory contains two files file1.txt and file2.txt, which contain different data. In this task, you need to display the contents of each of these files. You’ll then generate a hash value for each of these files and send the values to new files, which you’ll use to examine the differences in these values later.
![1_Check_files](https://github.com/Cr1msonPho3nix/Asset_Management/blob/main/img/Creating%20Hash%20values/1.1_Check_files.PNG)<br>

- Although the contents of both files appear identical when you use the cat command, you need to generate the hash for each file to determine if the files are actually different.
![Check_files](https://github.com/Cr1msonPho3nix/Asset_Management/blob/main/img/Creating%20Hash%20values/1.2_Hashing_files.PNG)<br>

## 2. Compare hashes
- In this task, you’ll write the hashes to two separate files and then compare them to find the difference.
![Check_files](https://github.com/Cr1msonPho3nix/Asset_Management/blob/main/img/Creating%20Hash%20values/2.1_Comparing_hashes.PNG)<br>
In this image, the first character of the files differ, so what seems to be both "X" aren't the same character.