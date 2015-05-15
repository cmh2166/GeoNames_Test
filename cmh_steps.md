## Christina's Steps

Steps taken to try using the GeoNames reconciliation service endpoint in LODRefine (Linked Open Data OpenRefine) with the States Geodata Spreadsheet from Austin.

1. Create Project in LODRefine with state_tgn.xlsx
2. Nothing changed in LODRefine excel default project creation steps.
3. Starting running GeoNames Python Reconciliation Service locally on http://0.0.0.0:5000
	3a. This instance on my computer already had the api key added, but nothing else changed. 
	3b. If this process fails for me, I'll delete, re-add from GitHub, and try process with adding new api key
4. Added the GeoNames Reconciliation Service Endpoint: 
	4a. State Column (or any column) Top Arrow
	4b. Reconcile
	4c. Start reconciling...
	4d. Add Standard Service...
	4e. Entered http://0.0.0.0:5000/reconcile as the service's URL
	4f. Clicked 'Add Service'
5. In reconciliation service pop-up, choose 'GeoNames Reconciliation Service'
6. Choose '/geonames/name' (starting with most specific API search option)
7. Didn't change any other of the default choices and clicked 'Start Reconciling'
8. Reconiliation occurred! Which is good and bad, because I don't know what is going differently with your instance.
9. For instances without direct, immediate match (37 out of 188, all but 1 of which had multiple matches), reviewed to choose match if there, otherwise ran steps 5-8 again, but using '/geonames/all'
10. More matches added by service. Those leftover need further review for typos, no longer existent regions/names, multiple matches (city and state with same name), etc.
