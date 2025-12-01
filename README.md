This page will convert the data provided in the excel into a json file.

Goal (Specific): Make a single web page that lets me pick one Excel file. Read only the first sheet. Use the first column as the Customer Name
 ,the second column as the Product and the third column as the url link. 
 The website should create a json file as output  with the sample format below. Add each line from excel with comma seperated until all the lines are read from the excel.
 The value for the key "Customer" should be picked from the first colums of excel."Deployment": "Cloud" is a constant for each section.   "ABPP", "BATM", "CATMAN" values should be picked form second colums of the excel.
"branch": "main" remains same for each customer. Different product for each customer get seperated by [].
 Sample json format :
 
 [
 {
    "Customer": "Medtronic, Inc.",
    "Deployment": "Cloud",
    "ABPP": [
      {
        "url": "https://github.com/aijantakar-arch/WebDevelopment/tree/main",
        "branch": "main",
        "verified": true
      },
      {
        "url": "https://github.com/aijantakar-arch/WebDevelopment/tree/main",
        "branch": "main",
        "verified": true
      }
    ],
     "BATM": [
      {
        "url": "https://github.com/aijantakar-arch/WebDevelopment/tree/main",
        "branch": "main"
      }
    ],
    "Deployment": "Cloud"
  },
   {
    "Customer": "7-Eleven Stores Pty Ltd.",
    "CATMAN": [
      {
        "url": "https://github.com/aijantakar-arch/WebDevelopment/tree/main",
        "branch": "main"
      }
    ],
    "Deployment": "Cloud"
  }
 ]
 Success checks (Measurable):
I can see a json file with the sample format with all the values picked from the excel file.


