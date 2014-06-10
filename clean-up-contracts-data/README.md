# Problem


You have two sets of csv files - one containing the contracts data and the other containing the awarded contracts. Your task is to combine the two csv files using the common field (contractName) and compute the total amount of closed awarded contracts. There are problems with the data, which means there are closed contracts which have been awarded yet.

The data are not real data and presented for this problem only. The data fields and real data are available at http://www.edolidar.gov.np/tenders.php

The first contract file contains the following fields

   * contractname
   * status
   * bidPurchaseDeadline
   * bidSubmissionDeadline
   * bidOpeningDate
   * tenderid
   * publicationDate
   * publishedIn

The second award file contains the following fields

   * contractName
   * contractDate
   * completionDate
   * awardee
   * awardeeLocation
   * Amount

The Output file will contain the fields from both files (blank values if the contract is not awarded yet)

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
   * Amount

After the file is created, read the output file and show the total amount of awarded contracts which have been closed.
700,000 in our case.

——

Your script should read the two files (contracts.csv and awards.csv) and output data-combined file (final.csv) and prints the following output in the screen.

`Total Amount of closed contracts: 700000`
