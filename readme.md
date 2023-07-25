# D2CSV

D2CSV is a tool to generate business leads using the Googlemaps Places API or to individually add businesses manually. Added businesses can be exported to a csv file. 

The tool and code can be accessed via this [link](https://9b8fc4f2-6868-4ba0-aa21-7a2b572431a6.pyscriptapps.com/75a9777a-fbc2-4d75-8f84-051f91f3b816/latest/). 

## Installation

No installation necessary. At first startup please wait till green "Ready" message is displayed before using the tool. 

## Usage

### Googlemaps Places API

Please enter your Googlemaps Places API key. Refer to this [link](https://developers.google.com/maps/documentation/elevation/start) for setting up your API key. Google provides a one time $300 free credit and a monthly recurring $200 free credit equivalent to around 12,000 monthly searches. 

Please also enter your CORS API key. A CORS proxy is required to run python natively in the browser. A free temporary key can be generated from this [link](https://cors.sh/). You can use this [link](https://www.emailgenerator.org) for a temporary email generator. 

After entering the keys please enter a single query for your search. E.g. "Hufschmied", or "Pferdeklinik". 

Then click the "Run Script" button and wait for "Script done!" to be displayed. This may take a while so be patient. If the page becomes unresponsive continue waiting.

Once the script has run, you can click the "Update Table" button to display the table in the "Result" section. You can also click the "Download data.csv" button to download a csv file containing the results. You can also change the query to add more results to the table. 

#### Changing search coordinates 


The Googlemaps Places API returns up to 60 results per coordinate in a set radius. The radius can be changed by updating the radius parameter in main.py.

```python
radius = 20000
```
To update the coordinates used for the search please refer to the coordinates.csv file in the project folder. 

### Manually add business

Please enter the businesses details into the provided fields. Once all details have been added you can click the "Add Row" button to add the business. Clicking the "Reset" button will reset the fields. 

Once a business has been added, you can view the added row by clicking on the "Update Table" button and download by clicking on the "Download data.csv" button. 

## Contributing

Pull requests are welcome. For major changes, please open an issue first
to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License

[MIT](https://choosealicense.com/licenses/mit/)