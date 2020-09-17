# PROJECT DESCRIPTION

A pixel in an image can be represented using 3 colours: red, green, and blue, where each colour intensity is an integer between 0 and 255. This project has a Map-Reduce program that derives a histogram for each colour. 

For red, for example, the histogram will indicate how many pixels in the dataset have a green value equal to 0, equal to 1, etc (256 values). The pixel file is a text file that has one text line for each pixel.

For example, the line  <br />
<b>23,140,45</b>  <br />
represents a pixel with red=23, green=140, and blue=45.

To compile and run the project navigate to the given directory and do the following steps: <br />
mvn install <br />
rm -rf output <br />
~/hadoop-2.6.5/bin/hadoop jar target/*.jar Histogram pixels-small.txt output <br />
