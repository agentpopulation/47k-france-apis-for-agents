<p align="center"><img src="assets/banner.svg" width="100%" alt="France API endpoints: 47,486 API endpoints passed a keyless data call"></p>

# 🇫🇷 France API endpoints

**47,486 API endpoints filed under country code FR that answered a keyless GET with a data body. For agent and app builders.**

<p align="center"><a href="#files"><img src="https://img.shields.io/badge/endpoints-47%2C486-6366F1" alt="endpoints: 47,486"></a> <a href="#columns-and-tags"><img src="https://img.shields.io/badge/keyless%20JSON-47%2C486-6366F1" alt="keyless JSON: 47,486"></a> <a href="#whats-inside"><img src="https://img.shields.io/badge/services-748-0F172A" alt="services: 748"></a> <a href="#whats-inside"><img src="https://img.shields.io/badge/country-FR-EA580C" alt="country: FR"></a> <a href="LICENSE"><img src="https://img.shields.io/badge/licence-CC%20BY%204.0-0F172A" alt="licence: CC BY 4.0"></a></p>

<p align="center"><a href="#whats-in-it-for-you">What's in it</a> · <a href="#for-ai-agents">For AI agents</a> · <a href="#quick-start">Quick start</a> · <a href="#test-it-yourself">Test it yourself</a> · <a href="#files">Files</a> · <a href="#licence-and-credit">Licence</a> · <a href="#part-of-10m-api-endpoints-for-ai-agents">More packs</a></p>

