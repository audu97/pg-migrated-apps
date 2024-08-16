# pg-migrated-apps

A collection of applications migrated from PostgreSQL to YugabyteDB.

## Prerequisites

1. Install [PostgreSQL](https://www.postgresql.org/download) or [run in Docker](https://hub.docker.com/_/postgres).
2. Install [YugabyteDB](https://docs.yugabyte.com/preview/quick-start/).
   **NOTE: Be sure to run YugabyteDB with the `--enable_pg_parity_tech_preview` flag**
3. Install [YugabyteDB Voyager](https://docs.yugabyte.com/preview/yugabyte-voyager/install-yb-voyager/).

## Migration Steps

Instructions for migrating and running each _completed_ application are avaialble and linked in the `Instructions` column of the table below. Unless otherwise stated, follow these steps:

### Run on PostgreSQL

1. Start the application on PostgreSQL.
2. Load sample data.
3. Confirm the application is running properly.

### Perform Offline Migration

Use the `yb-voyager` CLI to [perform an offline migration](https://docs.yugabyte.com/preview/yugabyte-voyager/migrate/migrate-steps/).

1. Generate and view migration assessment report.
2. Export the schema and data from PostgreSQL.
3. Import the schema and data to YugabyteDB.
4. Verify the migration was successful by running queries to check row counts.
5. Run the application on YugabyteDB.

### After Migration

1. Fill out application instructions in `/apps/APP_NAME.md`
2. Mark the application migration status in the table below as DONE.

|     | Name                | Description                                                                                                                                                                                        | GitHub                                                                                                                                                                                    | Instructions                                     | Status |
| --- | ------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------ | ------ |
| 1   | FireFly III         | A personal finances manager                                                                                                                                                                        | <a href="https://github.com/firefly-iii/firefly-iii"> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a>      | [Run on YugabyteDB](apps/FireFly-III.md)         |        |
| 2   | Documenso           | The Open Source DocuSign Alternative.                                                                                                                                                              | <a href="https://github.com/documenso/documenso"> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a>          | [Run on YugabyteDB](apps/Documenso.md)           |        |
| 3   | Twenty              | a modern alternative to Salesforce, powered by the community.                                                                                                                                      | <a href="https://github.com/twentyhq/twenty"> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a>              | [Run on YugabyteDB](apps/Twenty.md)              |        |
| 4   | Umami               | A simple, fast, privacy-focused alternative to Google Analytics.                                                                                                                                   | <a href="https://github.com/umami-software/umami"> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a>         | [Run on YugabyteDB](apps/Umami.md)               |        |
| 5   | HedgeDoc            | Was CodiMD: create real-time collaborative markdown notes                                                                                                                                          | <a href="https://github.com/hedgedoc/hedgedoc"> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a>            | [Run on YugabyteDB](apps/HedgeDoc.md)            |        |
| 6   | NocoDB              | An Open Source Alternative to Airtable                                                                                                                                                             | <a href="https://github.com/nocodb/nocodb"> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a>                | [Run on YugabyteDB](apps/NocoDB.md)              |        |
| 7   | Wiki.js             | A modern and powerful wiki app built on Node.js                                                                                                                                                    | <a href="https://github.com/requarks/wiki"> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a>                | [Run on YugabyteDB](apps/Wiki.js.md)             |        |
| 8   | Discourse           | A platform for community discussion. Free, open, simple.                                                                                                                                           | <a href="https://github.com/discourse/discourse"> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a>          | [Run on YugabyteDB](apps/Discourse.md)           |        |
| 9   | Temporal            | Open source durable execution system. Write code that’s fault tolerant, durable, and simple.                                                                                                       | <a href="https://github.com/temporalio/temporal"> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a>          | [Run on YugabyteDB](apps/Temporal.md)            |        |
| 10  | Commento            | A fast, bloat-free comments platform                                                                                                                                                               | <a href="https://github.com/adtac/commento"> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a>               | [Run on YugabyteDB](apps/Commento.md)            | DONE   |
| 11  | Spree               | Online Commerce for Ruby on Rails                                                                                                                                                                  | <a href="https://github.com/spree/spree"> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a>                  | [Run on YugabyteDB](apps/Spree.md)               |        |
| 12  | Redmine             | A flexible project management web application written using Ruby on Rails framework.                                                                                                               | <a href="https://github.com/redmine/redmine"> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a>              | [Run on YugabyteDB](apps/Redmine.md)             |        |
| 13  | Mattermost          | Open source platform that provides secure collaboration for technical and operational teams that work in environments with complex nation-state level security and trust requirements.             | <a href="https://github.com/mattermost/mattermost"> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a>        | [Run on YugabyteDB](apps/Mattermost.md)          |        |
| 14  | Plume               | A a federated blogging engine, based on ActivityPub.                                                                                                                                               | <a href="https://github.com/Plume-org/Plume"> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a>              | [Run on YugabyteDB](apps/Plume.md)               |        |
| 15  | Nocobase            | A scalability-first, open-source no-code/low-code platform to build internal tools.                                                                                                                | <a href="https://github.com/nocobase/nocobase"> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a>            | [Run on YugabyteDB](apps/Nocobase.md)            |        |
| 16  | Invidious           | An alternative front-end to YouTube                                                                                                                                                                | <a href="https://github.com/iv-org/invidious"> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a>             | [Run on YugabyteDB](apps/Invidious.md)           |        |
| 17  | Kine                | Alternative to Etcd. It already works on YugabyteDB - blog and video.                                                                                                                              | <a href="https://github.com/k3s-io/kine"> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a>                  | [Run on YugabyteDB](apps/Kine.md)                |        |
| 18  | AWS data.all        | A modern data marketplace that makes collaboration among diverse users (like business, analysts and engineers) easier, increasing efficiency and agility in data projects on AWS.                  | <a href="https://github.com/data-dot-all/dataall"> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a>         | [Run on YugabyteDB](apps/AWS-data.all.md)        |        |
| 19  | Cachet              | Open-source status page system                                                                                                                                                                     | <a href="https://github.com/cachethq/cachet"> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a>              | [Run on YugabyteDB](apps/Cachet.md)              |        |
| 20  | cal.com             | The open source Calendly alternative, formerly Calendso                                                                                                                                            | <a href="https://github.com/calcom/cal.com"> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a>               | [Run on YugabyteDB](apps/cal.com.md)             |        |
| 21  | Plane               | Open Source JIRA, Linear and Asana Alternative.                                                                                                                                                    | <a href="https://github.com/makeplane/plane"> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a>              | [Run on YugabyteDB](apps/Plane.md)               |        |
| 22  | Quivr               | Open-source RAG Framework                                                                                                                                                                          | <a href="https://github.com/QuivrHQ/quivr"> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a>                | [Run on YugabyteDB](apps/Quivr.md)               |        |
| 23  | Dogehouse           | Taking voice conversations to the moon                                                                                                                                                             | <a href="https://github.com/benawad/dogehouse"> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a>            | [Run on YugabyteDB](apps/Dogehouse.md)           |        |
| 24  | logto               | The better identity infrastructure for developers and the open-source alternative to Auth0.                                                                                                        | <a href="https://github.com/logto-io/logto"> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a>               | [Run on YugabyteDB](apps/logto.md)               |        |
| 25  | teable              | The Next Gen Airtable Alternative: No-Code Postgres                                                                                                                                                | <a href="https://github.com/teableio/teable"> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a>              | [Run on YugabyteDB](apps/teable.md)              |        |
| 26  | mathesar            | Web application providing an intuitive user experience to databases.                                                                                                                               | <a href="https://github.com/mathesar-foundation/mathesar"> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a> | [Run on YugabyteDB](apps/mathesar.md)            |        |
| 27  | bolt                | a simple CMS written in PHP                                                                                                                                                                        | <a href="https://github.com/bolt/bolt?tab=readme-ov-file"> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a> | [Run on YugabyteDB](apps/bolt.md)                |        |
| 28  | waline              | A Simple, Safe Comment System                                                                                                                                                                      | <a href="https://github.com/walinejs/waline"> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a>              | [Run on YugabyteDB](apps/waline.md)              |        |
| 29  | baserow             | an open source no-code database tool and Airtable alternative                                                                                                                                      | <a href="https://github.com/bram2w/baserow"> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a>               | [Run on YugabyteDB](apps/baserow.md)             |        |
| 30  | webapp.rs           | A web application completely written in Rust.                                                                                                                                                      | <a href="https://github.com/saschagrunert/webapp.rs"> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a>      | [Run on YugabyteDB](apps/webapp.rs.md)           |        |
| 31  | metafresh           | Open Source ERP                                                                                                                                                                                    | <a href="https://github.com/metasfresh/metasfresh"> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a>        | [Run on YugabyteDB](apps/metafresh.md)           |        |
| 32  | WrenAI              | Open-source Text-to-SQL solution, Wren AI makes your database RAG-ready                                                                                                                            | <a href="https://github.com/Canner/WrenAI"> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a>                | [Run on YugabyteDB](apps/WrenAI.md)              |        |
| 33  | mybb                | a free and open source forum software.                                                                                                                                                             | <a href="https://github.com/mybb/mybb"> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a>                    | [Run on YugabyteDB](apps/mybb.md)                |        |
| 34  | aquameta            | Web development platform built entirely in PostgreSQL                                                                                                                                              | <a href="https://github.com/aquametalabs/aquameta"> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a>        | [Run on YugabyteDB](apps/aquameta.md)            |        |
| 35  | cocalc              | Collaborative Calculation in the Cloud                                                                                                                                                             | <a href="https://github.com/sagemathinc/cocalc"> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a>           | [Run on YugabyteDB](apps/cocalc.md)              |        |
| 36  | bank                | Full Stack Web Application similar to financial software that is used in banking institutions &#124; React.js and Node.js                                                                          | <a href="https://github.com/pietrzakadrian/bank"> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a>          | [Run on YugabyteDB](apps/bank.md)                |        |
| 37  | zenedo              | a CERN service, is an open dependable home for the long-tail of science, enabling researchers to share and preserve any research outputs in any size, any format and from any science.             | <a href="https://github.com/zenodo/zenodo"> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a>                | [Run on YugabyteDB](apps/zenedo.md)              |        |
| 38  | chatWeb             | ChatWeb can crawl web pages, read PDF, DOCX, TXT, and extract the main content, then answer your questions based on the content, or summarize the key points.                                      | <a href="https://github.com/SkywalkerDarren/chatWeb"> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a>      | [Run on YugabyteDB](apps/chatWeb.md)             |        |
| 39  | Plausible Analytics | Simple, open source, lightweight (< 1 KB) and privacy-friendly web analytics alternative to Google Analytics.                                                                                      | <a href="https://github.com/plausible/analytics"> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a>          | [Run on YugabyteDB](apps/Plausible-Analytics.md) |        |
| 40  | LedgerSMB           | Double-entry accounting & ERP for the web                                                                                                                                                          | <a href=""> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a>                                                | [Run on YugabyteDB](apps/LedgerSMB.md)           |        |
| 41  | Jira                | An agile project management tool used by teams to plan, track, release and support software                                                                                                        | <a href=""> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a>                                                | [Run on YugabyteDB](apps/Jira.md)                |        |
| 42  | Confluence          | A collaborative platform used for creating, sharing, and organizing content within teams and organizations                                                                                         | <a href=""> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a>                                                | [Run on YugabyteDB](apps/Confluence.md)          |        |
| 43  | Puppet              |                                                                                                                                                                                                    | <a href=""> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a>                                                | [Run on YugabyteDB](apps/Puppet.md)              |        |
| 44  | GitLab              |                                                                                                                                                                                                    | <a href=""> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a>                                                | [Run on YugabyteDB](apps/GitLab.md)              |        |
| 45  | Stansoft            |                                                                                                                                                                                                    | <a href=""> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a>                                                | [Run on YugabyteDB](apps/Stansoft.md)            |        |
| 46  | Orthance            | free and open-source, lightweight DICOM server for medical imaging from Belgium.                                                                                                                   | <a href="https://www.orthanc-server.com/download.php"> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a>     | [Run on YugabyteDB](apps/Orthance.md)            |        |
| 47  | NodeBB              | Node.js based forum software built for the modern web                                                                                                                                              | <a href="https://github.com/NodeBB/NodeBB"> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a>                | [Run on YugabyteDB](apps/NodeBB.md)              |        |
| 48  | Evershop            | NodeJS E-commerce Platform                                                                                                                                                                         | <a href="https://github.com/evershopcommerce/evershop"> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a>    | [Run on YugabyteDB](apps/Evershop.md)            |        |
| 49  | Servicebot          | Open-source subscription management & billing automation system                                                                                                                                    | <a href="https://github.com/service-bot/servicebot"> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a>       | [Run on YugabyteDB](apps/Servicebot.md)          |        |
| 50  | Miaou               | A chat server with OAuth2 authentication, persistent and searchable history, video and audio, markdown formatting, private and public rooms, stars, votes, embedded games, and many other features | <a href="https://github.com/Canop/miaou"> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a>                  | [Run on YugabyteDB](apps/Miaou.md)               |        |
| 51  | Tasking Manager     | The app to team up for mapping in OpenStreetMap                                                                                                                                                    | <a href="https://github.com/hotosm/tasking-manager"> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a>       | [Run on YugabyteDB](apps/Tasking-Manager.md)     |        |
| 52  | FeedHQ              | FeedHQ is a web-based feed reader                                                                                                                                                                  | <a href="https://github.com/feedhq/feedhq"> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a>                | [Run on YugabyteDB](apps/FeedHQ.md)              |        |
| 53  | Open EduCat         | Comprehensive Open Source ERP for Educational Institutes                                                                                                                                           | <a href="https://github.com/openeducat/openeducat_erp"> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a>    | [Run on YugabyteDB](apps/Open-EduCat.md)         |        |
| 54  | SQL Translator      | SQL Translator is a tool for converting natural language queries into SQL code using artificial intelligence. This project is 100% free and open source.                                           | <a href="https://github.com/whoiskatrin/sql-translator"> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a>   | [Run on YugabyteDB](apps/SQL-Translator.md)      |        |
| 55  | Papermark           | Papermark is the open-source DocSend alternative with built-in analytics and custom domains.                                                                                                       | <a href="https://github.com/mfts/papermark"> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a>               | [Run on YugabyteDB](apps/Papermark.md)           |        |
| 56  | Saasfly             | Your Next SaaS Template or Boilerplate ! A magic trip start with `bun create saasfly` . The more stars, the more surprises                                                                         | <a href="https://github.com/saasfly/saasfly"> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a>              | [Run on YugabyteDB](apps/Saasfly.md)             |        |
| 57  | Worklenz            | All in one project management tool for efficient teams                                                                                                                                             | <a href="https://github.com/Worklenz/worklenz"> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a>            | [Run on YugabyteDB](apps/Worklenz.md)            |        |
| 58  | Picsur              | An easy to use, selfhostable image sharing service like Imgur with built in converting                                                                                                             | <a href="https://github.com/CaramelFur/Picsur"> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a>            | [Run on YugabyteDB](apps/Picsur.md)              |        |
| 59  | Miniflux/v2         | Minimalist and opinionated feed reader                                                                                                                                                             | <a href="https://github.com/miniflux/v2"> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a>                  | [Run on YugabyteDB](apps/Miniflux-v2.md)         |        |
| 60  | Goxygen             | Generate a modern Web project with Go and Angular, React, or Vue in seconds                                                                                                                        | <a href="https://github.com/Shpota/goxygen"> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a>               | [Run on YugabyteDB](apps/Goxygen.md)             |        |
| 61  | short               | URL shortening service written in Go and React                                                                                                                                                     | <a href="https://github.com/short-d/short"> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a>                | [Run on YugabyteDB](apps/short.md)               |        |
| 62  | maybe               | The OS for your personal finances                                                                                                                                                                  | <a href="https://github.com/maybe-finance/maybe"> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a>          | [Run on YugabyteDB](apps/maybe.md)               |        |
| 63  | windmill            | Open-source developer platform to turn scripts into workflows and UIs. Fastest workflow engine (5x vs Airflow). Open-source alternative to Airplane and Retool.                                    | <a href="https://github.com/windmill-labs/windmill"> <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="30" height="30"> </a>       | [Run on YugabyteDB](apps/windmill.md)            |        |
