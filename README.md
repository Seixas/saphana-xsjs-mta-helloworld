workflow
-HDB creation
--architect entities
--create VIEW
--add Projection mapping correct cloumns

-js module
--XSJS compatible?

-HTML module

INSERT INTO "projectName_HDI_nameOfDB_16"."tinyworld.tinydb::tinyf.world" VALUES ('Europe');
INSERT INTO "projectName_HDI_nameOfDB_16"."tinyworld.tinydb::tinyf.world" VALUES ('Asia');
INSERT INTO "projectName_HDI_nameOfDB_16"."tinyworld.tinydb::tinyf.country" VALUES ('Spain', 'Europe');
INSERT INTO "projectName_HDI_nameOfDB_16"."tinyworld.tinydb::tinyf.country" VALUES ('Japan', 'Asia');
INSERT INTO "projectName_HDI_nameOfDB_16"."tinyworld.tinydb::tinyf.country" VALUES ('Denmark', 'Europe');

#checking
SELECT * FROM "projectName_HDI_nameOfDB_16"."tinyworld.tinydb::tinyf.country" WHERE "partof.continent" = 'Europe'