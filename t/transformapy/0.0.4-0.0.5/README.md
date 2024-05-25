# Comparing `tmp/transformapy-0.0.4.zip` & `tmp/transformapy-0.0.5.zip`

## zipinfo {}

```diff
@@ -1,15 +1,16 @@
-Zip file size: 26495 bytes, number of entries: 13
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-09 16:06 transformapy-0.0.4/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-09 16:06 transformapy-0.0.4/transformapy.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-09 16:06 transformapy-0.0.4/transformapy/
--rw-r--r--  2.0 unx     5097 b- defN 24-Apr-09 16:06 transformapy-0.0.4/PKG-INFO
--rwx------  2.0 unx      743 b- defN 24-Apr-09 16:04 transformapy-0.0.4/setup.py
--rw-r--r--  2.0 unx       38 b- defN 24-Apr-09 16:06 transformapy-0.0.4/setup.cfg
--rwx------  2.0 unx     3827 b- defN 24-Apr-09 16:04 transformapy-0.0.4/README.rst
--rw-r--r--  2.0 unx     5097 b- defN 24-Apr-09 16:06 transformapy-0.0.4/transformapy.egg-info/PKG-INFO
--rw-r--r--  2.0 unx      217 b- defN 24-Apr-09 16:06 transformapy-0.0.4/transformapy.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx       13 b- defN 24-Apr-09 16:06 transformapy-0.0.4/transformapy.egg-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 24-Apr-09 16:06 transformapy-0.0.4/transformapy.egg-info/dependency_links.txt
--rwx------  2.0 unx      892 b- defN 24-Apr-09 10:48 transformapy-0.0.4/transformapy/__init__.py
--rwx------  2.0 unx    71862 b- defN 24-Apr-09 10:45 transformapy-0.0.4/transformapy/transformapy.py
-13 files, 87787 bytes uncompressed, 24467 bytes compressed:  72.1%
+Zip file size: 31036 bytes, number of entries: 14
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-25 22:01 transformapy-0.0.5/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-25 22:01 transformapy-0.0.5/transformapy.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-25 22:01 transformapy-0.0.5/transformapy/
+-rw-r--r--  2.0 unx     5490 b- defN 24-May-25 22:01 transformapy-0.0.5/PKG-INFO
+-rwx------  2.0 unx      758 b- defN 24-May-25 21:46 transformapy-0.0.5/setup.py
+-rw-r--r--  2.0 unx       38 b- defN 24-May-25 22:01 transformapy-0.0.5/setup.cfg
+-rwx------  2.0 unx     4140 b- defN 24-May-25 21:53 transformapy-0.0.5/README.rst
+-rw-r--r--  2.0 unx     5490 b- defN 24-May-25 22:01 transformapy-0.0.5/transformapy.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx      252 b- defN 24-May-25 22:01 transformapy-0.0.5/transformapy.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx       14 b- defN 24-May-25 22:01 transformapy-0.0.5/transformapy.egg-info/requires.txt
+-rw-r--r--  2.0 unx       13 b- defN 24-May-25 22:01 transformapy-0.0.5/transformapy.egg-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-May-25 22:01 transformapy-0.0.5/transformapy.egg-info/dependency_links.txt
+-rwx------  2.0 unx     1085 b- defN 24-May-25 21:36 transformapy-0.0.5/transformapy/__init__.py
+-rwx------  2.0 unx    91087 b- defN 24-May-25 21:34 transformapy-0.0.5/transformapy/transformapy.py
+14 files, 108368 bytes uncompressed, 28826 bytes compressed:  73.4%
```

## zipnote {}

```diff
@@ -1,40 +1,43 @@
-Filename: transformapy-0.0.4/
+Filename: transformapy-0.0.5/
 Comment: 
 
-Filename: transformapy-0.0.4/transformapy.egg-info/
+Filename: transformapy-0.0.5/transformapy.egg-info/
 Comment: 
 
-Filename: transformapy-0.0.4/transformapy/
+Filename: transformapy-0.0.5/transformapy/
 Comment: 
 
-Filename: transformapy-0.0.4/PKG-INFO
+Filename: transformapy-0.0.5/PKG-INFO
 Comment: 
 
-Filename: transformapy-0.0.4/setup.py
+Filename: transformapy-0.0.5/setup.py
 Comment: 
 
-Filename: transformapy-0.0.4/setup.cfg
+Filename: transformapy-0.0.5/setup.cfg
 Comment: 
 
-Filename: transformapy-0.0.4/README.rst
+Filename: transformapy-0.0.5/README.rst
 Comment: 
 
-Filename: transformapy-0.0.4/transformapy.egg-info/PKG-INFO
+Filename: transformapy-0.0.5/transformapy.egg-info/PKG-INFO
 Comment: 
 
-Filename: transformapy-0.0.4/transformapy.egg-info/SOURCES.txt
+Filename: transformapy-0.0.5/transformapy.egg-info/SOURCES.txt
 Comment: 
 
-Filename: transformapy-0.0.4/transformapy.egg-info/top_level.txt
+Filename: transformapy-0.0.5/transformapy.egg-info/requires.txt
 Comment: 
 
-Filename: transformapy-0.0.4/transformapy.egg-info/dependency_links.txt
+Filename: transformapy-0.0.5/transformapy.egg-info/top_level.txt
 Comment: 
 
-Filename: transformapy-0.0.4/transformapy/__init__.py
+Filename: transformapy-0.0.5/transformapy.egg-info/dependency_links.txt
 Comment: 
 
-Filename: transformapy-0.0.4/transformapy/transformapy.py
+Filename: transformapy-0.0.5/transformapy/__init__.py
+Comment: 
+
+Filename: transformapy-0.0.5/transformapy/transformapy.py
 Comment: 
 
 Zip file comment:
```

## Comparing `transformapy-0.0.4/PKG-INFO` & `transformapy-0.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: transformapy
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Toolkit for Identifying Transformation Product Structures of Emerging Contaminants Using HRMS Data
 Home-page: https://github.com/WangRui5/TransformaPy
 Author: Wang Rui
 Author-email: wtrt7009@gmail.com
 License: UNKNOWN
 Description: transformapy: A Toolkit for Identifying Transformation Product Structures of Emerging Contaminants Using HRMS Data
         ==================================================================================================================
@@ -15,15 +15,15 @@
         =====================
         
         First release date: Feb.28.2024
         
         Update
         ======
         
-        April.09.2024: transformapy 0.0.4
+        April.09.2024: transformapy 0.0.5
         
         1. **Updated `remove_2H` Function**: Modifications have been made to improve the performance and accuracy of the `remove_2H` function.
         2. **New Helper Functions**: Added `check_bad_valance_Hidx` and `remove_additional_H` functions, which are now utilized internally by `remove_2H` to enhance its functionality.
         3. **Added `add_missing_H` Function**: Introduced a new function to automatically add missing hydrogen atoms to molecules to correct their valency.
         4. **Enhanced `reaction_type` Checks**: Integrated the `add_missing_H` and `remove_additional_H` functions into the `reaction_type` function to ensure molecule structures are correctly adjusted during reactions.
         5. **Introduced `stepwise_reaction` Function**: A new function to facilitate the stepwise application of reaction steps on a target molecule, allowing more detailed control over complex reaction pathways.
         6. **Improvements to `generate_possible_TP_structures`**: Significant updates have been made to this function to optimize the generation of possible transformation product structures based on modified chemical reaction processes.
@@ -64,36 +64,46 @@
             from transformapy.transformapy import *
         
         **Project Structure:**
         
         .. code-block:: none
         
             transformapy/
+            Step 1:
             |- from_mass_to_formula
