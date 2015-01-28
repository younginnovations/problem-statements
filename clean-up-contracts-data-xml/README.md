# Problem


You have two sets of csv files - one containing the contracts data and the other containing the awarded contracts. Your task is to combine the two csv files using the common field (contractName), generate an XML file and compute the total amount of closed awarded contracts. The combined XML should also include one more field - latLon which contains the geocoded value of the contract location, if available. Use the API (from google, osm, or others) to geocode the location. 

There are problems with the data, which means there are closed contracts which have not been awarded yet.

The data are not real data and presented for this problem only. The data fields and real data are available at various e-procurement portals of government agencies. 

The first [contract file](contracts.csv) contains the following fields

   * contractName
   * status
   * bidPurchaseDeadline
   * bidSubmissionDeadline
   * bidOpeningDate
   * tenderId
   * publicationDate
   * publishedIn

The second [award file](awards.csv) contains the following fields

   * contractName
   * contractDate
   * completionDate
   * awardee
   * awardeeLocation
   * amount

The [output file](final.xml) will contain the fields from both files (blank values if the contract is not awarded yet)

   * contractName
   * status
   * bidPurchaseDeadline
   * bidSubmissionDeadline
   * bidOpeningDate
   * tenderId
   * publicationDate
   * publishedIn
   * contractDate
   * completionDate
   * awardee
   * awardeeLocation
   * latLon
   * amount

After the file is created, read the output file and show the total amount of awarded contracts which have been closed.
700,000 in our case.

——

Your script should read  two files [contracts.csv](contracts.csv) and [awards.csv](awards.csv) and generates combined XML file [final.xml](final.xml) and prints the following output in the screen. Make sure the generated XML file is valid and opens in your browser without any error.

`Total Amount of closed contracts: 700000`

--

The solution should be uploaded in the github with all the required csv files.

The script should be in one of the following languages: php, python

There should be a README file which should include the process of running the script, with installation/setup of dependencies if required. The script should be able to run by following the instructions.




