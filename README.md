# Beauty-Carefree-Giants
DBA Assignment

## Which commands caused errors, and why?

UPDATE WORD_REL
SET SYN_COL = 'blithe'
WHERE WORD = 'insouciant';

Resulted in a error saying: Error at line 2/5: ORA-42399: cannot perform a DML operation on a read-only view. This happened because as the error says, we tried to update a view that was set to read only.

## Why are DML operations restricted in some views?

DML operations are restricted in some views is because the tables are set to read only, they violate any constraints, the tables are non-key preserved, or they use group functions, they use the GROUP BY clause, the ROWNUM column, or the DISTINCT keyword.

## How is a materialized view different from a regular view?

The biggest difference is that while a normal view is completley virtual, a materialized view physically stores the view query results.
