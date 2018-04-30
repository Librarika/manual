# Medias

**Librarika** organizes books under two logical entities: Media and Media Copies. When a new book is added to a library, master book information is added once as `Media` entity, we call this as title. And other info is added to the `Media Copy` entity. Then when another copy book of same book is added, only a new `Media Copy` entity is added.

#### Media Entity

Contains non-repeating fields such as title, ISBN, ISBN13, description, abstract, publisher, authors, cover photos etc.

#### Media Copy Entity

Contains uniquely identifiable data such as accession number, copy number, location as well as some other information.

#### Relationship
```
 		Media (Single)
			  |
 	 	 	   --- Media Copies (Multiple)
```

## Smart Add

[...]

## Manual Add

[...]

## Bulk Import

Librarika support builk import of catalog items in CSV formats.

#### a. Prepare your data

* Read our [Import Items](https://demo.librarika.com/spages/import-items) for critical information.
* See our sample google spread sheet at [Sample Import Format](https://docs.google.com/spreadsheets/d/1MOphgqXTbOs2YvzvFDjIVAzS8Z7aji58bpuVmDbTnb8/edit?usp=sharing).
* Use google sheets to avoid UTF-8 encoding issue with Microsoft Excel. 
* Download the final CSV file directly from google docs using `File -> Download as -> Comma Separated Values (.csv)` to avoid issues.

#### b. Check List

Please make sure followings before you go ahead with importing your data:

* Columns names must be exactly same and case sensitive.
* File in correct CSV format. Use google sheets if possible.
* The CSV file is UTF-8 encoded. MS Excel produce non UTF-8 csv file.
* Numeric columns contain numeric values.
* Accession numbers are unique and not empty.

#### c. Import Items

1. Go to `Dashboard -> Catalogs -> Catalog Items` section.
2. Click on `Import Items` button.
3. Select data format, specify the CSV file and select branch name.
4. Click on `Submit` button to submit the form.
5. If everything is all right, you will see your data to review. Please review them carefully.
6. Confirm the data and click on `Save` button.
7. You will see the confirmation with number of items added into the system.
8. If same book is provided multiple times, only one record in media section will be created, each one will be added as a separate copy linked to that media record.


## Delete Media

[...]

---

# Media Copies

[...]

## Add Copy

[...]

## Edit Copy

[...]

## Change Accession Number

[...]

## Barcode Scanning

[...]

## Delete Copy

[...]

---

# E-Books

[...]