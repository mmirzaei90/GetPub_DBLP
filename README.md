# GetPub_DBLP
To get the publicatioin list of researchers from DBLP dump. First, you need to download dblp.xml, dblp-2017-08-29.dtd and mmdb-2019-04-29.jar. You can download these files from https://dblp.org/faq/1474681.html. 
The input of this code is the researchers' list which include the reseacher name and the reseachers' institution name. The format of this fils is: family name, name "\t"	institution_name
 First, you should compile the DblpExampleParser.jave using the following command:
 javac -cp mmdb-2019-04-29.jar DblpExampleParser.java
Then, you run the next command to get the publication list of each researcher
java -Xmx8G -cp mmdb-2019-04-29.jar:. DblpExampleParser dblp.xml dblp-2017-08-29.dtd
Note that you should change the path of the researcher's list and the output file in your code. 
