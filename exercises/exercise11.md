# Break a pipeline and debug it

1.	Click on pipelines
2.	Click on Deploy Drupal Pipeline
3.	Click configure 
4.	Click on Deploy (Manifest) Stage
5.	Scroll Down to manifest source
6.	Change namespace to a non-existent mcgonagle2 namespace
7.	Save Pipeline
8.	Run Pipeline
9.	Pipeline Breaks
10.	Click on Pipeline
11.	Click on Source in bottom right
12.	Use a JSON Formatter for Chrome such as JSONView to view JSON
13.	Change the manifest back to existing mcgonagle namespace
14.	Re-run pipeline
