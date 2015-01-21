# Problem


You have two sets of csv files - one containing the contracts data and the other containing the awarded contracts. Your task is to combine the two csv files using the common field (contractName) and compute the total amount of currently running awarded contracts. There are problems with the data, which means there are closed contracts which have not been awarded yet.

The data are not real data and presented for this problem only. The data fields and real data are available at eProcurement site of various government agencies.

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
   * Amount

After the file is created, read the output file and show the total amount of awarded contracts which are still running (current).
600000 in our case.

——

Your script should read the two files [contracts.csv](contracts.csv) and [awards.csv](awards.csv) and output data-combined file [final.csv](final.csv) and prints the following output in the screen.

`Total Amount of current contracts: 600000`

--

The solution should be uploaded in the github or bitbucket with all the required csv files.

The script should be in one of the following languages: php, python, node, ruby

There should be a README file which should include the process of running the script, with installation/setup of dependencies if required. The script should be able to run by following the instructions.

