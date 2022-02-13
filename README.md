# Fp Growth Unique Rules
 
The included jupyter notebook purges rules/associations that are duplicates by simple pandas duplication removal procedure. 

# Methodology
The return dataframe from the `association_rules` contains two columns with our original sets of products => `antecedents`  & `consequents`.
The frozensets are first converted into normal sets then merged & sorted stringified.

duplicates are then handled by pandas `drop_duplicates`.

This solution might not work for all scenarios & might also have performance issues with 1000's of products and sales overtime.
