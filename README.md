workflow(using xsjs)
-HDB creation
--architect entities
--create VIEW
--add Projection mapping correct cloumns

-js module
--XSJS compatible?

-HTML module
--we need to map our routes[] at xs-app.json, ex.: {“source”: “^/xsjsOdataServiceName.xsodata/.*$”, “destination”: “moduleNamejs_be”}

-XSOData file
--expose modules through mta.yaml aka provide a url of js_api and requires our DB hdi-container
--expose api for our UI module in mta.yaml that requires moduleNamejs_api with group destinations and name/url properties(good pratical naming js_be for back-end)

INSERT INTO "projectName_HDI_nameOfDB_16"."tinyworld.tinydb::tinyf.world" VALUES ('Europe');
INSERT INTO "projectName_HDI_nameOfDB_16"."tinyworld.tinydb::tinyf.world" VALUES ('Asia');
INSERT INTO "projectName_HDI_nameOfDB_16"."tinyworld.tinydb::tinyf.country" VALUES ('Spain', 'Europe');
INSERT INTO "projectName_HDI_nameOfDB_16"."tinyworld.tinydb::tinyf.country" VALUES ('Japan', 'Asia');
INSERT INTO "projectName_HDI_nameOfDB_16"."tinyworld.tinydb::tinyf.country" VALUES ('Denmark', 'Europe');

#checking
SELECT * FROM "projectName_HDI_nameOfDB_16"."tinyworld.tinydb::tinyf.country" WHERE "partof.continent" = 'Europe'