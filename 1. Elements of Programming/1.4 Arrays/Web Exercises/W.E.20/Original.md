***US postal barcodes.*** The POSTNET barcode is used by the US Postal System to route mail. Each decimal digit in the zip code is encoded using a sequence of 5 short and long lines for use by scanners as follows:


![image](https://user-images.githubusercontent.com/80197312/208040370-f15252d1-822b-4b5e-a3ca-46b1b32220d1.png)


A sixth checksum digit is appended: it is computed by summing up the original five digits mod 10. In addition, a long line is added to the beginning and appended to the end. Write a program ZipBarCoder.java that reads in a five digit zip code as the command line parameter and prints the corresponding postal barcode. Print the code vertically instead of horizontally, e.g, the following encodes 08540 (with the check digit of 7).


![image](https://user-images.githubusercontent.com/80197312/208040434-6c539bd4-6f1b-4fdd-b4d0-e51d96ec526e.png)
