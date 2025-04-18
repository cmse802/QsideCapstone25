# Testing US Census API 

This example shows how to take one specific address and get the corresponding GEOID using the U.S. Census Geocoder API for testing purposes to make sure the request works. 
**This part of the instructions is not necessary but just for testing purposes**

Code Explanation:

1. First, we set the address of the GeoID we want to find. For this example, we used the white house however you can replace this address with whatever you want, 
all you would need to replace is the “address”, “city”, and “state” in address_params.

2. We set the base URL to: [https://geocoding.geo.census.gov/geocoder/geographies/address](https://geocoding.geo.census.gov/geocoder/geographies/address)

3. Next, we make the API request by using the request libraries in python to send this address to the Census Geocoder API

4. We then parse the response to see if the address is valid or not. If the address is valid, the API returns a GEOID from the "2020 Census Blocks" geography. The code then prints out the GeoID of the address you have inputted.

Notes:

- We recommended you use the address that we provide first since we know the address works. Then if it works you could use a different address if you wanted.
- GEOIDs are key when working with Census data—they help you join datasets geographically.
- No Excel files or datasets are involved in this version—just a quick, standalone test.
