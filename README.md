# SC Archives Online Records Index - Postman collection

South Carolina Department of Archives and History, [Online Records Index](https://www.archivesindex.sc.gov/). Statewide index to colonial and state plats and grants, wills, estate papers, Revolutionary War audited accounts and more, with page images.

## Import
In Postman: **Import > Link** and paste
`https://raw.githubusercontent.com/mikeyeves/SC-Archives-Online-Records-Index-Postman/main/SC_Archives_Online_Records_Index.postman_collection.json`

## Requests
| Folder | Request | Type |
|---|---|---|
| IIIF | Manifest for an item | JSON (IIIF Presentation 3) |
| IIIF | Image info.json / full image | IIIF Image 2, level 2 |
| Website | Search, Detail, Advanced search, Collections | HTML |

## Notes
- `/service.php/IIIF/...` is public and fast (tested 25 Nov 2026).
- Other `/service.php/...` paths (Auth, Search, Item, find) answer "Invalid controller path": the CollectiveAccess GraphQL/JSON services are not exposed.
- Keyword search is HTML only and slow; extract ids from `Detail/objects/{id}` links.

Built for family-history research (Genealogy-Vault), November 2026. Status lines say what was live-tested.

## Licence
Collection: CC0. The data and images belong to the source institutions; follow their terms of use.
