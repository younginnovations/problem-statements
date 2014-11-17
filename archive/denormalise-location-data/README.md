# Problem


You are given an [unorganised csv](amp-unorganised-location.csv) file from AMP http://portal.mof.gov.np where the project locations for a given project are present in a single cell. Your task is to denormalise the data row by splitting the location field content. The number of rows should match the number of districts present. In case of missing location, there should be only one data row with blank district and city. 

The input [unorganised csv file](amp-unorganised-location.csv) contains the following fields

   * AMP ID
   * Project Title
   * Status
   * District

The [organised csv file](amp-organised-location.csv) will contain the following fields

   * AMP ID
   * Project Title
   * Status
   * District
   * City


——

Your script should read the following file [amp-unorganised-location.csv](amp-unorganised-location.csv) and output new file [amp-organised-location.csv](amp-organised-location.csv) in exact form. 
