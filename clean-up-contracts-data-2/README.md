# Problem


You have two sets of csv files - one containing the contracts data and the other containing the awarded contracts. Your task is to combine the two csv files using the common field (contractName) and compute the total amount of closed awarded contracts. The combined csv should also include one more field - latlon which contains the geocoded value of the contract location, if available. Use the API (from google, osm, or others) to geocode the location. 

There are problems with the data, which means there are closed contracts which have not been awarded yet.

The data are not real data and presented for this problem only. The data fields and real data are available at http://www.edolidar.gov.np/tenders.php

The first [contract file](contracts.csv) contains the following fields

   * contractname
   * status
   * bidPurchaseDeadline
   * bidSubmissionDeadline
   * bidOpeningDate
   * tenderid
   * publicationDate
   * publishedIn

The second [award file](awards.csv) contains the following fields

   * contractName
   * contractDate
   * completionDate
   * awardee
   * awardeeLocation
   * Amount

The [output file](final.csv) will contain the fields from both files (blank values if the contract is not awarded yet)

   * contractname
   * status
   * bidPurchaseDeadline
   * bidSubmissionDeadline
   * bidOpeningDate
   * tenderid
   * publicationDate
   * publishedIn
   * contractDate
   * completionDate
   * awardee
   * awardeeLocation
   * latlon
   * Amount

After the file is created, read the output file and show the total amount of awarded contracts which have been closed.
700,000 in our case.

Additional problem (optional): Visualise the contracts with location in a map (in separate script) using leaflet or similar libraries. 

——

Your script should read the two files [contracts.csv](contracts.csv) and [awards.csv](awards.csv) and output data-combined file [final.csv](final.csv) and prints the following output in the screen.

`Total Amount of closed contracts: 700000`

--

The solution should be uploaded in the github or bitbucket with all the required csv files.

The script should be in any of the following languages: php, python, node, ruby

There should be a README file which should include the process of running the script, with installation/setup of dependencies if required. The script should be able to run by following the instructions without any assumptions. 




