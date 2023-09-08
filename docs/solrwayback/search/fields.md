---
title: Field descriptions
layout: home
parent: Search
grand_parent: SolrWayback
nav_order: 3
permalink: /docs/solrwayback/search/fields
---

# Field desriptions
Below you will find explanations of the most crucial fields. From the search result, you can also click "See all fields" to inspect other possible fields.
{: .fs-6 .fw-300 }

|--- |--- |-- |--- |
|**Field**|**Multivalued**|**Type**|**Description**|
|author|yes|string|From Author meta-data (typical for word, html, pdf, image etc.)|
|description|no|string|From description meta-data (word, html, pdf, image etc.)|
|content_language|no|string|Language of text (recognised by Tika)|
|content_length|no|int|Content length of the payload from the server|
|content_text_length|no|int|Content length of the extracted text|
|content_type_norm|no|string|Content type determined by Tika. Possible values: html,image,pdf,audio,video,word,powerpoint,excel,text,other|
|crawl_date|no|date|When was then url crawled. Additional similar fields: crawl_year_month_day,crawl_year_month,crawl_year|
|domain|no|string|Domain of the URL. Example: nb.dk|
|host|no|string|Host of the URL, this includes subdomain Example: nettarkivet.nb.no|
|id|no|string|The index identifier, unique for each indexed resource.|
|image_size|no|long|The size of image in pixels. There are also similar fields image_height and image_width|
|links_images|yes|string|Links of all image tags on a HTML page.|
|links|yes|string|Links to other pages found in this HTML.|
|links_norm|yes|string|Same as the links field except values are normalized|
|public_suffix|no|string|The public suffix of the url: Example: no, org, co.uk|
|resourcename|no|string|Last part of the URL, after '/' with query parameters. E.g. index.html or cats.jpg&size=100|
|server|yes|string|Value of the Server field in the HTTP header|
|status_code|no|int|The http status code in the HTTP header. 200=ok, 301=redirect, 403=forbidden|
|source_file_path|no|string|Full path to the warc-file where the resource is from. The field source_file_offset gives the offset for the resource in that warc-file|
|source_file|no|string|The filename of the WARC-file without the absolute file path. Is case sensitive|
|title|no|string|From title meta-data|
|type|no|string|Almost same content_type_norm. Just more human names and fewer values: Web Page, Image, Other, Document, Audio, Video, Presentation, Data|
|url|no|string|The exact url seen from the harvest client that created the warc-file|
|url_norm|no|string|A normalized version of the url field. It is lowercased and https is made into http. Also finds unique representation of varius encodings. Also removes som predefined parameter names such as session-id etc. This field is very important for playback in SolrWayback.|
|warc_ip|no|string|IP-address of the server. Taken from the metadat field WARC-IP-Address in the warc-header.|
|warc_key_id|yes|string|The unique identifier (URN) of the resource. Used for persistent referencing.|


----

