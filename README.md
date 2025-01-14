# aqueous-solubility-data

Experimental aqueous solubility data for several hundred inorganic compounds. ata has
been adapted from various references and presented for use in materials informatics.

**Disclaimer**: The data is provided as is and should be used for educational purposes
only. No guarantees are provided for the accuracy of the data.

## Data

### all_solubilities.csv

This is a combined dataset of all the solubility data. It contains the following columns:

- `formula`: The chemical formula of the compound. Note that hydrates are listed as (H2O)$_n$.
- `reduced_formula`: The chemical formula of the compound, processed with pymatgen's *Composition.reduced_formula* method. For example, the reduced formula of "O6Fe4" is "Fe2O3".
- `solubility_XXC`: The solubility of the compound in water at XX degrees Celsius, in
  grams of solute per 100g H2O (i.e., 100 mL).

Data adapted from the raw data sources below.

## Raw Data

### solubilities_raw.csv

solubility.csv contains the following columns:

- `formula`: The chemical formula of the compound
- `reduced_formula`: The chemical formula of the compound, processed with pymatgen's
  *Composition.reduced_formula* method. For example, the reduced formula of "O6Fe4" is
  "Fe2O3".
- `solubility_XXC`: The solubility of the compound in water at XX degrees Celsius, in
  grams of solute per 100g H2O (i.e., 100 mL).

*Data adapted from CRC Handbook of Chemistry and Physics, 91th Edition, 2010, 8-112
through 8-117*.

### solubility_products_raw.csv

This is a dataset of solubility products ($K_{sp}$) for various inorganic compounds. The
solubility products of sulfides are excluded It contains the following columns:

- `compound`: The name of the compound
- `formula`: The chemical formula of the compound
- `reduced_formula`: The chemical formula of the compound, processed with pymatgen's *Composition.reduced_formula* method. For example, the reduced formula of "O6Fe4" is "Fe2O3".
- `ksp_25C`: The solubility product, $K_{sp}$ of the compound at 25ºC.

*Data adapted from CRC Handbook of Chemistry and Physics, 87th Edition, 2006, 8-118 and 8-119*.
