# PrepareHathiMemberHoldings
Given a group of marc records, create print holdings files for HathiTrust following their guidelines at https://www.hathitrust.org/print_holdings

NOTE:  this project is under construction and is the work of a small pymarc code club.


### Goal

Create 3 output files:

- Single-part monographic holdings – leader 07 = m or i
- Multi-part monographic holdings – leader 07 = a or c
- Serial holdings  – leader 07   =s, b, or d

Need to make sure in the Leader 06 and 008 position 23 that type of record/form of item is print.

Hathi also needs gov docs to be flagged as such - check 008/28

Need to be able to tell it what field the local system number is in (e.g. for III it’s usually 907 subfield a)

### Current Tasks 

Work on outline of what exactly we want to accomplish, e.g. in some cases there might be other fields we’d want to look at - e.g. any markers for it being a brief or temporary record (e.g. is there a valid bib utility number.) We could just make some assumptions for now, e.g. data is supposed to have an OCLC # in the 001, but would need to accommodate easily modifying that test. 

Assign small tasks based on above.

Figure out how to integrate unit testing 