This repository holds a 1,000-row sample and the services list; the full list of 47,486 endpoints is one download from the [latest release](https://github.com/agentpopulation/47k-france-apis-for-agents/releases/latest).

**Endpoints filed under country code FR, for building an agent or app for France.** Tables of data.gouv.fr through its tabular API, one CSV resource each, and map layers of regions, departments and agglomerations, as URLs that answered with no key on their test date.

Selection rule: rows where `country is FR`, less the rows that a leave-out rule drops (each counted under Known limits).

32,300 of these 47,486 rows match the focus rule (below); the others are in the pack by the selection rule only, and Known limits says what they are. 20,400 rows (43.0%) are map layers on ArcGIS Online, where anyone can publish.

## In plain words

**What is an API endpoint?** An API endpoint is one web address that a program can ask for data, for example the latest reading at one weather station. A single service, such as a national weather agency, can have thousands of endpoints: one per station, city or dataset. This pack counts endpoints, not separate services.

**What does "passed a data call" mean?** On the date shown in each row, AgentPopulation sent one plain request to that address, with no password or key, and got a non-empty data body back (JSON, CSV, XML or a file): not an error page and not an empty result. Some bodies describe a dataset rather than hold its values; see Known limits. It shows the address answered with data on that day. It is not a promise that it answers today, and licences and usage limits were not reviewed.

## What's in it for you

Four ways to use this pack. Each bucket gives a count, a filter you can apply to the CSV, one example that passed, and a list of recommended starting points with the rule that picked them. Buckets overlap; a row can fit more than one.

Examples, recommended lists and the preview are drawn from rows that match this pack's focus rule, so a row that the selection rule put in this pack but that is about something else is not shown as a starting point. Counts cover the whole bucket.

<details>
<summary>The focus rule</summary>

Focus rule: `NOT title matches /(?<![a-z])(test|tests|testing|draft|drafts|copy|sample|samples|demo|untitled|scratch|temp|tmp|delete|deleteme|practice|dummy|example|training)(?![a-z])|final_final|\d{7,}/i AND (NOT url matches ///(services[0-9]*(-[a-z0-9]+)?|utility)\.arcgis\.com//i OR NOT service matches /^ArcGIS organization /i)`

</details>

### 🤖 Agent tools: Keyless JSON layers and tables an agent can call (France)

**47,486** endpoints from 748 services · Wrap one layer query as a get_layer_features tool: pass a where clause or a bounding box, return the matching features with a timeout.

20,442 of these are map-layer queries that asked for a few records (`resultRecordCount`); add a where clause or a geometry to ask about one place, and page through for the whole layer.

Start with: `tags has agent-ready`

Example: [Étalages\_et\_terrasses](https://services.arcgis.com/d3voDfTFbHOCRwVR/ArcGIS/rest/services/%C3%89talages_et_terrasses/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) · Esri France (ArcGIS Online) · passed 2026-11-16

<details>
<summary>Recommended starting points: 8 services, picked by the stated criteria inside</summary>

**Recommended starting points.** Selected by stated criteria, not a ranking of quality: Services in this pack with the most endpoints that match this bucket and are tagged `agent-ready` (no key sent in the test call, JSON body, passed a data call). Ties go to the service with more country codes, then by name. Only services with at least one bucket row that matches the focus rule are listed, and the sample comes from those rows; the counts cover the whole bucket. The sample URL is the first row by URL sort after preferring, in this order: rows that match the bucket's sample preference when it has one, rows that return values rather than describe a dataset or a service (not ERDDAP /info/ pages, OGC GetCapabilities requests, bare OWS addresses, PxWeb tables, UN SDG series lists, Statistics Canada download pointers, WorldPop listings, GTFS validation reports, untitled rows or service root addresses), and agent-ready rows. Sample preference in this bucket: `url matches //query\?/i`. Services named "ArcGIS organization" hold map layers from many owners and are added only when fewer than 5 other services match.

| Service (host) | Endpoints in bucket | In pack | Country codes in bucket | Formats in bucket | Sample URL that passed |
|---|---:|---:|---|---|---|
| tabular-api.data.gouv.fr | 27,044 | 27,044 | FR | json | [data.gouv.fr tabular API: Arrêt physiqu…](https://tabular-api.data.gouv.fr/api/resources/000046e3-6c93-4a0c-9648-8ce30bad2dc2/data/?page_size=10) (2026-11-16) |
| Esri France (ArcGIS Online) (services.arcgis.com) | 933 | 933 | FR | json | [Étalages\_et\_terrasses](https://services.arcgis.com/d3voDfTFbHOCRwVR/ArcGIS/rest/services/%C3%89talages_et_terrasses/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| Collectivité de Corse (ArcGIS Online) (services1.arcgis.com) | 373 | 373 | FR | json | [Accidentologie\_](https://services1.arcgis.com/fugWfqwxXpHDGQIl/ArcGIS/rest/services/Accidentologie_/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| Conseil départemental de l'Aisne (ArcGIS Online) (services1.arcgis.com) | 261 | 261 | FR | json | [ADM\_COMMUNES AGES](https://services1.arcgis.com/iNWpti7T6X4xmP8G/ArcGIS/rest/services/ADM_COMMUNES%20AGES/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| Portail SIG du CD28 (ArcGIS Online) (services3.arcgis.com) | 259 | 259 | FR | json | [ARCGIS\_ONLINE\_ROUTES\_2028\_GLOBAL\_NOV\_20…](https://services3.arcgis.com/OT44GCUVawSsHvFg/ArcGIS/rest/services/ARCGIS_ONLINE_ROUTES_2028_GLOBAL_NOV_2023/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| Communauté d'Agglomération Plaine Vallée (ArcGIS Online) (services2.arcgis.com) | 174 | 174 | FR | json | [18\_communes](https://services2.arcgis.com/rDH2Z04XoJ9VRLop/ArcGIS/rest/services/18_communes/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| Commune de Petit-Caux (ArcGIS Online) (services2.arcgis.com) | 154 | 154 | FR | json | [Accès\_plage](https://services2.arcgis.com/DhKp7RYehDQLyWZh/ArcGIS/rest/services/Acc%C3%A8s_plage/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| Communauté d'Agglomération de Lens-Liévin (ArcGIS Online) (services1.arcgis.com) | 145 | 145 | FR | json | [ADMINISTRATIF](https://services1.arcgis.com/BRw7qlbbcVM2z8ab/ArcGIS/rest/services/ADMINISTRATIF/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |

</details>

### 📱 App features: Map layers and table rows to show in an app (France)

**47,486** endpoints from 748 services · Show a layer on a map, or the first rows of a data.gouv.fr table in a card; page through for more.

Start with: `url matches //(Feature|Map)Server//i OR host is tabular-api.data.gouv.fr`

Example: [data.gouv.fr tabular API: Arrêt physique sur le r…](https://tabular-api.data.gouv.fr/api/resources/000046e3-6c93-4a0c-9648-8ce30bad2dc2/data/?page_size=10) · tabular-api.data.gouv.fr · passed 2026-11-16

<details>
<summary>Recommended starting points: 8 services, picked by the stated criteria inside</summary>

**Recommended starting points.** Selected by stated criteria, not a ranking of quality: Services in this pack with the most endpoints that match this bucket and passed a data call. Ties go to the service with more country codes, then by name. Only services with at least one bucket row that matches the focus rule are listed, and the sample comes from those rows; the counts cover the whole bucket. The sample URL is the first row by URL sort after preferring, in this order: rows that match the bucket's sample preference when it has one, rows that return values rather than describe a dataset or a service (not ERDDAP /info/ pages, OGC GetCapabilities requests, bare OWS addresses, PxWeb tables, UN SDG series lists, Statistics Canada download pointers, WorldPop listings, GTFS validation reports, untitled rows or service root addresses), and agent-ready rows. Services named "ArcGIS organization" hold map layers from many owners and are added only when fewer than 5 other services match.

| Service (host) | Endpoints in bucket | In pack | Country codes in bucket | Formats in bucket | Sample URL that passed |
|---|---:|---:|---|---|---|
| tabular-api.data.gouv.fr | 27,044 | 27,044 | FR | json | [data.gouv.fr tabular API: Arrêt physiqu…](https://tabular-api.data.gouv.fr/api/resources/000046e3-6c93-4a0c-9648-8ce30bad2dc2/data/?page_size=10) (2026-11-16) |
| Esri France (ArcGIS Online) (services.arcgis.com) | 933 | 933 | FR | json | [Étalages\_et\_terrasses](https://services.arcgis.com/d3voDfTFbHOCRwVR/ArcGIS/rest/services/%C3%89talages_et_terrasses/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| Collectivité de Corse (ArcGIS Online) (services1.arcgis.com) | 373 | 373 | FR | json | [Accidentologie\_](https://services1.arcgis.com/fugWfqwxXpHDGQIl/ArcGIS/rest/services/Accidentologie_/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| Conseil départemental de l'Aisne (ArcGIS Online) (services1.arcgis.com) | 261 | 261 | FR | json | [ADM\_COMMUNES AGES](https://services1.arcgis.com/iNWpti7T6X4xmP8G/ArcGIS/rest/services/ADM_COMMUNES%20AGES/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| Portail SIG du CD28 (ArcGIS Online) (services3.arcgis.com) | 259 | 259 | FR | json | [ARCGIS\_ONLINE\_ROUTES\_2028\_GLOBAL\_NOV\_20…](https://services3.arcgis.com/OT44GCUVawSsHvFg/ArcGIS/rest/services/ARCGIS_ONLINE_ROUTES_2028_GLOBAL_NOV_2023/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| Communauté d'Agglomération Plaine Vallée (ArcGIS Online) (services2.arcgis.com) | 174 | 174 | FR | json | [18\_communes](https://services2.arcgis.com/rDH2Z04XoJ9VRLop/ArcGIS/rest/services/18_communes/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| Commune de Petit-Caux (ArcGIS Online) (services2.arcgis.com) | 154 | 154 | FR | json | [Accès\_plage](https://services2.arcgis.com/DhKp7RYehDQLyWZh/ArcGIS/rest/services/Acc%C3%A8s_plage/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| Communauté d'Agglomération de Lens-Liévin (ArcGIS Online) (services1.arcgis.com) | 145 | 145 | FR | json | [ADMINISTRATIF](https://services1.arcgis.com/BRw7qlbbcVM2z8ab/ArcGIS/rest/services/ADMINISTRATIF/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |

</details>

### 🧠 Grounding and data pipelines: Statistics, boundaries, parcels and inventories for scheduled loads (France)

**1,695** endpoints from 177 services · Load the tables and layers on a schedule into your own store, so an agent can cite a dated source.

Start with: `format in (csv, xml, geojson) OR title matches /statist|census|population|boundar|parcel|zoning|district|budget|election|crash|permit|inventory|land ?use|landuse|cadast|address/i`

Example: [data.gouv.fr tabular API: Budget 2026 (BP) de la …](https://tabular-api.data.gouv.fr/api/resources/0007b6c0-9040-4445-a744-ab9090721f57/data/?page_size=10) · tabular-api.data.gouv.fr · passed 2026-11-16

<details>
<summary>Recommended starting points: 8 services, picked by the stated criteria inside</summary>

**Recommended starting points.** Selected by stated criteria, not a ranking of quality: Services in this pack with the most endpoints that match this bucket and passed a data call. Ties go to the service with more country codes, then by name. Only services with at least one bucket row that matches the focus rule are listed, and the sample comes from those rows; the counts cover the whole bucket. The sample URL is the first row by URL sort after preferring, in this order: rows that match the bucket's sample preference when it has one, rows that return values rather than describe a dataset or a service (not ERDDAP /info/ pages, OGC GetCapabilities requests, bare OWS addresses, PxWeb tables, UN SDG series lists, Statistics Canada download pointers, WorldPop listings, GTFS validation reports, untitled rows or service root addresses), and agent-ready rows. Services named "ArcGIS organization" hold map layers from many owners and are added only when fewer than 5 other services match.

| Service (host) | Endpoints in bucket | In pack | Country codes in bucket | Formats in bucket | Sample URL that passed |
|---|---:|---:|---|---|---|
| tabular-api.data.gouv.fr | 1,195 | 27,044 | FR | json | [data.gouv.fr tabular API: Budget 2026 (…](https://tabular-api.data.gouv.fr/api/resources/0007b6c0-9040-4445-a744-ab9090721f57/data/?page_size=10) (2026-11-16) |
| Esri France (ArcGIS Online) (services.arcgis.com) | 43 | 933 | FR | json | [District\_Inde\_JP](https://services.arcgis.com/d3voDfTFbHOCRwVR/ArcGIS/rest/services/District_Inde_JP/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| Communauté d'Agglomération Plaine Vallée (ArcGIS Online) (services2.arcgis.com) | 19 | 174 | FR | json | [Parcellaire\_public\_2023\_Andilly](https://services2.arcgis.com/rDH2Z04XoJ9VRLop/ArcGIS/rest/services/Parcellaire_public_2023_Andilly/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| Gouvernement de la Nouvelle-Calédonie (ArcGIS Online) (services1.arcgis.com) | 15 | 105 | FR | json | [cadastre\_centroide](https://services1.arcgis.com/TZcrgU6CIbqWt9Qv/ArcGIS/rest/services/cadastre_centroide/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| Ville de Victoriaville (ArcGIS Online) (services1.arcgis.com) | 14 | 112 | FR | json | [Demographie2 / Population totale](https://services1.arcgis.com/UojxRYPSwkE7A9CP/ArcGIS/rest/services/Demographie2/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| PETR du Piémont des Vosges (ArcGIS Online) (services2.arcgis.com) | 13 | 139 | FR | json | [Parcelles\_orphelines](https://services2.arcgis.com/WEjoILHjHd4dghw9/ArcGIS/rest/services/Parcelles_orphelines/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| Commune de Petit-Caux (ArcGIS Online) (services2.arcgis.com) | 11 | 154 | FR | json | [Adresse\_cadastre](https://services2.arcgis.com/DhKp7RYehDQLyWZh/ArcGIS/rest/services/Adresse_cadastre/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| Atmo Auvergne-Rhône-Alpes (ArcGIS Online) (services3.arcgis.com) | 9 | 74 | FR | json | [Populations exposées en Auvergne-Rhône-…](https://services3.arcgis.com/o7Q3o5SkiSeZD5LK/ArcGIS/rest/services/Populations%20expos%C3%A9es%20en%20Auvergne-Rh%C3%B4ne-Alpes%20en%202020/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |

</details>

### 🧪 Evals and testing: Varied responses to test tool calls and parsers

**47,486** endpoints · 748 services · country FR · 1 format · Run your tool calls against a fixed set of URLs across formats and record which answer; last_tested is the baseline for your own re-tests.

Start with: the whole pack

Example: [data.gouv.fr tabular API: Arrêt physique sur le r…](https://tabular-api.data.gouv.fr/api/resources/000046e3-6c93-4a0c-9648-8ce30bad2dc2/data/?page_size=10) · tabular-api.data.gouv.fr · passed 2026-11-16

<details>
<summary>Recommended starting points: 8 services, picked by the stated criteria inside</summary>

**Recommended starting points.** Selected by stated criteria, not a ranking of quality: Services in this pack that returned the most different formats, then the most endpoints that passed a data call, then by name: a mix of response shapes to test parsers and tool calls. Here the services returned 1 format each, so the order comes down to endpoint counts. Only services with at least one bucket row that matches the focus rule are listed, and the sample comes from those rows; the counts cover the whole bucket. The sample URL is the first row by URL sort after preferring, in this order: rows that match the bucket's sample preference when it has one, rows that return values rather than describe a dataset or a service (not ERDDAP /info/ pages, OGC GetCapabilities requests, bare OWS addresses, PxWeb tables, UN SDG series lists, Statistics Canada download pointers, WorldPop listings, GTFS validation reports, untitled rows or service root addresses), and agent-ready rows. Services named "ArcGIS organization" hold map layers from many owners and are added only when fewer than 5 other services match.

| Service (host) | Endpoints in bucket | In pack | Country codes in bucket | Formats in bucket | Sample URL that passed |
|---|---:|---:|---|---|---|
| tabular-api.data.gouv.fr | 27,044 | 27,044 | FR | json | [data.gouv.fr tabular API: Arrêt physiqu…](https://tabular-api.data.gouv.fr/api/resources/000046e3-6c93-4a0c-9648-8ce30bad2dc2/data/?page_size=10) (2026-11-16) |
| Esri France (ArcGIS Online) (services.arcgis.com) | 933 | 933 | FR | json | [Étalages\_et\_terrasses](https://services.arcgis.com/d3voDfTFbHOCRwVR/ArcGIS/rest/services/%C3%89talages_et_terrasses/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| Collectivité de Corse (ArcGIS Online) (services1.arcgis.com) | 373 | 373 | FR | json | [Accidentologie\_](https://services1.arcgis.com/fugWfqwxXpHDGQIl/ArcGIS/rest/services/Accidentologie_/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| Conseil départemental de l'Aisne (ArcGIS Online) (services1.arcgis.com) | 261 | 261 | FR | json | [ADM\_COMMUNES AGES](https://services1.arcgis.com/iNWpti7T6X4xmP8G/ArcGIS/rest/services/ADM_COMMUNES%20AGES/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| Portail SIG du CD28 (ArcGIS Online) (services3.arcgis.com) | 259 | 259 | FR | json | [ARCGIS\_ONLINE\_ROUTES\_2028\_GLOBAL\_NOV\_20…](https://services3.arcgis.com/OT44GCUVawSsHvFg/ArcGIS/rest/services/ARCGIS_ONLINE_ROUTES_2028_GLOBAL_NOV_2023/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| Communauté d'Agglomération Plaine Vallée (ArcGIS Online) (services2.arcgis.com) | 174 | 174 | FR | json | [18\_communes](https://services2.arcgis.com/rDH2Z04XoJ9VRLop/ArcGIS/rest/services/18_communes/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| Commune de Petit-Caux (ArcGIS Online) (services2.arcgis.com) | 154 | 154 | FR | json | [Accès\_plage](https://services2.arcgis.com/DhKp7RYehDQLyWZh/ArcGIS/rest/services/Acc%C3%A8s_plage/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |
| Communauté d'Agglomération de Lens-Liévin (ArcGIS Online) (services1.arcgis.com) | 145 | 145 | FR | json | [ADMINISTRATIF](https://services1.arcgis.com/BRw7qlbbcVM2z8ab/ArcGIS/rest/services/ADMINISTRATIF/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (2026-11-16) |

</details>

The same lists are in [recommended.json](recommended.json), ready for an agent to load.

## Questions an agent can answer with this pack

- What do the first rows of a data.gouv.fr table hold? Try [data.gouv.fr tabular API: Arrêt physique sur le r…](https://tabular-api.data.gouv.fr/api/resources/000046e3-6c93-4a0c-9648-8ce30bad2dc2/data/?page_size=10) (tabular-api.data.gouv.fr, passed 2026-11-16).
- Which layers does the Collectivité de Corse publish? Try [Accidentologie\_](https://services1.arcgis.com/fugWfqwxXpHDGQIl/ArcGIS/rest/services/Accidentologie_/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (Collectivité de Corse (ArcGIS Online), passed 2026-11-16).
- Which layers does the Conseil départemental de l'Aisne publish? Try [ADM\_COMMUNES AGES](https://services1.arcgis.com/iNWpti7T6X4xmP8G/ArcGIS/rest/services/ADM_COMMUNES%20AGES/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) (Conseil départemental de l'Aisne (ArcGIS Online), passed 2026-11-16).

## What "passed a data call" means

> [!NOTE]
> On the date in `last_tested` (IST), one GET to the URL, sent with no key, returned HTTP 2xx and a non-empty data body. HTML pages and empty results did not pass. The `format` column records what came back. This is a test result for that date, not a promise that the URL answers today. Licences, terms, rate limits, accuracy and freshness were not reviewed. Endpoints are URLs, not separate APIs; many share one service. This pack was tested 16–17 Nov 2026; snapshot 16 Nov 2026.

## For AI agents

Start from keyless JSON endpoints (`agent-ready`). The code below loads `recommended.json` and calls the first recommended service in the Agent tools bucket, with a timeout (`node examples/agent-start.mjs --recommended`). With no argument, `node examples/agent-start.mjs` calls the most recently tested agent-ready row of the sample; pass a `.csv` or `.csv.gz` path to use that file instead. See [examples/agent-start.mjs](examples/agent-start.mjs).

```js
// Node 18+. Loads recommended.json (the local copy, or the raw file on GitHub) and calls one keyless JSON endpoint.
import fs from 'node:fs';

const RAW = 'https://raw.githubusercontent.com/agentpopulation/47k-france-apis-for-agents/main/recommended.json';
const rec = fs.existsSync('recommended.json')
  ? JSON.parse(fs.readFileSync('recommended.json', 'utf8'))
  : await (await fetch(RAW)).json();

const pick = rec.buckets.find((b) => b.id === 'agent').services[0];
try {
  const res = await fetch(pick.sample_url, {
    headers: { 'User-Agent': 'agent-example/1.0' },
    signal: AbortSignal.timeout(15000),
  });
  console.log(pick.service, res.status, res.headers.get('content-type'));
  console.log((await res.text()).slice(0, 300));
} catch (err) {
  console.log(`did not answer now; last passed ${pick.sample_last_tested} (${err.message})`);
}
```

How an agent picks an endpoint:

1. Filter to `agent-ready` and your country or topic.
2. Prefer the newest `last_tested` and the larger services.
3. Call with a timeout and check the body before you use it.

## Quick start

The examples run against the sample in `data/` out of the box (1,000 rows). Each takes an optional path to a `.csv` or `.csv.gz` file instead.

```bash
git clone https://github.com/agentpopulation/47k-france-apis-for-agents.git
cd 47k-france-apis-for-agents
python examples/quickstart.py
node examples/quickstart.mjs
node examples/agent-start.mjs
```

Full list: download `France_API_Endpoints_AgentPopulation_Snapshot_2026-11-16.csv.gz` (47,486 rows, 2.0 MB) from [releases/latest](https://github.com/agentpopulation/47k-france-apis-for-agents/releases/latest), then gunzip it and pass its path. The scripts also read the `.csv.gz` as it is.

```bash
gunzip France_API_Endpoints_AgentPopulation_Snapshot_2026-11-16.csv.gz
python examples/quickstart.py France_API_Endpoints_AgentPopulation_Snapshot_2026-11-16.csv
node examples/quickstart.mjs France_API_Endpoints_AgentPopulation_Snapshot_2026-11-16.csv
```

### curl

Quote the URL: some contain commas.

```bash
curl -sL "https://raw.githubusercontent.com/agentpopulation/47k-france-apis-for-agents/main/data/France_API_Endpoints_AgentPopulation_Sample.csv" | head -n 4
curl -s --max-time 15 "https://services.arcgis.com/d3voDfTFbHOCRwVR/ArcGIS/rest/services/%C3%89talages_et_terrasses/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json" | head -c 600
```

### Python

Standard library only: [examples/quickstart.py](examples/quickstart.py) reads the sample, or the path you pass, keeps agent-ready rows and calls the most recently tested one.

<details>
<summary>The code</summary>

```python
# Python 3, standard library only. Run from a clone of this repository:
#   python examples/quickstart.py [path]
# With no path it reads the sample in data/. Pass the full list from the latest release (.csv or .csv.gz) instead.
# Keeps agent-ready rows and calls the most recently tested one.
import csv
import gzip
import os
import re
import sys
import urllib.request

HERE = os.path.dirname(os.path.abspath(__file__))
path = sys.argv[1] if len(sys.argv) > 1 else os.path.join(HERE, "..", "data", "France_API_Endpoints_AgentPopulation_Sample.csv")
opener = gzip.open if path.endswith(".gz") else open
with opener(path, "rt", newline="", encoding="utf-8") as f:
    rows = list(csv.DictReader(f))

agent = [r for r in rows if "agent-ready" in r["tags"].split("|")]
# Newest test date first; URLs that describe a dataset or a service rather than return values go last.
DESCRIBES = re.compile(r"/erddap/info/|action-report\.json$|[?&]request=getcapabilities|/GeoArea/[^/?]+/List|getFullTableDownloadCSV|hub\.worldpop\.org", re.I)
agent.sort(key=lambda r: r["last_tested"], reverse=True)
agent.sort(key=lambda r: 1 if DESCRIBES.search(r["url"]) else 0)
print(len(rows), "rows,", len(agent), "agent-ready")
if not agent:
    sys.exit(0)

row = agent[0]
req = urllib.request.Request(row["url"], headers={"User-Agent": "agent-example/1.0"})
try:
    with urllib.request.urlopen(req, timeout=15) as res:
        body = res.read(1_000_000).decode("utf-8", "replace")
        print(res.status, res.headers.get("Content-Type"))
        print(body[:300])
except Exception as err:
    print(f"did not answer now; last passed {row['last_tested']} ({err})")
```

</details>

### JavaScript

Reads the sample as JSON because the CSV has quoted commas.

<details>
<summary>The code</summary>

```js
// Node 18+. Reads the sample as JSON (the CSV has quoted commas), local file first.
import fs from 'node:fs';

const FILE = 'data/France_API_Endpoints_AgentPopulation_Sample.json';
const rows = fs.existsSync(FILE)
  ? JSON.parse(fs.readFileSync(FILE, 'utf8'))
  : await (await fetch('https://raw.githubusercontent.com/agentpopulation/47k-france-apis-for-agents/main/data/France_API_Endpoints_AgentPopulation_Sample.json')).json();

const row = rows.find((r) => r.tags.includes('agent-ready'));
const res = await fetch(row.url, { headers: { 'User-Agent': 'agent-example/1.0' }, signal: AbortSignal.timeout(15000) });
console.log(res.status, (await res.text()).slice(0, 300));
```

</details>

### Agent tools

[examples/agent-tools.json](examples/agent-tools.json) holds two tool definitions in the shape most tool-calling APIs accept (name, description, JSON Schema); rename `parameters` if yours uses another key. [examples/quickstart.mjs](examples/quickstart.mjs) implements them:

- `find_endpoints` searches the agent-ready rows of the list by words (their format is json). When you load the tools of more than one pack, prefix the names (for example `france_find_endpoints`) so they do not clash.
- `fetch_endpoint` calls one URL, **refuses any URL that is not in the list** and does not follow redirects. The allowlist is built from the CSV, so a URL injected into a prompt is refused.

The same two tools can sit behind an MCP server.

## Test it yourself

Re-test endpoints from the sample with the same rule: HTTP 2xx and a non-empty body that is not an HTML page. Node 18+, no packages.

```bash
node tools/test-endpoints.mjs
```

It tests the first 50 URLs and prints one line: tested, passed, did not pass. Options: a `.csv` or `.csv.gz` path (the full list from the release), `--limit 50`, `--timeout-ms 10000`, `--out results.csv`. The results file holds `url`, `status`, `passed`, `content_type`, `ms` and `checked_at`; a status of `timeout` or `error:<code>` means no HTTP answer came back. It is polite: GET only, no key sent, at most 4 requests in flight, one at a time per listed host, at least 1 second between requests to one listed host, and reading stops once 256 kB of a body is kept. Redirects are followed and may lead to another host. `results.csv` is in `.gitignore`.

## Preview

One row from each of the five largest services among rows that match the focus rule, services with rows that return values first.

| Title | Service | Country | Format | Tested | Link |
|---|---|---|---|---|---|
| data.gouv.fr tabular API: Arrêt physique sur le réseau SAEI… | tabular-api.data.gouv.fr | FR | json | 2026-11-16 | [tabular-api.data.gouv.fr](https://tabular-api.data.gouv.fr/api/resources/000046e3-6c93-4a0c-9648-8ce30bad2dc2/data/?page_size=10) |
| Étalages\_et\_terrasses | Esri France (ArcGIS Online) | FR | json | 2026-11-16 | [services.arcgis.com](https://services.arcgis.com/d3voDfTFbHOCRwVR/ArcGIS/rest/services/%C3%89talages_et_terrasses/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) |
| Accidentologie\_ | Collectivité de Corse (ArcGIS Online) | FR | json | 2026-11-16 | [services1.arcgis.com](https://services1.arcgis.com/fugWfqwxXpHDGQIl/ArcGIS/rest/services/Accidentologie_/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) |
| ADM\_COMMUNES AGES | Conseil départemental de l'Aisne (ArcGIS Online) | FR | json | 2026-11-16 | [services1.arcgis.com](https://services1.arcgis.com/iNWpti7T6X4xmP8G/ArcGIS/rest/services/ADM_COMMUNES%20AGES/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) |
| ARCGIS\_ONLINE\_ROUTES\_2028\_GLOBAL\_NOV\_2023 | Portail SIG du CD28 (ArcGIS Online) | FR | json | 2026-11-16 | [services3.arcgis.com](https://services3.arcgis.com/OT44GCUVawSsHvFg/ArcGIS/rest/services/ARCGIS_ONLINE_ROUTES_2028_GLOBAL_NOV_2023/FeatureServer/0/query?where=1%3D1&outFields=*&resultRecordCount=10&f=json) |

Browse the 1,000-row sample: [Sample CSV](data/France_API_Endpoints_AgentPopulation_Sample.csv) · [Sample JSON](data/France_API_Endpoints_AgentPopulation_Sample.json).

## What's inside

<p align="center"><img src="assets/breakdown.svg" width="100%" alt="Top categories and formats in this pack"></p>

<details>
<summary>Categories: top 8</summary>

| Category | Endpoints | |
|---|---:|---|
| Government & Open Data | 14,578 | `████████████████████` |
| Transport & Mobility | 12,419 | `█████████████████` |
| Navigation & Geo/Maps | 10,888 | `███████████████` |
| Statistics & Economy | 3,248 | `████▌` |
| Environment | 2,673 | `███▋` |
| Weather & Climate | 1,752 | `██▍` |
| Hydrology & Oceans | 816 | `█▏` |
| Health | 710 | `█` |

</details>

Formats: json 47,486

<details>
<summary>Largest services: top 25 of 748</summary>

| Service | Host | Endpoints | Keyless JSON | |
|---|---|---:|---:|---|
| tabular-api.data.gouv.fr | tabular-api.data.gouv.fr | 27,044 | 27,044 | `████████████████████` |
| Esri France (ArcGIS Online) | services.arcgis.com | 933 | 933 | `▊` |
| ArcGIS Online layers (services.arcgis.com, org wLDmHsvxROjaiPKt) † | services.arcgis.com | 659 | 659 | `▌` |
| ArcGIS Online layers (services6.arcgis.com, org xSLkUVFsDwlw8OJK) † | services6.arcgis.com | 646 | 646 | `▌` |
| ArcGIS Online layers (services5.arcgis.com, org 7RhKUl41LEYtc4NA) † | services5.arcgis.com | 456 | 456 | `▍` |
| Collectivité de Corse (ArcGIS Online) | services1.arcgis.com | 373 | 373 | `▎` |
| ArcGIS Online layers (services-eu1.arcgis.com, org wNMu5mi0eOU5tY3u) † | services-eu1.arcgis.com | 338 | 338 | `▎` |
| ArcGIS Online layers (services1.arcgis.com, org K1RVqQUkYg8ZCwTQ) † | services1.arcgis.com | 285 | 285 | `▎` |
| ArcGIS Online layers (services2.arcgis.com, org qjNehkfurYBmoO45) † | services2.arcgis.com | 270 | 270 | `▎` |
| Conseil départemental de l'Aisne (ArcGIS Online) | services1.arcgis.com | 261 | 261 | `▎` |
| Portail SIG du CD28 (ArcGIS Online) | services3.arcgis.com | 259 | 259 | `▎` |
| ArcGIS Online layers (services6.arcgis.com, org t1x2fCpzwVTiotcK) † | services6.arcgis.com | 256 | 256 | `▎` |
| ArcGIS Online layers (services3.arcgis.com, org Jt57y69af30KhGer) † | services3.arcgis.com | 255 | 255 | `▎` |
| ArcGIS Online layers (services-eu1.arcgis.com, org pFNDYLmkNQWF2E8p) † | services-eu1.arcgis.com | 239 | 239 | `▏` |
| ArcGIS Online layers (services7.arcgis.com, org oEkatiABgemcQjxI) † | services7.arcgis.com | 238 | 238 | `▏` |
| ArcGIS Online layers (services-eu1.arcgis.com, org de9awAHJGTPtVVLW) † | services-eu1.arcgis.com | 234 | 234 | `▏` |
| ArcGIS Online layers (services7.arcgis.com, org wR9S45tPMlnR7zkM) † | services7.arcgis.com | 223 | 223 | `▏` |
| ArcGIS Online layers (services.arcgis.com, org CaoMq07djE0FqJTO) † | services.arcgis.com | 191 | 191 | `▏` |
| ArcGIS Online layers (services2.arcgis.com, org fKO2K6qiLNlgkZ2U) † | services2.arcgis.com | 177 | 177 | `▏` |
| Communauté d'Agglomération Plaine Vallée (ArcGIS Online) | services2.arcgis.com | 174 | 174 | `▏` |
| ArcGIS Online layers (services9.arcgis.com, org nuNzn0OMg75uWEMq) † | services9.arcgis.com | 171 | 171 | `▏` |
| ArcGIS Online layers (services6.arcgis.com, org XgSVk5L0bMP2HZ15) † | services6.arcgis.com | 163 | 163 | `▏` |
| ArcGIS Online layers (services.arcgis.com, org AFB2OfbV8ZevekJ0) † | services.arcgis.com | 155 | 155 | `▏` |
| ArcGIS Online layers (services2.arcgis.com, org OSTljxuSj3y4z219) † | services2.arcgis.com | 154 | 154 | `▏` |
| Commune de Petit-Caux (ArcGIS Online) | services2.arcgis.com | 154 | 154 | `▏` |

† No row of these services matches the focus rule: the selection rule put them in this pack, so they are not used as a starting point.

</details>

<details>
<summary>Rows per test date: 16–17 Nov 2026</summary>

| Date (IST) | Endpoints | |
|---|---:|---|
| 2026-11-17 | 35 | `▏` |
| 2026-11-16 | 47,451 | `████████████████████` |

</details>

## Files

| File | Rows | Size | Use |
|---|---:|---:|---|
| [data/France_API_Services_AgentPopulation.csv](data/France_API_Services_AgentPopulation.csv) | 748 | 48.7 kB | One row per service with its endpoint count in this pack |
| [data/France_API_Endpoints_AgentPopulation_Sample.csv](data/France_API_Endpoints_AgentPopulation_Sample.csv) | 1,000 | 333.2 kB | The sample: focus-rule rows first, each service in proportion to its share; ArcGIS Online layers count as one service |
| [data/France_API_Endpoints_AgentPopulation_Sample.json](data/France_API_Endpoints_AgentPopulation_Sample.json) | 1,000 | 516.1 kB | The same rows as JSON, tags as an array |
| [France_API_Endpoints_AgentPopulation_Snapshot_2026-11-16.csv.gz](https://github.com/agentpopulation/47k-france-apis-for-agents/releases/latest) | 47,486 | 2.0 MB | The full list, gzipped CSV: a download from the latest release, checked by `SHA256SUMS.txt` |
| [tools/test-endpoints.mjs](tools/test-endpoints.mjs) | | | Re-tests endpoints from the sample or the full list |

Sample size: 1,000 rows, which is 1,000 or one third of the pack rounded down, whichever is smaller. Rows that match the focus rule come first. Each service gets rows in proportion to its share of those rows, at least one for the largest services and at most 50% of the sample while other services have rows; ArcGIS Online layers count as one service, whatever their organisation. Within a service, agent-ready rows, rows that return values and the newest test dates come first, and rows are written in turn across services. Service root addresses are placed at the end of the sample.

Full list: download `France_API_Endpoints_AgentPopulation_Snapshot_2026-11-16.csv.gz` (47,486 rows, 2.0 MB) from [releases/latest](https://github.com/agentpopulation/47k-france-apis-for-agents/releases/latest), then gunzip it and pass its path. The scripts also read the `.csv.gz` as it is.

Excel users: Data > From Text/CSV, UTF-8. Files are UTF-8 without a byte-order mark and comma-separated.

## Columns and tags

<details>
<summary>Columns, types and tags</summary>

| Column | Type | Example | Meaning |
|---|---|---|---|
| url | string | [https://tabular-api.data.gouv.fr/api/re…](https://tabular-api.data.gouv.fr/api/resources/000046e3-6c93-4a0c-9648-8ce30bad2dc2/data/?page_size=10) | The address that was tested |
| title | string | data.gouv.fr tabular API: Arrêt physiqu… | Station, dataset or feed name |
| service | string | tabular-api.data.gouv.fr | The service the endpoint belongs to; joins to the services file together with host |
| host | string | tabular-api.data.gouv.fr | Host name of the address |
| country | string | FR | ISO 3166-1 alpha-2 code, or EU; empty when global or unknown |
| category | string | Transport & Mobility | Category of the endpoint |
| subcategory | string |  | Left empty from the 15 Nov 2026 snapshot; kept so the columns stay the same |
| format | string | json | What the test call returned: json, csv, geojson, xml, gtfs, zip, txt and so on |
| tags | string | `no-key\|json\|agent-ready` | Tags separated by \| |
| last_tested | date | 2026-11-16 | Date of the test call, YYYY-MM-DD (IST) |

| Tag | Rows | Meaning |
|---|---:|---|
| agent-ready | 47,486 | No key sent, JSON body, passed a data call on last_tested |
| json | 47,486 | Format of the body |
| no-key | 47,486 | No key was sent in the test call |

A machine-readable copy of this dictionary is in [datapackage.json](datapackage.json).

</details>

## Known limits

- 20,442 rows are map-layer queries with resultRecordCount set: the tested call asked for a few records; change the query to get the full layer.
- 20,400 rows are layers on ArcGIS Online, where anyone can publish: some are class projects, tests or copies. Check the owner and the fields before you rely on one. Only layers of organisations with a name of their own, whose titles do not read as a test, draft or copy, are used as starting points.
- 2,754 rows have a title that reads as a test, a draft, a copy or a sample; they are not used as starting points.
- The country code (FR) is the code the endpoint is filed under, not the place the data covers and not always the publisher's country. Where a row had no code, the code of its ArcGIS organisation is used when that organisation lists one country only. In a sample of 14 titles read before release, none was about a place outside France. Filter by title or service if you need data about one place.
- Stations and feeds can go quiet after their test date; re-test a URL before you rely on it.
- Not in this pack: endpoints that need a key or a POST, and URLs that did not pass.
- Left out: 332 ArcGIS Survey123 layers (they can hold people's form answers).
- Left out: 1 layer marked editable in the title (it can hold entries that people added).
- Left out: 23 ArcGIS layers that keep a form's default service name (they can hold people's form answers).
- Left out: 151 ArcGIS class or coursework layers (lab, assignment, exam, quiz, lesson, exercise, tutorial and final-project layers, copies of class layers, layers named for a person or a person's home, and layers whose name ends in a person's name or holds a student number).
- Left out: 7 ArcGIS layers that hold reports, comments, submissions or form responses sent in by the public.
- Left out: 1 ArcGIS layer that is a record about named people (employee, patient, client or donor lists, home addresses, voter lists, sex offender and missing person layers).
- Left out: 2 rows that are another address of an ArcGIS layer dropped for what it holds (one of the reasons above, found under another address of the layer).
- Left out: 28 rows of ArcGIS Online organisations that are class accounts (3 class sets or more in at least 20% of their rows, 10 class sets or more with no organisation name, or layers signed by students read by hand): their other layers are students' work too.
- Left out: 85 rows of class sets: one map layer saved under 5 or more students' initials or names in one ArcGIS Online organisation, or in 4 or more students' own organisations.
- Left out: 2,566 rows of university, college and school organisations and hosts (many of their layers are students' work).
- Left out: 82 rows whose address is already in an earlier pack of the collection.
- Left out: 7,780 rows that are another address form of an ArcGIS layer already in an earlier pack of the collection (the same rows under another query).
- Left out: 8,077 rows that are a second address form of an ArcGIS layer in this list (the same rows under another query); one address is kept per layer, the newest test first.

## Licence and credit

> [!IMPORTANT]
> This list (URLs, titles, tags and test results) is © 2026 AgentPopulation, released under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Credit AgentPopulation and link agentpopulation.com. The data each endpoint returns belongs to its provider and stays under that provider's terms; this licence does not cover it.

Copy-ready credit:

`France API endpoints by AgentPopulation (https://agentpopulation.com), CC BY 4.0, snapshot 16 Nov 2026.`

GitHub's "Cite this repository" button reads [CITATION.cff](CITATION.cff).

<!-- agentpopulation:start -->
## Part of 10M API endpoints for AI agents

This pack is one of the 50 topic packs of [10m-open-apis-for-ai-agents](https://github.com/agentpopulation/10m-open-apis-for-ai-agents), the open collection by [AgentPopulation](https://agentpopulation.com). Target: 10 million+ open API endpoints that pass a keyless API call.

AgentPopulation's test run of 16 Nov 2026: 4,452,803 tested, 3,346,053 passed a data call. This is the France pack: 47,486 endpoints from 748 services, none of them in a pack read from the earlier snapshot, by address or as another address of the same map layer. Packs overlap, so an endpoint can appear in more than one.

For the latest tested endpoints, search [agentpopulation.com/apis](https://agentpopulation.com/apis). This pack is a snapshot from 16 Nov 2026.

Sibling packs that share the most URLs with this one: [59k-europe-region-arcgis-apis-for-agents](https://github.com/agentpopulation/59k-europe-region-arcgis-apis-for-agents) (2,383 shared) · [160k-county-and-city-gis-apis-for-agents](https://github.com/agentpopulation/160k-county-and-city-gis-apis-for-agents) (183 shared) · [25k-arcgis-server-apis-for-agents](https://github.com/agentpopulation/25k-arcgis-server-apis-for-agents) (42 shared) · [47k-public-agency-gis-apis-for-agents](https://github.com/agentpopulation/47k-public-agency-gis-apis-for-agents) (11 shared). The rest are listed in [10m-open-apis-for-ai-agents](https://github.com/agentpopulation/10m-open-apis-for-ai-agents).

Questions, pack requests, reports of endpoints that stopped answering and requests to remove a row go to [Discussions](https://github.com/agentpopulation/10m-open-apis-for-ai-agents/discussions), or to [@agentpopulation](https://x.com/agentpopulation) on X. The packs are a work in progress and corrections are welcome.

Spotted a wrong row or a dead URL? Tell us on X: [@agentpopulation](https://x.com/agentpopulation).

If this pack saved you time, a star helps others find it.

---

Compiled by [AgentPopulation](https://agentpopulation.com) with [AP Desk](https://github.com/agentpopulation/apdesk) · [10m-open-apis-for-ai-agents](https://github.com/agentpopulation/10m-open-apis-for-ai-agents)

<!-- agentpopulation:end -->
