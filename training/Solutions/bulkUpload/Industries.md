# Industry List

The table below is the master list of sub industries and their IDs to be used within the CSV loader

|Sub Industry ID|Industry|Sub Industry|
|---|---|---|
387171|Communications, Media & Entertainment|Technology
831|Communications, Media & Entertainment|Media & Entertainment
830|Communications, Media & Entertainment|Communications
832|Consumer Industries & Retail|Consumer Packaged Goods
833|Consumer Industries & Retail|Retail
643294|Energy|Water utilities
836|Energy|Mining
834|Energy|Chemical
838|Energy|Oil & Gas
839|Energy|Electric utilities
840|Banking & Capital Markets|Banking
841|Banking & Capital Markets|Capital Markets
843|Banking & Capital Markets|Professional Services
800690|Public Sector|Smart Cities
382734|Public Sector|Social protection
382733|Public Sector|Sport, culture and religion
382732|Public Sector|Public health
382731|Public Sector|Housing and community
382730|Public Sector|Environmental protection
382729|Public Sector|Economic affairs
382728|Public Sector|Public order, justice and safety
382727|Public Sector|External (foreign) affairs
382726|Public Sector|Fiscal affairs
382725|Public Sector|Executive operations
846|Public Sector|Education
845|Public Sector|Defence and intelligence
856|Healthcare & Life Sciences|Healthcare Payers
857|Healthcare & Life Sciences|Healthcare Providers
858|Healthcare & Life Sciences|Life Sciences
859|Healthcare & Life Sciences|Government Health & Human Services
806068|Manufacturing|Construction and Services
861|Manufacturing|Automotive
862|Manufacturing|High Tech
863|Manufacturing|Industrial
864|Manufacturing|High Tech/Electronics
860|Manufacturing|Aerospace & Defense
865|Travel & Transportation|Airlines
866|Travel & Transportation|Freight & Logistics
867|Travel & Transportation|Hospitality
868|Travel & Transportation|Rail
405990|Pan Industry|Pan Industry
405040|Insurance|Reinsurance
405039|Insurance|Broker
405038|Insurance|P&C Insurance
405037|Insurance|Life Insurance



**To request new entries to this list contact the Digital Explorer admin team**

---

~~~
match (i:META_Industry)--(si:META_SubIndustry)
return id(si),i.name,si.name
~~~