-            |- generate_possible_TP_structures
-               |- modify_chemical_formula
-               |- generate_fragments
-               |- calculate_formula_differences
-               |- combine_two_frags
-               |- calculate_changed_num
-                  |- parse_formula
-               |- stepwise_reaction
-                  |- reaction_type
-                     |- combine_fragments_and_generate_smiles
-                     |- replace_dummies_with_hydrogens
-                     |- replace_hydrogen_with_substituent
-                     |- split_molecule_at_bond
-                     |- Remove_2H
-                        |- is_atom_in_double_bond
-                        |- add_or_modify_bond
-                        |- has_hydrogen_count
-                     |- Add_2H
-                     |- remove_additional_H
-                        |- check_bad_valance_Hidx
-                     |- add_missing_H
+               |- get_formula_elements_range
+        
+            Step 2:
+            ｜- unfold_formula_result
+        
+            Step 3:
+            |- generate_possible_TP_structures_to_df
+               |- generate_possible_TP_structures
+                  |- modify_chemical_formula
+                  |- generate_fragments
+                  |- calculate_formula_differences
+                  |- combine_two_frags
+                  |- calculate_changed_num
+                     |- parse_formula
+                  |- stepwise_reaction_single_tp
+                     |- one_step_reaction_based_on_fp
+                        |- reaction_type
+                           |- combine_fragments_and_generate_smiles
+                           |- replace_dummies_with_hydrogens
+                           |- replace_hydrogen_with_substituent
+                           |- split_molecule_at_bond
+                           |- Remove_2H
+                              |- is_atom_in_double_bond
+                              |- add_or_modify_bond
+                              |- has_hydrogen_count
+                           |- Add_2H
+                           |- remove_additional_H
+                              |- check_bad_valance_Hidx
+                           |- add_missing_H
+           
             |- remove_explicit_hydrogens
             |- draw_molecule_with_atom_indices
             |- GetIdxOfDummy
             |- adjust_valence_by_removing_hydrogen
         
         Acknowledgment
         ==============
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## Comparing `transformapy-0.0.4/setup.py` & `transformapy-0.0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 
 def readme_file():
     with open('README.rst') as rf:
         return rf.read()
 
 setuptools.setup(
     name = 'transformapy',
-    version = '0.0.4',
+    version = '0.0.5',
     author = 'Wang Rui',
     author_email = 'wtrt7009@gmail.com',
     url = 'https://github.com/WangRui5/TransformaPy',
     description = 'A Toolkit for Identifying Transformation Product Structures of Emerging Contaminants Using HRMS Data',
     long_description = readme_file(),
     packages = setuptools.find_packages(),
-    install_requires = [],
+    install_requires = ['pyhrms>=0.9.2'],
     classifiers = [
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
```

## Comparing `transformapy-0.0.4/README.rst` & `transformapy-0.0.5/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 =====================
 
 First release date: Feb.28.2024
 
 Update
 ======
 
-April.09.2024: transformapy 0.0.4
+April.09.2024: transformapy 0.0.5
 
 1. **Updated `remove_2H` Function**: Modifications have been made to improve the performance and accuracy of the `remove_2H` function.
 2. **New Helper Functions**: Added `check_bad_valance_Hidx` and `remove_additional_H` functions, which are now utilized internally by `remove_2H` to enhance its functionality.
 3. **Added `add_missing_H` Function**: Introduced a new function to automatically add missing hydrogen atoms to molecules to correct their valency.
 4. **Enhanced `reaction_type` Checks**: Integrated the `add_missing_H` and `remove_additional_H` functions into the `reaction_type` function to ensure molecule structures are correctly adjusted during reactions.
 5. **Introduced `stepwise_reaction` Function**: A new function to facilitate the stepwise application of reaction steps on a target molecule, allowing more detailed control over complex reaction pathways.
 6. **Improvements to `generate_possible_TP_structures`**: Significant updates have been made to this function to optimize the generation of possible transformation product structures based on modified chemical reaction processes.
@@ -56,36 +56,46 @@
     from transformapy.transformapy import *
 
 **Project Structure:**
 
 .. code-block:: none
 
     transformapy/
+    Step 1:
     |- from_mass_to_formula
-    |- generate_possible_TP_structures
-       |- modify_chemical_formula
-       |- generate_fragments
-       |- calculate_formula_differences
-       |- combine_two_frags
-       |- calculate_changed_num
-          |- parse_formula
-       |- stepwise_reaction
-          |- reaction_type
-             |- combine_fragments_and_generate_smiles
-             |- replace_dummies_with_hydrogens
-             |- replace_hydrogen_with_substituent
-             |- split_molecule_at_bond
-             |- Remove_2H
-                |- is_atom_in_double_bond
-                |- add_or_modify_bond
-                |- has_hydrogen_count
-             |- Add_2H
-             |- remove_additional_H
-                |- check_bad_valance_Hidx
-             |- add_missing_H
+       |- get_formula_elements_range
+
+    Step 2:
+    ｜- unfold_formula_result
+
+    Step 3:
+    |- generate_possible_TP_structures_to_df
+       |- generate_possible_TP_structures
+          |- modify_chemical_formula
+          |- generate_fragments
+          |- calculate_formula_differences
+          |- combine_two_frags
+          |- calculate_changed_num
+             |- parse_formula
+          |- stepwise_reaction_single_tp
+             |- one_step_reaction_based_on_fp
+                |- reaction_type
+                   |- combine_fragments_and_generate_smiles
+                   |- replace_dummies_with_hydrogens
+                   |- replace_hydrogen_with_substituent
+                   |- split_molecule_at_bond
+                   |- Remove_2H
+                      |- is_atom_in_double_bond
+                      |- add_or_modify_bond
+                      |- has_hydrogen_count
+                   |- Add_2H
+                   |- remove_additional_H
+                      |- check_bad_valance_Hidx
+                   |- add_missing_H
+   
     |- remove_explicit_hydrogens
     |- draw_molecule_with_atom_indices
     |- GetIdxOfDummy
     |- adjust_valence_by_removing_hydrogen
 
 Acknowledgment
 ==============
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## Comparing `transformapy-0.0.4/transformapy.egg-info/PKG-INFO` & `transformapy-0.0.5/transformapy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: transformapy
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Toolkit for Identifying Transformation Product Structures of Emerging Contaminants Using HRMS Data
 Home-page: https://github.com/WangRui5/TransformaPy
 Author: Wang Rui
 Author-email: wtrt7009@gmail.com
 License: UNKNOWN
 Description: transformapy: A Toolkit for Identifying Transformation Product Structures of Emerging Contaminants Using HRMS Data
         ==================================================================================================================
@@ -15,15 +15,15 @@
         =====================
         
         First release date: Feb.28.2024
         
         Update
         ======
         
-        April.09.2024: transformapy 0.0.4
+        April.09.2024: transformapy 0.0.5
         
         1. **Updated `remove_2H` Function**: Modifications have been made to improve the performance and accuracy of the `remove_2H` function.
         2. **New Helper Functions**: Added `check_bad_valance_Hidx` and `remove_additional_H` functions, which are now utilized internally by `remove_2H` to enhance its functionality.
         3. **Added `add_missing_H` Function**: Introduced a new function to automatically add missing hydrogen atoms to molecules to correct their valency.
         4. **Enhanced `reaction_type` Checks**: Integrated the `add_missing_H` and `remove_additional_H` functions into the `reaction_type` function to ensure molecule structures are correctly adjusted during reactions.
         5. **Introduced `stepwise_reaction` Function**: A new function to facilitate the stepwise application of reaction steps on a target molecule, allowing more detailed control over complex reaction pathways.
         6. **Improvements to `generate_possible_TP_structures`**: Significant updates have been made to this function to optimize the generation of possible transformation product structures based on modified chemical reaction processes.
@@ -64,36 +64,46 @@
             from transformapy.transformapy import *
         
         **Project Structure:**
         
         .. code-block:: none
         
             transformapy/
+            Step 1:
             |- from_mass_to_formula
-            |- generate_possible_TP_structures
-               |- modify_chemical_formula
-               |- generate_fragments
-               |- calculate_formula_differences
-               |- combine_two_frags
-               |- calculate_changed_num
-                  |- parse_formula
-               |- stepwise_reaction
-                  |- reaction_type
-                     |- combine_fragments_and_generate_smiles
-                     |- replace_dummies_with_hydrogens
-                     |- replace_hydrogen_with_substituent
-                     |- split_molecule_at_bond
-                     |- Remove_2H
-                        |- is_atom_in_double_bond
-                        |- add_or_modify_bond
-                        |- has_hydrogen_count
-                     |- Add_2H
-                     |- remove_additional_H
-                        |- check_bad_valance_Hidx
-                     |- add_missing_H
+               |- get_formula_elements_range
+        
+            Step 2:
+            ｜- unfold_formula_result
+        
+            Step 3:
+            |- generate_possible_TP_structures_to_df
+               |- generate_possible_TP_structures
+                  |- modify_chemical_formula
+                  |- generate_fragments
+                  |- calculate_formula_differences
+                  |- combine_two_frags
+                  |- calculate_changed_num
+                     |- parse_formula
+                  |- stepwise_reaction_single_tp
+                     |- one_step_reaction_based_on_fp
+                        |- reaction_type
+                           |- combine_fragments_and_generate_smiles
+                           |- replace_dummies_with_hydrogens
+                           |- replace_hydrogen_with_substituent
+                           |- split_molecule_at_bond
+                           |- Remove_2H
+                              |- is_atom_in_double_bond
+                              |- add_or_modify_bond
+                              |- has_hydrogen_count
+                           |- Add_2H
+                           |- remove_additional_H
+                              |- check_bad_valance_Hidx
+                           |- add_missing_H
+           
             |- remove_explicit_hydrogens
             |- draw_molecule_with_atom_indices
             |- GetIdxOfDummy
             |- adjust_valence_by_removing_hydrogen
         
         Acknowledgment
         ==============
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## Comparing `transformapy-0.0.4/transformapy/__init__.py` & `transformapy-0.0.5/transformapy/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from . import transformapy
 
-__version__ = "0.0.4"
+__version__ = "0.0.5"
 
 __all__ = [
+
     "generate_possible_TP_structures",
     "modify_chemical_formula",
     "generate_fragments",
     "split_peak_picking",
     "calculate_formula_differences",
     "calculate_changed_num",
     "parse_formula",
@@ -26,9 +27,17 @@
     "GetIdxOfDummy",
     "adjust_valence_by_removing_hydrogen",
     "add_missing_H",
     "check_bad_valance_Hidx",
     "remove_additional_H",
     "stepwise_reaction",
     "from_mass_to_formula",
-    "is_valid_formula"
+    "is_valid_formula",
+    "generate_possible_TP_structures_to_df",
+    "get_formula_elements_range",
+    "one_step_reaction_based_on_fp",
+    "stepwise_reaction_single_tp",
+    "unfold_formula_result"
+
+
+
 ]
```

## Comparing `transformapy-0.0.4/transformapy/transformapy.py` & `transformapy-0.0.5/transformapy/transformapy.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,523 @@
 from collections import defaultdict
 import itertools
 import re
 from rdkit.Chem.Draw import rdMolDraw2D
 from IPython.display import SVG
 import rdkit
 from pyhrms.pyhrms import *
+from rdkit.DataStructs import FingerprintSimilarity
+
+
+def generate_possible_TP_structures_to_df(unfold_result,parent_mol, neutral_formula_column = 'neutral_formula'):
+    """
+    Generates possible transformation product (TP) structures by modifying a parent molecule
+    based on the neutral formulas in a DataFrame.
+
+    This function iterates over each row in the input DataFrame, generates possible transformation
+    product (TP) structures for each neutral formula, and appends the resulting intermediate structure,
+    element changes, reaction steps, and final TP structure to the DataFrame.
+
+    Parameters:
+    - unfold_result (pd.DataFrame): A DataFrame containing the neutral formulas.
+    - parent_mol (Chem.Mol): The RDKit molecule object representing the parent molecule.
+    - neutral_formula_column (str): The column name containing the neutral formulas. Default is 'neutral_formula'.
+
+    Returns:
+    - pd.DataFrame: The input DataFrame with added columns for intermediate structure, element changes,
+      reaction steps, and final TP structure.
+
+    The added columns:
+    - 'intermediate': The SMILES string of the intermediate structure.
+    - 'element_change': A string representation of the element changes from the intermediate to the final TP.
+    - 'rxn_steps': A string representation of the reaction steps to convert the intermediate to the final TP.
+    - 'tp_structure': The SMILES string of the final transformation product.
+
+    Steps:
+    1. Iterate over each row in the DataFrame to obtain the neutral formula.
+    2. If the neutral formula is valid and not empty, generate possible TP structures using the 
+       `generate_possible_TP_structures` function.
+    3. Append the resulting intermediate structure, element changes, reaction steps, and final TP 
+       structure to the corresponding columns in the DataFrame.
+    4. Return the updated DataFrame.
+
+    Note:
+    - The neutral formula column in the input DataFrame should contain valid chemical formula strings.
+    - The generated TP structures are theoretical and may require further validation to ensure their 
+      chemical plausibility.
+    """
+    for i in tqdm(range(len(unfold_result)),desc = 'Processing molecular structures'):
+        neutral_formula = unfold_result.loc[i,neutral_formula_column]
+        if isinstance(neutral_formula,str)&(neutral_formula!='[]'):
+            intermediate,element_change, rxn_steps,final_tp = generate_possible_TP_structures(parent_mol,neutral_formula)
+            unfold_result.loc[i,'intermediate'] = intermediate
+            unfold_result.loc[i,'element_change'] = element_change
+            unfold_result.loc[i,'rxn_steps'] = rxn_steps
+            unfold_result.loc[i,'tp_structure'] = final_tp
+    return unfold_result
+
+
+
+def combine_fragments_and_generate_smiles(fragment1_smiles, fragment2_smiles, fragment1_connect_atom_idx,
+                                          fragment2_connect_atom_idx):
+    """
+    Combines two molecular fragments, represented by their SMILES strings, into a single molecule by forming a bond
+    between specified atoms from each fragment.
+
+    This function takes the SMILES strings of two molecular fragments and the indices of the atoms (within each fragment)
+    that should be connected. It then combines these fragments into a single molecule by forming a single bond between
+    the specified atoms. The resulting molecule is returned as a SMILES string.
+
+    Parameters:
+    - fragment1_smiles (str): The SMILES string representing the first molecular fragment.
+    - fragment2_smiles (str): The SMILES string representing the second molecular fragment.
+    - fragment1_connect_atom_idx (int): The zero-based index of the atom in the first fragment to be connected.
+    - fragment2_connect_atom_idx (int): The zero-based index of the atom in the second fragment to be connected.
+
+    Returns:
+    - str: The SMILES string representing the combined molecule after connecting the specified atoms.
+
+    Example:
+    >>> combine_fragments_and_generate_smiles('CCO', 'N', 2, 0)
+    'CCON'
+
+    Note:
+    - The indices of the connecting atoms are based on the order of atoms in their respective SMILES strings.
+    - The function assumes valid SMILES strings and valid atom indices are provided. Invalid inputs may lead to
+      unexpected results or errors.
+    - The bond formed between the fragments is a single bond. Modifications are needed to form other types of bonds.
+    - If the specified atom in the first fragment does not have any hydrogen atoms available for bonding,
+      the function will search for another atom with available hydrogen atoms in the combined molecule.
+    """
+    # Create molecule objects from the SMILES strings
+    fragment1_mol = Chem.MolFromSmiles(fragment1_smiles)
+    fragment2_mol = Chem.MolFromSmiles(fragment2_smiles)
+    
+    # Combine the molecules
+    combined_mol = rdmolops.CombineMols(fragment1_mol, fragment2_mol)
+    
+    # 检查combined 之后原来的结构是否还有H
+    atom = combined_mol.GetAtomWithIdx(fragment1_connect_atom_idx)
+    if has_hydrogen_count(atom):
+        pass
+    else:
+        for atom in combined_mol.GetAtoms():
+            if has_hydrogen_count(atom):
+                fragment1_connect_atom_idx = atom.GetIdx()
+                break
+    # Create an editable molecule for further modifications
+    editable_mol = Chem.EditableMol(combined_mol)
+
+    # Calculate the index of the first atom in fragment2 within the combined molecule
+    fragment2_start_idx = fragment1_mol.GetNumAtoms()
+
+    # Add a bond between the specified atoms
+    # The index of the connecting atom in fragment2 needs to be adjusted to its new index in the combined molecule
+    editable_mol.AddBond(fragment1_connect_atom_idx, fragment2_start_idx + fragment2_connect_atom_idx,
+                         order=Chem.rdchem.BondType.SINGLE)
+
+    # Convert back to a regular Mol object
+    final_mol = editable_mol.GetMol()
+
+    for atom in final_mol.GetAtoms():
+        atom.SetNumExplicitHs(0)
+        
+    # try:
+    smi1 = Chem.MolToSmiles(final_mol)
+    final_mol = Chem.MolFromSmiles(smi1)
+    # Sanitize the molecule
+    Chem.SanitizeMol(final_mol) # new test
+
+    # Generate and return the SMILES of the combined molecule
+    final_smiles = Chem.MolToSmiles(final_mol, isomericSmiles=True)
+    return final_smiles
+
+
+def get_formula_elements_range(parent_mol,max_mz,min_mz,addition_element = {}):
+    """
+    Get the reasonable atoms and their quantity ranges based on the parent molecule
+    and the specified m/z range.
+
+    Args:
+        parent_mol (Mol): The parent molecule for which to calculate the atom ranges.
+        max_mz (float): The maximum m/z value to predict.
+        min_mz (float): The minimum m/z value to predict. If only one m/z value is used,
+                        set min_mz equal to max_mz.
+        addition_element (dict, optional): Additional atoms and their ranges to include
+                                           in the prediction. Defaults to an empty dictionary.
+
+    Returns:
+        tuple: A tuple containing:
+            - atoms (list): List of atom symbols.
+            - atom_n (list): List of tuples representing the range (min, max) for each atom's count.
+    """
+    # 获得基础信息
+    parent_formula = CalcMolFormula(parent_mol)
+    formula_dict = parse_formula(parent_formula)
+    atoms = [k for k, v in formula_dict.items()] + [k for k, v in addition_element.items()]
+    
+
+    # 获得检索的元素和数量范围
+    max_C = int(max_mz / 14)  # 考虑CnH2n+2
+    min_C = int(min_mz / 100)  # 考虑C-I
+    atom_n = []
+    for k, v in formula_dict.items():
+        if k == 'C':
+            atom_n.append([min_C, max_C])
+        elif k == 'H':
+            atom_n.append([max(min_C * 2 + 2, v - 20), v + 20])
+        elif k == 'N':
+            atom_n.append([max(0, v - 10), v + 5])
+        elif k == 'O':
+            atom_n.append([max(0, v - 10), v + 10])
+        elif k == 'P':
+            atom_n.append([max(0, v - 5), v + 2])
+        elif k == 'S':
+            atom_n.append([max(0, v - 5), v + 2])
+        else:
+            atom_n.append([0, v])
+    atom_n = atom_n + [[0, v] for k, v in addition_element.items()]
+    return atoms, atom_n
+
+def one_step_reaction_based_on_fp(target_mol, rxn_type,num, parent_fp):
+    """
+    Performs a single reaction step on a target molecule based on a specified reaction type and
+    number of transformations, then selects the most similar product to the parent molecule based
+    on fingerprint similarity.
+
+    This function applies a specified reaction to a target molecule, generating a list of possible
+    transformation products. It then calculates the fingerprint similarity between each product
+    and the parent molecule, and returns the product with the highest similarity.
+
+    Parameters:
+    - target_mol (Chem.Mol): The RDKit molecule object representing the target molecule.
+    - rxn_type (str): The type of reaction to apply (e.g., 'NH', 'O', 'CH2').
+    - num (int): The number of transformations to apply for the reaction type.
+    - parent_fp (rdkit.DataStructs.cDataStructs.ExplicitBitVect): The fingerprint of the parent molecule for similarity comparison.
+
+    Returns:
+    - Chem.Mol: The RDKit molecule object representing the most similar product after the reaction step,
+      or None if no valid products are generated.
+
+    Example:
+    >>> parent_fp = AllChem.GetMorganFingerprintAsBitVect(parent_mol, 2, nBits=1024)
+    >>> one_step_reaction_based_on_fp(target_mol, 'NH', 1, parent_fp)
+    """
+    tps1 = reaction_type(target_mol, rxn_type=rxn_type, num=num)
+    if len(tps1)> 1:
+        tp_fps = [AllChem.GetMorganFingerprintAsBitVect(target_mol, 2, nBits=1024) for target_mol in tps1]
+        tp_list_similarity = [ FingerprintSimilarity(parent_fp, tp_fp) for tp_fp in tp_fps]
+        combined = list(zip(tps1,tp_list_similarity))
+        sorted_combined = sorted(combined, key=lambda x: x[1],reverse = True)
+        tps1,tp_list_similarity = zip(*sorted_combined)
+        tp_1st_step = tps1[0]
+    elif len(tps1) == 1:
+        tp_1st_step = tps1[0]
+    else:
+        tp_1st_step = None
+    return tp_1st_step
+
+def stepwise_reaction_single_tp(target_mol, rxn_s1,parent_mol):
+    """
+    Applies a series of reactions stepwise to a target molecule, selecting the most similar product
+    to the parent molecule at each step based on fingerprint similarity.
+
+    This function iteratively applies a series of specified reactions to a target molecule. At each
+    step, it selects the most similar product to the parent molecule based on fingerprint similarity.
+    The process continues until all reactions are applied or no valid products are generated.
+
+    Parameters:
+    - target_mol (Chem.Mol): The RDKit molecule object representing the initial target molecule.
+    - rxn_s1 (dict): A dictionary where keys are reaction types and values are the number of transformations
+      to apply for each reaction type.
+    - parent_mol (Chem.Mol): The RDKit molecule object representing the parent molecule.
+
+    Returns:
+    - Chem.Mol: The RDKit molecule object representing the final transformation product after all reaction steps,
+      or None if no valid products are generated.
+
+    Example:
+    >>> rxn_s1 = {'NH': 1, 'O': 1}
+    >>> stepwise_reaction_single_tp(target_mol, rxn_s1, parent_mol)
+    """
+    final_tp = target_mol
+    if len(rxn_s1)>=1:
+        parent_fp = AllChem.GetMorganFingerprintAsBitVect(parent_mol, 2, nBits=1024)
+        # 1. 先把有多少步反应讲清楚
+        dict1 = rxn_s1
+        keys_list = []
+        values_list = []
+        for key, value in dict1.items():
+            if value > 0:
+                keys_list.extend([key] * value)
+                values_list.extend([1] * value)
+            elif value < 0:
+                keys_list.extend([key] * abs(value))
+                values_list.extend([-1] * abs(value))
+        # 2. 再一步步进行解析(第一步)
+        tp_1st = one_step_reaction_based_on_fp(target_mol, keys_list[0],values_list[0], parent_fp)
+        if (len(keys_list)==1)|(tp_1st is None):
+            final_tp = tp_1st
+        else: # 3. 如果反应不止1步，开始做第二步
+            tp_2nd = one_step_reaction_based_on_fp(tp_1st, keys_list[1],values_list[1], parent_fp)
+            if (len(keys_list) ==2)|(tp_2nd is None):
+                final_tp = tp_2nd
+            else: # 4. 如果反应不止2步，开始做第三步
+                tp_3rd = one_step_reaction_based_on_fp(tp_2nd, keys_list[2],values_list[2], parent_fp)
+                if (len(keys_list) == 3)|(tp_3rd is None):
+                    final_tp = tp_3rd
+                else: # 5. 如果反应不止3步，开始做第4步
+                    tp_4th = one_step_reaction_based_on_fp(tp_3rd, keys_list[3],values_list[3], parent_fp)
+                    if (len(keys_list) == 4)|(tp_4th is None):
+                        final_tp = tp_4th
+                    else: # 5. 如果反应不止4步，开始做第5步
+                        tp_5th = one_step_reaction_based_on_fp(tp_4th, keys_list[4],values_list[4], parent_fp)
+                        if (len(keys_list) == 5)|(tp_5th is None):
+                            final_tp = tp_5th
+                        else: # 5. 如果反应不止5步，开始做第6步
+                            tp_6th = one_step_reaction_based_on_fp(tp_5th, keys_list[5],values_list[5], parent_fp)
+                            final_tp = tp_6th
+    else:
+        pass
+    return final_tp
+
+
+
+
+def unfold_formula_result(input_data,parent_mol,fold_change = 5):
+    """
+    Expands possible molecular formulas from input data, calculates changes relative to the parent molecule,
+    and filters the results based on specified criteria.
+
+    This function takes input data containing potential neutral formulas, calculates the changes in molecular
+    composition relative to a parent molecule, and filters the results based on fold change and other criteria.
+    It returns a DataFrame with detailed information about the expanded formulas.
+
+    Parameters:
+    - input_data (pd.DataFrame): The input data containing potential neutral formulas and other relevant information.
+    - parent_mol (Chem.Mol): The RDKit molecule object representing the parent molecule.
+    - fold_change (int): The fold change of compounds to consider. Default is 5.
+
+    Returns:
+    - pd.DataFrame: A DataFrame containing the expanded formulas and calculated changes relative to the parent molecule.
+
+    Example:
+    >>> input_data = pd.DataFrame({'neutral_formula': ['C6H12O6', 'C7H14O7'], 'error': ['0.01', '0.02'], 'iso_score': ['0.8', '0.9']})
+    >>> parent_mol = Chem.MolFromSmiles('CCO')
+    >>> unfold_formula_result(input_data, parent_mol)
+    """
+    
+    # 1. 将可能的分子式展开
+    parent_formula = CalcMolFormula(parent_mol)
+    row_nan = input_data[(input_data['neutral_formula'].isna()|(input_data['neutral_formula'] == '[]'))]
+    row_formula = input_data[~(input_data['neutral_formula'].isna()|(input_data['neutral_formula'] == '[]'))].reset_index(drop = True)
+    data_all = []
+    for i in tqdm(range(len(row_formula)),desc = 'Extracting all formula',leave = False):
+        a = eval(row_formula.loc[i,'neutral_formula'])
+        b = eval(row_formula.loc[i,'error'])
+        c = eval(row_formula.loc[i,'iso_score'])
+        num = len(a)
+        single_row_df = row_formula.loc[[i]]
+        single_row_df_replicates = pd.concat([single_row_df] * num, ignore_index=True)
+        single_row_df_replicates['neutral_formula'] = a
+        single_row_df_replicates['error'] = b
+        single_row_df_replicates['iso_score'] = c
+        data_all.append(single_row_df_replicates)
+    formula_df = pd.concat(data_all,axis=0)
+
+    # 2. 筛选fold change
+    fold_change_name = [i for i in formula_df.columns if 'fold_change' in i]
+    result1 = formula_df[(formula_df[fold_change_name]>fold_change).all(axis=1)].reset_index(drop = True)
+
+    # 3. 计算改变信息
+    for i in range(len(result1)):
+        formula = result1.loc[i, 'neutral_formula']
+        reduced_part, added_part = calculate_formula_differences(parent_formula, formula)
+        result1.loc[i, 'added part'] = added_part
+        result1.loc[i, 'reduced part'] = reduced_part
+        result1.loc[i, 'Changed Num'] = int(calculate_changed_num(added_part, reduced_part))
+        result1.loc[i, 'element Num'] = len(parse_formula(added_part)) + len(parse_formula(reduced_part))
+    result1['Changed Num'] = result1['Changed Num'].astype(int)
+    result1['element Num'] = result1['element Num'].astype(int)
+    result2 = result1.sort_values(by=['Changed Num', 'element Num'])
+    result3 = pd.concat([result2,row_nan]).reset_index(drop = True)
+
+    return result3
+
+
+
+def generate_possible_TP_structures(parent_mol, TP_formula_neutral):
+    """
+    Generates possible transformation product (TP) structures by modifying a parent molecule
+    based on a target transformation product formula.
+
+    This function identifies potential sites for modification in the parent molecule, applies
+    chemical transformations based on the specified target TP formula, and considers the reaction
+    mode to adjust the molecular structure accordingly. The goal is to explore plausible structural
+    changes that align with the target TP formula, generating a set of potential TP structures.
+
+    Parameters:
+    - parent_mol (Chem.Mol): The RDKit molecule object representing the parent molecule.
+    - TP_formula_neutral (str): The chemical formula of the target transformation product. Note: TP_formula_neutral must be neutral.
+
+    Returns: (intermediate,element_change, rxn_steps,final_tp)
+    - intermediate (str or None): The SMILES string of the intermediate structure before the final TP, or None if not applicable.
+    - element_change (str or None): A string representation of the element changes from the intermediate to the final TP, or None if not applicable.
+    - rxn_steps (str or None): A string representation of the reaction steps needed to transform the intermediate to the final TP, or None if not applicable.
+    - final_tp (str or None): The SMILES string of the final transformation product, or None if no valid TP is generated.
+
+    Steps:
+    1. Identify atoms in the parent molecule that have hydrogen atoms available for substitution.
+    2. Adjust the target TP formula based on the reaction mode to account for ionization effects.
+    3. Compare the parent molecule's formula with the target TP formula to identify differences.
+    4. Fragment the parent molecule and evaluate each fragment for potential modifications.
+    5. Generate a series of reaction types based on the identified differences and apply these to the parent molecule or its fragments to generate potential TP structures.
+
+    Note:
+    - The function assumes that the parent molecule and the target TP formula represent chemically valid structures.
+    - The generated TP structures are theoretical and may require further validation to ensure their chemical plausibility.
+    """
+
+    formula = CalcMolFormula(parent_mol)
+
+    possible_TPs = {}
+    # Step 0. 看看哪些原子上有H，这样可以取代
+    atoms_with_H = []
+    for atom in parent_mol.GetAtoms():
+        if has_hydrogen_count(atom):
+            atoms_with_H.append(atom.GetIdx())
+
+    # step 1. 根据正负离子模式转化成中性分子(删除了)
+
+    # step 2. 对比一下和母体结构差异
+    structures_dict = {}  # 创建一个新的字典
+    reduced_part, added_part = calculate_formula_differences(formula, TP_formula_neutral)
+    num = calculate_changed_num(reduced_part, added_part)
+    structures_dict[parent_mol] = num
+
+    # Step 3. 打碎分子并存储
+    frags = generate_fragments(parent_mol)
+    frags = [replace_dummies_with_hydrogens(frag) for frag in frags]
+    frag_smis = list(set([Chem.MolToSmiles(frag) for frag in frags]))
+    frags1 = [Chem.MolFromSmiles(frag_smi) for frag_smi in frag_smis]
+
+    # Step 3.1 补充那些两两组合的
+    frags = generate_fragments(parent_mol)
+    pairs = list(itertools.combinations(list(np.arange(len(frags))), 2))
+    for pair in tqdm(pairs, desc='Combine different frags',leave = False):
+        mol1 = frags[pair[0]]
+        mol2 = frags[pair[1]]
+        new_mol = combine_two_frags(mol1, mol2)
+        frags1.append(new_mol)
+
+    # Step 4. 计算分子式总的改变个数,确定在哪个碎片上进行加工 (要重新写，考虑同样分子式的情况)
+
+    for frag in tqdm(frags1, desc='Finding the most relavent structure',leave = False):
+        frag_formula = CalcMolFormula(frag)
+        reduced_part, added_part = calculate_formula_differences(frag_formula, TP_formula_neutral)
+        frag_total_num = calculate_changed_num(reduced_part, added_part)
+        structures_dict[frag] = frag_total_num
+
+    # Step 5. 将要修改的parent/frag与TP的分子式对比，生成series
+    sub_rxn = ['NH', 'O', 'CH2', 'H-1NO2', 'H2', 'H-1Cl', 'H-1Br', 'H-1F', 'H-1I']
+    s = pd.Series(structures_dict).sort_values()
+    s1 = s[s == s.min()]
+    target_mols = list(s1.index)
+    # 去除重复的
+    target_mols_smi = list(set([Chem.MolToSmiles(i) for i in target_mols]))
+    target_mols = [Chem.MolFromSmiles(i) for i in target_mols_smi]
+
+    # 先对intermediate,rxn_s1_dict,final_tp进行定义
+    intermediate = None
+    element_change = None
+    rxn_steps = None
+    final_tp = None 
+    
+
+    if len(target_mols) !=0:
+        # Step 6. 对target_mols进行筛选，找到最相似的
+        if len(target_mols)>1:
+            parent_fp = AllChem.GetMorganFingerprintAsBitVect(parent_mol, 2, nBits=1024)
+            tp_list_similarity = []
+            for i in range(len(target_mols)):
+                tp_fp = AllChem.GetMorganFingerprintAsBitVect(target_mols[i], 2, nBits=1024)
+                similarity = FingerprintSimilarity(parent_fp, tp_fp)
+                tp_list_similarity.append(similarity)
+            combined = list(zip(target_mols,tp_list_similarity))
+            sorted_combined = sorted(combined, key=lambda x: x[1],reverse = True)
+            target_mols,tp_list_similarity = zip(*sorted_combined)
+        target_mol = target_mols[0]
+
+        # step 7. 开始对target_mol 进行处理，找到基于target_mol到products改变了什么
+        frag_formula = CalcMolFormula(target_mol)
+        reduced_part, added_part = calculate_formula_differences(frag_formula, TP_formula_neutral)
+        s1 = pd.Series(parse_formula(reduced_part), dtype=object) * -1
+        s2 = pd.Series(parse_formula(added_part), dtype=object)
+        change_s = pd.concat([s1, s2])
+
+        # step 8. 开始分析final_tp
+        if len(change_s) == 0:  # 说明和碎片相同
+            # final_tp就是碎片，因此intermediate和element change仍然是None
+            final_tp = target_mol
+           
+        else:
+            intermediate = target_mol # 先给intermediate赋值
+            element_change = str(change_s.to_dict())
+            # 开始处理每个元素
+            atoms = ['C', 'H', 'O', 'N', 'Cl', 'Br', 'F', 'I']
+            atoms_not_present = [i for i in atoms if i not in change_s.index]
+            unpresent_s = pd.Series(np.zeros(len(atoms_not_present)).astype(int), atoms_not_present)
+            change_s1 = pd.concat([change_s, unpresent_s])
+            # 确定范围
+            ranges = [range(min([0, change_s1['N']]), max([0, change_s1['N']]) + 1),
+                      range(min([0, change_s1['O']]), max([0, change_s1['O']]) + 1),
+                      range(min([0, change_s1['C']]), max([0, change_s1['C']]) + 1),
+                      range(min([0, change_s1['N']]), max([0, change_s1['N']]) + 1),
+                      range(-5, 5),
+                      range(min([0, change_s1['Cl']]), max([0, change_s1['Cl']]) + 1),
+                      range(min([0, change_s1['Br']]), max([0, change_s1['Br']]) + 1),
+                      range(min([0, change_s1['F']]), max([0, change_s1['F']]) + 1),
+                      range(min([0, change_s1['I']]), max([0, change_s1['I']]) + 1)]
+            patterns_list = list(itertools.product(*ranges))
+            # 开始做匹配
+            rxn_s = None
+            for pattern in patterns_list:
+                a, b, c, d, e, f, g, h, i = pattern  # a*NH, b*O, c*CH2, d*H-1NO2, e*H2, f*H-1Cl, g*H-1Br, h*H-1F, i*H-1I
+                N_num = a + d  # a
+                O_num = b + 2 * d  # b
+                C_num = c  # c
+                Cl_num = f
+                Br_num = g
+                F_num = h
+                I_num = i
+                H_num = a + 2 * c - d + 2 * e - f - g - h - i
+                if (N_num == change_s1['N']) & (O_num == change_s1['O']) & (C_num == change_s1['C']) & (
+                        Cl_num == change_s1['Cl']) & (Br_num == change_s1['Br']) & (F_num == change_s1['F']) & (
+                        I_num == change_s1['I']) & (H_num == change_s1['H']):
+                    rxn_s = pd.Series([a, b, c, d, e, f, g, h, i], sub_rxn)
+                    # 开始处理该分子
+                    rxn_s1 = rxn_s[rxn_s != 0]  # 去掉那些没有用的
+                    rxn_s1 = pd.concat([rxn_s1[['H2']], rxn_s1.drop('H2')]) if 'H2' in rxn_s1.index else rxn_s1
+                    rxn_s1_dict = rxn_s1.to_dict() 
+                    rxn_steps = str(rxn_s1_dict) # 再给rxn_s1_dict赋值
+                    final_tp = stepwise_reaction_single_tp(target_mol, rxn_s1,parent_mol)
+
+        if final_tp is not None: # 检查final_tp是否正确,并且转化成smile
+            if parse_formula(CalcMolFormula(final_tp)) == parse_formula(TP_formula_neutral):
+                final_tp = Chem.MolToSmiles(final_tp)
+            else:
+                final_tp = None
+
+        if intermediate is not None:
+            intermediate = Chem.MolToSmiles(intermediate)
+
+    else:
+        print("No target mols were generated")
+    return intermediate,element_change, rxn_steps,final_tp
+
 
 
 def add_missing_H(mol):
     """
     Adds missing hydrogen atoms to the first encountered under-saturated carbon (C), nitrogen (N),
     or oxygen (O) atom in a given molecule. This function is designed to ensure that these atoms reach
     their typical valency: C (up to 4), N (up to 3), and O (up to 2).
@@ -44,21 +553,22 @@
             break
         if (atom.GetSymbol() == 'N' and atom.GetExplicitValence() < 3):
             mol = Chem.EditableMol(mol)
             h_idx = mol.AddAtom(Chem.Atom(1))
             mol.AddBond(atom.GetIdx(), h_idx, Chem.BondType.SINGLE)
             mol = mol.GetMol()
             break
-        if (atom.GetSymbol() == 'O' and atom.GetExplicitValence() < 2):
-            mol = Chem.EditableMol(mol)
+        if ((atom.GetSymbol() == 'O') and (atom.GetExplicitValence() < 2)  and ('N' not in [i.GetSymbol() for i in atom.GetNeighbors()])):
+            mol = Chem.EditableMol(mol) # 考虑NO2情况，不能给O上加H
             h_idx = mol.AddAtom(Chem.Atom(1))
             mol.AddBond(atom.GetIdx(), h_idx, Chem.BondType.SINGLE)
             mol = mol.GetMol()
             break
-
+    smi = Chem.MolToSmiles(mol)
+    mol = Chem.MolFromSmiles(smi)
     mol = Chem.RemoveHs(mol)
     return mol
 
 
 def check_bad_valance_Hidx(test1):
     """
     Adds missing hydrogen atoms to under-saturated carbon (C), nitrogen (N), or oxygen (O) atoms in a molecule.
@@ -187,249 +697,172 @@
                 if len(keys_list) == 3:
                     final_tps.extend(tps3)
                 else:
                     print('Please simplify the reaction or break it down into multiple steps.')
     return final_tps
 
 
-def generate_possible_TP_structures(parent_mol, TP_formula, mode='pos'):
-    """
-    Generates possible transformation product (TP) structures by modifying a parent molecule
-    based on a target transformation product formula and reaction mode.
 
-    This function identifies potential sites for modification in the parent molecule, applies
-    chemical transformations based on the specified target TP formula, and considers the reaction
-    mode (positive or negative ion mode) to adjust the molecular structure accordingly. The goal
-    is to explore plausible structural changes that align with the target TP formula, generating
-    a set of potential TP structures.
 
-    Parameters:
-    - parent_mol (Chem.Mol): The RDKit molecule object representing the parent molecule.
-    - TP_formula (str): The chemical formula of the target transformation product.
-    - mode (str, optional): The ionization mode, either 'pos' for positive or 'neg' for negative.
-      Default is 'pos'. This affects how the molecular structure is adjusted to match the target
-      TP formula.
-
-    Returns:
-    - list of Chem.Mol: A list of RDKit molecule objects representing potential TP structures
-      that match the target TP formula.
-
-    Steps:
-    1. Identify atoms in the parent molecule that have hydrogen atoms available for substitution.
-    2. Adjust the target TP formula based on the reaction mode to account for ionization effects.
-    3. Compare the parent molecule's formula with the target TP formula to identify differences.
-    4. Fragment the parent molecule and evaluate each fragment for potential modifications.
-    5. Generate a series of reaction types based on the identified differences and apply these
-       to the parent molecule or its fragments to generate potential TP structures.
-
-    Note:
-    - The function assumes that the parent molecule and the target TP formula represent chemically
-      valid structures.
-    - The generated TP structures are theoretical and may require further validation to ensure
-      their chemical plausibility.
-    """
-
-    formula = CalcMolFormula(parent_mol)
-
-    possible_TPs = {}
-    # Step 0. 看看哪些原子上有H，这样可以取代
-    atoms_with_H = []
-    for atom in parent_mol.GetAtoms():
-        if has_hydrogen_count(atom):
-            atoms_with_H.append(atom.GetIdx())
-
-    # step 1. 根据正负离子模式转化成中性分子
-    if mode == 'pos':
-        TP_formula = modify_chemical_formula(TP_formula, '-H')
-    if mode == 'neg':
-        TP_formula = modify_chemical_formula(TP_formula, '+H')
-
-    # step 2. 对比一下和母体结构差异
-    structures_dict = {}  # 创建一个新的字典
-    reduced_part, added_part = calculate_formula_differences(formula, TP_formula)
-    num = calculate_changed_num(reduced_part, added_part)
-    structures_dict[parent_mol] = num
-
-    # Step 3. 打碎分子并存储
-    frags = generate_fragments(parent_mol)
-    frags = [replace_dummies_with_hydrogens(frag) for frag in frags]
-    frag_smis = list(set([Chem.MolToSmiles(frag) for frag in frags]))
-    frags1 = [Chem.MolFromSmiles(frag_smi) for frag_smi in frag_smis]
-
-    # Step 3.1 补充那些两两组合的
-    frags = generate_fragments(parent_mol)
-    pairs = list(itertools.combinations(list(np.arange(len(frags))), 2))
-    for pair in tqdm(pairs, desc='Combine different frags'):
-        mol1 = frags[pair[0]]
-        mol2 = frags[pair[1]]
-        new_mol = combine_two_frags(mol1, mol2)
-        frags1.append(new_mol)
-
-    # Step 4. 计算分子式总的改变个数,确定在哪个碎片上进行加工 (要重新写，考虑同样分子式的情况)
-
-    for frag in tqdm(frags1, desc='Finding the most relavent structure'):
-        frag_formula = CalcMolFormula(frag)
-        reduced_part, added_part = calculate_formula_differences(frag_formula, TP_formula)
-        frag_total_num = calculate_changed_num(reduced_part, added_part)
-        structures_dict[frag] = frag_total_num
-
-    # Step 5. 将要修改的parent/frag与TP的分子式对比，生成series
-    sub_rxn = ['NH', 'O', 'CH2', 'H-1NO2', 'H2', 'H-1Cl', 'H-1Br', 'H-1F', 'H-1I']
-    s = pd.Series(structures_dict).sort_values()
-    s1 = s[s == s.min()]
-    target_mols = list(s1.index)
-    # 去除重复的
-    target_mols_smi = list(set([Chem.MolToSmiles(i) for i in target_mols]))
-    target_mols = [Chem.MolFromSmiles(i) for i in target_mols_smi]
-    for target_mol in target_mols:
-        print(f'First Step TP: {Chem.MolToSmiles(target_mol)}')
-        print(f'----------------------------------------------')
-        frag_formula = CalcMolFormula(target_mol)
-        reduced_part, added_part = calculate_formula_differences(frag_formula, TP_formula)
-        print(f'reduced_part:{reduced_part}, added_part:{added_part}')
-        s1 = pd.Series(parse_formula(reduced_part), dtype=object) * -1
-        s2 = pd.Series(parse_formula(added_part), dtype=object)
-        change_s = pd.concat([s1, s2])
-        if len(change_s) == 0:  # 说明和碎片相同
-            possible_TPs[target_mol] = 'Frag'
-        else:
-            # 开始处理每个元素
-            atoms = ['C', 'H', 'O', 'N', 'Cl', 'Br', 'F', 'I']
-            atoms_not_present = [i for i in atoms if i not in change_s.index]
-            unpresent_s = pd.Series(np.zeros(len(atoms_not_present)).astype(int), atoms_not_present)
-            change_s1 = pd.concat([change_s, unpresent_s])
-            # 确定范围
-            ranges = [range(min([0, change_s1['N']]), max([0, change_s1['N']]) + 1),
-                      range(min([0, change_s1['O']]), max([0, change_s1['O']]) + 1),
-                      range(min([0, change_s1['C']]), max([0, change_s1['C']]) + 1),
-                      range(min([0, change_s1['N']]), max([0, change_s1['N']]) + 1),
-                      range(-5, 5),
-                      range(min([0, change_s1['Cl']]), max([0, change_s1['Cl']]) + 1),
-                      range(min([0, change_s1['Br']]), max([0, change_s1['Br']]) + 1),
-                      range(min([0, change_s1['F']]), max([0, change_s1['F']]) + 1),
-                      range(min([0, change_s1['I']]), max([0, change_s1['I']]) + 1)]
-            patterns_list = list(itertools.product(*ranges))
-            # 开始做匹配
-            rxn_s = None
-            for pattern in patterns_list:
-                a, b, c, d, e, f, g, h, i = pattern  # a*NH, b*O, c*CH2, d*H-1NO2, e*H2, f*H-1Cl, g*H-1Br, h*H-1F, i*H-1I
-                N_num = a + d  # a
-                O_num = b + 2 * d  # b
-                C_num = c  # c
-                Cl_num = f
-                Br_num = g
-                F_num = h
-                I_num = i
-                H_num = a + 2 * c - d + 2 * e - f - g - h - i
-                if (N_num == change_s1['N']) & (O_num == change_s1['O']) & (C_num == change_s1['C']) & (
-                        Cl_num == change_s1['Cl']) & (Br_num == change_s1['Br']) & (F_num == change_s1['F']) & (
-                        I_num == change_s1['I']) & (H_num == change_s1['H']):
-                    rxn_s = pd.Series([a, b, c, d, e, f, g, h, i], sub_rxn)
-                    # 开始处理该分子
-                    rxn_s1 = rxn_s[rxn_s != 0]  # 去掉那些没有用的
-                    rxn_s1 = pd.concat([rxn_s1[['H2']], rxn_s1.drop('H2')]) if 'H2' in rxn_s1.index else rxn_s1
-                    rxn_s1_dict = rxn_s1.to_dict()
-                    print(rxn_s1_dict)
-                    # 先关注第一步的结构
-                    print(Chem.MolToSmiles(target_mol))
-                    possible_tp_list = stepwise_reaction(target_mol, rxn_s1)
-
-                    for rxn_tp in possible_tp_list:
-                        possible_TPs[rxn_tp] = str(rxn_s1_dict)
-
-        print(f'===============================================')
-    tp_list = [k for k, v in possible_TPs.items()]
-    tp_list = [i for i in tp_list if CalcMolFormula(i) == TP_formula]  # 去掉不符合formula的
-    tp_smiles = list(set([Chem.MolToSmiles(i) for i in tp_list]))  # 去重
-    tp_list = [Chem.MolFromSmiles(i) for i in tp_smiles]
-    return tp_list
-
-
-def from_mass_to_formula(parent_mol, observed_mz, mode, iso_info, ms_error=10, iso_score=0.7, addition_element={}):
+def from_mass_to_formula(parent_mol, input_data, mode,  mz_error=10,
+                         iso_info = None,iso_checking= False, iso_score_threshold=0.7,
+                         max_possible_num=2e7, addition_element={}):
     """
     Convert an observed mass to a chemical formula based on a parent molecule and additional criteria.
 
     Args:
         parent_mol (Mol): The parent molecule (RDKit Mol object) from which to derive the formula.
-        observed_mz (float): The observed mass/charge (m/z) ratio.
+        input_data (float or pd.DataFrame): Either a single m/z value (float) or a DataFrame containing m/z values.
         mode (str): The ionization mode, either 'pos' for positive or 'neg' for negative.
-        iso_info (dict): Isotope information used for scoring isotope patterns.
-        ms_error (float, optional): The mass spectrometry error tolerance (default is 10 ppm).
-        iso_score (float, optional): The minimum isotope score to consider a formula reasonable (default is 0.7).
+        mz_error (float, optional): The mass spectrometry error tolerance in parts per million (ppm). Defaults to 10 ppm.
+        iso_info (dict, optional): Isotope information used for scoring isotope patterns. Only applicable for a single m/z value.
+        iso_checking (bool, optional): Whether to check isotope information for all m/z values in the DataFrame. Defaults to False.
+        iso_score_threshold (float, optional): The minimum isotope score to consider a formula reasonable. Only applicable for DataFrame input. Defaults to 0.7.
         addition_element (dict, optional): Additional elements to consider in the formula calculation. Keys are element symbols
-            and values are the maximum number of atoms allowed for each element (default is an empty dict).
+                                           and values are the maximum number of atoms allowed for each element. Defaults to an empty dict.
 
     Returns:
-        DataFrame: A pandas DataFrame containing the possible formulas, sorted by the number of changes and
-        the number of elements involved in the change. Additional columns include:
+        DataFrame: A pandas DataFrame containing the possible formulas, sorted by the number of changes and the number of elements involved in the change.
+        Additional columns include:
         - 'formula': Possible molecular formula.
         - 'reasonable': Boolean indicating if the formula is reasonable based on isotope pattern scoring.
         - 'formula_neutral': The neutral molecular formula after adjusting for ionization mode.
         - 'added part': Elements added to the parent molecule to get the possible formula.
         - 'reduced part': Elements removed from the parent molecule to get the possible formula.
         - 'Changed Num': The number of atoms changed (added or removed) to get the possible formula.
         - 'element Num': The number of distinct elements involved in the change.
         - 'iso_score': The isotope pattern score for the formula.
 
     This function calculates possible chemical formulas based on an observed m/z value and a parent molecule. It takes
     into account the ionization mode, additional elements to consider, and isotope information for scoring. The function
     adjusts formulas for ionization, evaluates their reasonableness based on isotope patterns, and identifies changes
     relative to the parent molecule.
+
+    Raises:
+        ValueError: If the input_data is neither a float nor a pd.DataFrame.
     """
-    # 获得基础信息
-    parent_formula = CalcMolFormula(parent_mol)
-    formula_dict = parse_formula(parent_formula)
-    atoms = [k for k, v in formula_dict.items()] + [k for k, v in addition_element.items()]
-    mz_difference = ExactMolWt(parent_mol) - observed_mz  # 看看差别了多少
 
-    # 获得检索的元素和数量范围
-    max_C = int(observed_mz / 14)  # 考虑CnH2n+2
-    min_C = int(observed_mz / 100)  # 考虑C-I
-    atom_n = []
-    for k, v in formula_dict.items():
-        if k == 'C':
-            atom_n.append([min_C, max_C])
-        elif k == 'H':
-            atom_n.append([max(min_C * 2 + 2, v - 20), v + 20])
-        elif k == 'N':
-            atom_n.append([max(0, v - 10), v + 5])
-        elif k == 'O':
-            atom_n.append([max(0, v - 10), v + 10])
-        elif k == 'P':
-            atom_n.append([max(0, v - 5), v + 2])
-        elif k == 'S':
-            atom_n.append([max(0, v - 5), v + 2])
+    
+    if isinstance(input_data, float):
+        parent_formula = CalcMolFormula(parent_mol)
+        max_mz,min_mz = input_data,input_data
+        atoms, atom_n = get_formula_elements_range(parent_mol,max_mz,min_mz,addition_element = addition_element)
+        # 获得所有可能的分子式
+        result = formula_prediction(input_data, mode, atoms, atom_n,mz_error = mz_error,max_possible_num=max_possible_num)
+        if len(result) == 0:
+            return result
         else:
-            atom_n.append([0, v])
-    atom_n = atom_n + [[0, v] for k, v in addition_element.items()]
-    # 获得所有可能的分子式
-    result = formula_prediction(observed_mz, mode, atoms, atom_n)
-    result['reasonable'] = result['formula'].apply(is_valid_formula)  # 看看哪些分子式合理
-    result1 = result[result['reasonable'] == True].reset_index(drop=True)
-
-    # 对pos和neg下的分子式进行修改
-    result1['formula_neutral'] = result1['formula'].apply(modify_chemical_formula,
-                                                          args=['-H'] if mode == 'pos' else ['+H'])
+            result['reasonable'] = result['formula'].apply(is_valid_formula)  # 看看哪些分子式合理
+            result1 = result[result['reasonable'] == True].reset_index(drop=True)
+
+            # 对pos和neg下的分子式进行修改
+            result1['formula_neutral'] = result1['formula'].apply(modify_chemical_formula,
+                                                                  args=['-H'] if mode == 'pos' else ['+H'])
+
+            # 看看这些合理的分子式相对于母体的变化
+            if len(result1) == 0:
+                return result1
+            else:
+                for i in range(len(result1)):
+                    formula = result1.loc[i, 'formula_neutral']
+                    reduced_part, added_part = calculate_formula_differences(parent_formula, formula)
+                    result1.loc[i, 'added part'] = added_part
+                    result1.loc[i, 'reduced part'] = reduced_part
+                    result1.loc[i, 'Changed Num'] = int(calculate_changed_num(added_part, reduced_part))
+                    result1.loc[i, 'element Num'] = len(parse_formula(added_part)) + len(parse_formula(reduced_part))
+                    if isinstance(iso_info, dict):
+                        iso_score = isotope_score(iso_info, formula, mode=mode)
+                        result1.loc[i, 'iso_score'] = iso_score
+
+                result1['Changed Num'] = result1['Changed Num'].astype(int)
+                result1['element Num'] = result1['element Num'].astype(int)
+                result2 = result1.sort_values(by=['Changed Num', 'element Num']).reset_index(drop=True)
+                return result2
+    elif isinstance(input_data, pd.DataFrame):
+        
+        # 3. 开始获得mz
+        observed_mz = input_data['mz'].values
+        max_mz,min_mz = max(observed_mz), min(observed_mz)
+        # 4. 获得范围
+        atoms,atom_n = get_formula_elements_range(parent_mol,max_mz,min_mz,addition_element=addition_element)
+        # 5. 获得分子式匹配结果和偏差
+        formula_result = formula_prediction(observed_mz, mode, atoms=atoms,
+                               atom_n=atom_n, max_possible_num=max_possible_num, mz_error=mz_error,all_info = True)
+
+        if iso_checking is False:
+            # 6. 挨个检查这些分子式是否合理,并重新生成
+            formula = []
+            error = []
+            iso_score = [] 
+            for i in tqdm(range(len(formula_result[0])),desc = 'Removing unreasonable formula',leave = False):
+                if formula_result[0][i] is None:
+                    formula.append(np.nan)
+                    error.append(np.nan)
+                    iso_score.append(np.nan)
+                else:
+                    old_formula = eval(formula_result[0][i])
+                    old_error = eval(formula_result[1][i])
+
+                    if mode == 'pos':
+                        new_formula = [modify_chemical_formula(f,'-H') for i,f in enumerate(old_formula) if is_valid_formula(f)]
+                    else:
+                        new_formula = [modify_chemical_formula(f,'+H') for i,f in enumerate(old_formula) if is_valid_formula(f)]
+
+                    new_error = [f for i,f in enumerate(old_error) if is_valid_formula(old_formula[i])]
+
+                    formula.append(str(new_formula))
+                    error.append(str(new_error))
+                    iso_score.append(np.nan)
+        else:
+            # 7.如果需要检查iso_info
+            formula = []
+            error = []
+            iso_score = []
+            for i in tqdm(range(len(formula_result[0])),desc = 'Checking formula',leave = False):
+                if formula_result[0][i] is None:
+                    formula.append(np.nan)
+                    error.append(np.nan)
+                    iso_score.append(np.nan)
+                else:
+                    old_formula = eval(formula_result[0][i])
+                    old_error = eval(formula_result[1][i])
+
+                    if mode == 'pos':
+                        new_formula = [modify_chemical_formula(f,'-H') for i,f in enumerate(old_formula) if is_valid_formula(f)]
+                    else:
+                        new_formula = [modify_chemical_formula(f,'+H') for i,f in enumerate(old_formula) if is_valid_formula(f)]
+                    new_error = [f for i,f in enumerate(old_error) if is_valid_formula(old_formula[i])]
+
+                    iso_info = eval(input_data.loc[i,'iso_distribution']) #获得iso_info
+                    score = []
+                    for f in new_formula:
+
+                        sc = isotope_score(iso_info,f,mode = mode)
+                        score.append(round(sc,2))
+
+                    # 筛选条件
+                    score_array = np.array(score)
+                    index = np.where(score_array>iso_score_threshold)
+                    score = list(score_array[index])
+                    new_formula = list(np.array(new_formula)[index])
+                    new_error = list(np.array(new_error)[index])
+
+                    formula.append(str(new_formula))
+                    error.append(str(new_error))
+                    iso_score.append(str(score))
+        # 8. 把生成的结果添加到列表中
+        unique1 = input_data.copy()
+        unique1['formula'] = formula
+        unique1['error'] = error
+        unique1['iso_score'] = iso_score
+        unique1 = unique1.rename(columns=lambda x: x.replace('formula', 'neutral_formula') if 'formula' in x else x)
+        
+        return unique1
 
-    # 看看这些合理的分子式相对于母体的变化
-    for i in range(len(result1)):
-        formula = result1.loc[i, 'formula_neutral']
-        reduced_part, added_part = calculate_formula_differences(parent_formula, formula)
-        result1.loc[i, 'added part'] = added_part
-        result1.loc[i, 'reduced part'] = reduced_part
-        result1.loc[i, 'Changed Num'] = int(calculate_changed_num(added_part, reduced_part))
-        result1.loc[i, 'element Num'] = len(parse_formula(added_part)) + len(parse_formula(reduced_part))
-        if isinstance(iso_info, dict):
-            iso_score = isotope_score(iso_info, formula, mode=mode)
-            result1.loc[i, 'iso_score'] = iso_score
 
-    result1['Changed Num'] = result1['Changed Num'].astype(int)
-    result1['element Num'] = result1['element Num'].astype(int)
-    result2 = result1.sort_values(by=['Changed Num', 'element Num']).reset_index(drop=True)
-    return result2
 
 
 def is_valid_formula(formula):
     """
     Determines if a given chemical formula is valid based on specific elemental ratios and counts.
 
     This function checks if the provided formula adheres to common organic chemistry rules regarding the relative
@@ -449,15 +882,15 @@
 
     The function parses the formula to count each element's occurrences and applies the validation rules to determine
     if the formula could represent a plausible organic molecule.
     """
 
     element_counts = parse_formula(formula)
     # 计算C数量
-    C_count = element_counts['C']
+    C_count = element_counts['C'] if 'C' in [k for k, v in element_counts.items()] else 0
     # 计算各个元素的数量
     F_count = element_counts['F'] if 'F' in [k for k, v in element_counts.items()] else 0
     Cl_count = element_counts['Cl'] if 'Cl' in [k for k, v in element_counts.items()] else 0
     Br_count = element_counts['Br'] if 'Br' in [k for k, v in element_counts.items()] else 0
     I_count = element_counts['I'] if 'I' in [k for k, v in element_counts.items()] else 0
 
     H_count = element_counts['H'] if 'H' in [k for k, v in element_counts.items()] else 0
@@ -1404,74 +1837,14 @@
                         neighbors = sorted([i.GetSymbol() for i in atom.GetNeighbors()])
                         if neighbors == target_neighbors:
                             index = atom.GetIdx()
 
     return mol_no_h, index
 
 
-def combine_fragments_and_generate_smiles(fragment1_smiles, fragment2_smiles, fragment1_connect_atom_idx,
-                                          fragment2_connect_atom_idx):
-    """
-    Combines two molecular fragments, represented by their SMILES strings, into a single molecule by forming a bond
-    between specified atoms from each fragment.
-
-    This function takes the SMILES strings of two molecular fragments and the indices of the atoms (within each fragment)
-    that should be connected. It then combines these fragments into a single molecule by forming a single bond between
-    the specified atoms. The resulting molecule is returned as a SMILES string.
-
-    Parameters:
-    - fragment1_smiles (str): The SMILES string representing the first molecular fragment.
-    - fragment2_smiles (str): The SMILES string representing the second molecular fragment.
-    - fragment1_connect_atom_idx (int): The zero-based index of the atom in the first fragment to be connected.
-    - fragment2_connect_atom_idx (int): The zero-based index of the atom in the second fragment to be connected.
-
-    Returns:
-    - str: The SMILES string representing the combined molecule after connecting the specified atoms.
-
-    Example:
-    >>> combine_fragments_and_generate_smiles('CCO', 'N', 2, 0)
-    'CCON'
-
-    Note:
-    - The indices of the connecting atoms are based on the order of atoms in their respective SMILES strings.
-    - The function assumes valid SMILES strings and valid atom indices are provided. Invalid inputs may lead to
-      unexpected results or errors.
-    - The bond formed between the fragments is a single bond. Modifications are needed to form other types of bonds.
-    """
-    # Create molecule objects from the SMILES strings
-    fragment1_mol = Chem.MolFromSmiles(fragment1_smiles)
-    fragment2_mol = Chem.MolFromSmiles(fragment2_smiles)
-
-    # Combine the molecules
-    combined_mol = rdmolops.CombineMols(fragment1_mol, fragment2_mol)
-
-    # Create an editable molecule for further modifications
-    editable_mol = Chem.EditableMol(combined_mol)
-
-    # Calculate the index of the first atom in fragment2 within the combined molecule
-    fragment2_start_idx = fragment1_mol.GetNumAtoms()
-
-    # Add a bond between the specified atoms
-    # The index of the connecting atom in fragment2 needs to be adjusted to its new index in the combined molecule
-    editable_mol.AddBond(fragment1_connect_atom_idx, fragment2_start_idx + fragment2_connect_atom_idx,
-                         order=Chem.rdchem.BondType.SINGLE)
-
-    # Convert back to a regular Mol object
-    final_mol = editable_mol.GetMol()
-
-    for atom in final_mol.GetAtoms():
-        atom.SetNumExplicitHs(0)
-    # Sanitize the molecule
-    Chem.SanitizeMol(final_mol)
-
-    # Generate and return the SMILES of the combined molecule
-    final_smiles = Chem.MolToSmiles(final_mol, isomericSmiles=True)
-    return final_smiles
-
-
 def draw_molecule_with_atom_indices(mol):
     """
     Draws an RDKit molecule object with atom indices.
 
     Parameters:
     - mol (Chem.Mol): The RDKit molecule object to be drawn.
```

