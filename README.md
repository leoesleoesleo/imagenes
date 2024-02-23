WITH CTE AS (
    SELECT
        llave,
        tabla,
        ROW_NUMBER() OVER (PARTITION BY llave ORDER BY tabla) AS row_num
    FROM
        stgcri.cif
)
SELECT
    llave,
    tabla,
    llave AS codigo_cif,
    campo
FROM
    CTE
WHERE
    row_num = 1;
