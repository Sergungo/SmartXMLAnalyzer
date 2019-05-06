# SmartXMLAnalyzer

Program execution:

java -jar SmartXmlAnalyzer.jar <input_origin_file_path> <input_other_sample_file_path> <target_element_id>

Algorithm :

1) Finds target element.
2) Gets all attributes from target element.
3) Gets all elements which matching attributes from other file.
4) Finds the most similar element and returns it.
5) Gets path to similar element.

Comparison output:

sample-1-evil-gemini.html:

html[0] > body[1] > div[0] > div[1] > div[2] > div[0] > div[0] > div[1] > a[1]

sample-2-container-and-clone.html:

html[0] > body[1] > div[0] > div[1] > div[2] > div[0] > div[0] > div[1] > div[0] > a[0]

sample-3-the-escape.html:

html[0] > body[1] > div[0] > div[1] > div[2] > div[0] > div[0] > div[2] > a[0]

sample-4-the-mash.html:

html[0] > body[1] > div[0] > div[1] > div[2] > div[0] > div[0] > div[2] > a[0]
