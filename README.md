June-2024 Multi-Select Lookup LWC for Lightning Screen Flow
Currently the standard Salesforce Lookup component, used in Lightning Screen Flows, does not provide the capability to select more than one item on the mobile form factor.  This custom component provides that capability. This custom component is a generic multi-select lookup component. It can be used for any SObject.  Also, Record Types can be used as a query filter.  
The parameters for this component:
(1) objectApiName: 		input the Api name of the Object to be used for the lookup.
(2) keyFieldApiName: 	input the field name to use in selection (i.e.Name or CaseNumber). This is used in the WHERE clause of the query.
(3) lookupLabel: 			input the text to be used as a label for the lookup.
(4) iconName: 				input the technical name for the Icon (e.g. standard:account).
(5) recordTypes: 			input a record collection of the record types to be used to filter the selection result.
(6) maxQueryResult: 	input the maximum number of records to select on each search. Used in the LIMIT clause of the query. Default value is 10. 
(7) maxSelection: 		input the maximum number of records that the user can select from the lookup. Default value is 5.
(8) userSelection: 		output to save the User Selection to a text Collection. This is used to re-display the user's selection as needed.  For example, when the screen is refreshed due to a data validation error.
(9) selectedRecIds		output collection of record Ids of the selection result. Use this to retrieve the records.
