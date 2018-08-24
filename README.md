# sql-study

LEFT JOIN must have joined table's alias

SELECT COUNT(*) FROM intent_example IE LEFT JOIN (SELECT I.id FROM intent I LEFT JOIN (SELECT D.id FROM domain D WHERE D.bot_id = 1) DJ ON I.domain_id = DJ.id) IJ ON IE.intent_id = IJ.id
