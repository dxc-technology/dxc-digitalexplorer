# Digital Explorer - Solutions
## Bulk Upload

The Digital Explorer solution module allows for solution editors and administrators to upload multiple solutions via a bulk load form.  The bulk load form requires only a simple representation of a solution to be included.<br>


### [SAMPLE FILE](sample.csv)

<br>
The following information is required

- Solution Name
- Description
- Elevator Pitch	
- Solution SubType	
- Referenceable	**OPTIONAL - DEFAULTS TO NO**
- Status	
- Contacts	
- Attachments **OPTIONAL**
- IsPrivate **OPTIONAL - DEFAULTS TO FALSE**
- MetaSubIndustries	 **OPTIONAL**
- Tags **OPTIONAL**


### The following fields support a list of entries

- contacts
- attachment
- MetaSubIndustries
- tag
 
### Structure of listed entries

- A list within the CSV file begins and end with the square brackets `[ ]`
- Values within the list are separated by a semi colon `;`


### Examples

### Contacts

The contact information needs to be provided in the following structure

- `Name, email, role`

`[admin;admin@dxc.com;Solution Owner;test;test@dxc.com;Architect]`

### attachments

`[https://www.dxc.com;https://luxoft.com]`

### MetaSubIndustries

`[405040;843]`


### tags

`[tag1;tag2;tag3]`


---

## Upload process

The upload process reviews the following fields and creates relationships to any matching Business Trends, Technology Trends or Insights within the knowledge graph, this ensures the added solution is connected to the recommendation engine used within the Digital Explorer Workspace and Roadmap modules.

- Solution Name
- Description
- Elevator Pitch	


---

## Special considerations

The `solution Sub type` and `sub industries` require the internal Digital Explorer ID to be provided, review the links below for the latest codes to be used.

- [Solution Types](SolutionTypes.md)
- [Industries](Industries.md)


## Updating existing entries

To update an existing entry, simply include the Digital Explorer Solution ID in the first column of the CSV file.