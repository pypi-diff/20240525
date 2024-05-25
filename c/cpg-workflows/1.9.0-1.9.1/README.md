# Comparing `tmp/cpg-workflows-1.9.0.tar.gz` & `tmp/cpg-workflows-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpg-workflows-1.9.0.tar", last modified: Wed Dec 21 03:31:36 2022, max compression
+gzip compressed data, was "cpg-workflows-1.9.1.tar", last modified: Wed Dec 21 07:03:23 2022, max compression
```

## Comparing `cpg-workflows-1.9.0.tar` & `cpg-workflows-1.9.1.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 03:31:36.946259 cpg-workflows-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    35087 2022-12-21 03:31:36.946259 cpg-workflows-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    34350 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 03:31:36.938259 cpg-workflows-1.9.0/cpg_workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7246 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/batch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 03:31:36.938259 cpg-workflows-1.9.0/cpg_workflows/dataproc_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/dataproc_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/dataproc_scripts/annotate_cohort.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/dataproc_scripts/annotate_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6974 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/dataproc_scripts/mt_to_es.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/dataproc_scripts/vep_json_to_ht.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/defaults.toml
--rw-r--r--   0 runner    (1001) docker     (123)     6619 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/filetypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     9297 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/inputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 03:31:36.942259 cpg-workflows-1.9.0/cpg_workflows/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21438 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/jobs/align.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/jobs/fastqc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11740 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/jobs/genotype.py
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/jobs/happy.py
--rw-r--r--   0 runner    (1001) docker     (123)    17668 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/jobs/joint_genotyping.py
--rw-r--r--   0 runner    (1001) docker     (123)     6887 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/jobs/multiqc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14994 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/jobs/picard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/jobs/samtools.py
--rw-r--r--   0 runner    (1001) docker     (123)     5876 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/jobs/seqr_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     9211 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/jobs/somalier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/jobs/stripy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6832 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/jobs/vcf.py
--rw-r--r--   0 runner    (1001) docker     (123)     8199 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/jobs/vep.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/jobs/verifybamid.py
--rw-r--r--   0 runner    (1001) docker     (123)    32261 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/jobs/vqsr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 03:31:36.942259 cpg-workflows-1.9.0/cpg_workflows/large_cohort/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/large_cohort/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8904 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/large_cohort/ancestry_pca.py
--rw-r--r--   0 runner    (1001) docker     (123)     9361 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/large_cohort/ancestry_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     4808 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/large_cohort/combiner.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      863 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/large_cohort/dataproc_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/large_cohort/dataproc_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/large_cohort/dense_subset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4962 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/large_cohort/frequencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/large_cohort/load_vqsr.py
--rw-r--r--   0 runner    (1001) docker     (123)     4428 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/large_cohort/relatedness.py
--rw-r--r--   0 runner    (1001) docker     (123)     6177 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/large_cohort/sample_qc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/large_cohort/site_only_vcf.py
--rw-r--r--   0 runner    (1001) docker     (123)    24425 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/metamist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 03:31:36.942259 cpg-workflows-1.9.0/cpg_workflows/python_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/python_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/python_scripts/check_multiqc.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10695 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/python_scripts/check_pedigree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 03:31:36.942259 cpg-workflows-1.9.0/cpg_workflows/query_modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/query_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11432 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/query_modules/seqr_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4366 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/query_modules/vep.py
--rw-r--r--   0 runner    (1001) docker     (123)    11216 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/slack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 03:31:36.946259 cpg-workflows-1.9.0/cpg_workflows/stages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/stages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/stages/align.py
--rw-r--r--   0 runner    (1001) docker     (123)    11649 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/stages/cram_qc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5355 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/stages/fastqc.py
--rw-r--r--   0 runner    (1001) docker     (123)    27725 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/stages/gatk_sv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/stages/genotype.py
--rw-r--r--   0 runner    (1001) docker     (123)     6416 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/stages/gvcf_qc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/stages/joint_genotyping.py
--rw-r--r--   0 runner    (1001) docker     (123)     5910 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/stages/joint_genotyping_qc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12231 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/stages/large_cohort.py
--rw-r--r--   0 runner    (1001) docker     (123)     6904 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/stages/seqr_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/stages/stripy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/stages/vep.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/stages/vqsr.py
--rw-r--r--   0 runner    (1001) docker     (123)     5457 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/status.py
--rw-r--r--   0 runner    (1001) docker     (123)    19483 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/targets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    44304 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/cpg_workflows/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 03:31:36.938259 cpg-workflows-1.9.0/cpg_workflows.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    35087 2022-12-21 03:31:36.000000 cpg-workflows-1.9.0/cpg_workflows.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2981 2022-12-21 03:31:36.000000 cpg-workflows-1.9.0/cpg_workflows.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-21 03:31:36.000000 cpg-workflows-1.9.0/cpg_workflows.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      177 2022-12-21 03:31:36.000000 cpg-workflows-1.9.0/cpg_workflows.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2022-12-21 03:31:36.000000 cpg-workflows-1.9.0/cpg_workflows.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      306 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-21 03:31:36.946259 cpg-workflows-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 03:31:36.946259 cpg-workflows-1.9.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 03:31:36.946259 cpg-workflows-1.9.0/test/stages/
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/test/stages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/test/stages/test_first_last_stages.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/test/stages/test_first_last_stages_misconfigured.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/test/stages/test_first_stages.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/test/stages/test_force_stages.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/test/stages/test_last_stages.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/test/stages/test_skip_stages.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/test/stages/test_skip_stages_fail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/test/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/test/test_check_multiqc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/test/test_check_pedigree.py
--rw-r--r--   0 runner    (1001) docker     (123)     7971 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/test/test_cohort.py
--rw-r--r--   0 runner    (1001) docker     (123)     6085 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/test/test_large_cohort.py
--rw-r--r--   0 runner    (1001) docker     (123)     6418 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/test/test_seqr_loader_dry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5470 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/test/test_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2022-12-21 03:31:33.000000 cpg-workflows-1.9.0/test/test_workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 07:03:23.542929 cpg-workflows-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    35087 2022-12-21 07:03:23.542929 cpg-workflows-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    34350 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 07:03:23.534929 cpg-workflows-1.9.1/cpg_workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7246 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/batch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 07:03:23.534929 cpg-workflows-1.9.1/cpg_workflows/dataproc_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/dataproc_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/dataproc_scripts/annotate_cohort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/dataproc_scripts/annotate_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6974 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/dataproc_scripts/mt_to_es.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/dataproc_scripts/vep_json_to_ht.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/defaults.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     6619 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/filetypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9297 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/inputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 07:03:23.538929 cpg-workflows-1.9.1/cpg_workflows/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21438 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/jobs/align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/jobs/fastqc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11740 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/jobs/genotype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/jobs/happy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17668 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/jobs/joint_genotyping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6887 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/jobs/multiqc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14994 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/jobs/picard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/jobs/samtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5876 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/jobs/seqr_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9211 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/jobs/somalier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/jobs/stripy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6832 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/jobs/vcf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8199 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/jobs/vep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/jobs/verifybamid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32261 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/jobs/vqsr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 07:03:23.538929 cpg-workflows-1.9.1/cpg_workflows/large_cohort/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/large_cohort/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8904 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/large_cohort/ancestry_pca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9361 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/large_cohort/ancestry_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4808 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/large_cohort/combiner.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      863 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/large_cohort/dataproc_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/large_cohort/dataproc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/large_cohort/dense_subset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/large_cohort/frequencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/large_cohort/load_vqsr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4428 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/large_cohort/relatedness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6177 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/large_cohort/sample_qc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/large_cohort/site_only_vcf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24425 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/metamist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 07:03:23.538929 cpg-workflows-1.9.1/cpg_workflows/python_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/python_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/python_scripts/check_multiqc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10695 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/python_scripts/check_pedigree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 07:03:23.538929 cpg-workflows-1.9.1/cpg_workflows/query_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/query_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11432 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/query_modules/seqr_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4366 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/query_modules/vep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11216 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/slack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 07:03:23.542929 cpg-workflows-1.9.1/cpg_workflows/stages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/stages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/stages/align.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11649 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/stages/cram_qc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5355 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/stages/fastqc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27725 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/stages/gatk_sv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/stages/genotype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6416 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/stages/gvcf_qc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/stages/joint_genotyping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5910 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/stages/joint_genotyping_qc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12231 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/stages/large_cohort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6904 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/stages/seqr_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/stages/stripy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/stages/vep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/stages/vqsr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5457 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19483 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44304 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/cpg_workflows/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 07:03:23.534929 cpg-workflows-1.9.1/cpg_workflows.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    35087 2022-12-21 07:03:23.000000 cpg-workflows-1.9.1/cpg_workflows.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2022-12-21 07:03:23.000000 cpg-workflows-1.9.1/cpg_workflows.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-21 07:03:23.000000 cpg-workflows-1.9.1/cpg_workflows.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2022-12-21 07:03:23.000000 cpg-workflows-1.9.1/cpg_workflows.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2022-12-21 07:03:23.000000 cpg-workflows-1.9.1/cpg_workflows.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-21 07:03:23.542929 cpg-workflows-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 07:03:23.542929 cpg-workflows-1.9.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 07:03:23.542929 cpg-workflows-1.9.1/test/stages/
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/test/stages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/test/stages/test_first_last_stages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/test/stages/test_first_last_stages_misconfigured.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/test/stages/test_first_stages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/test/stages/test_force_stages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/test/stages/test_last_stages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/test/stages/test_skip_stages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/test/stages/test_skip_stages_fail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/test/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/test/test_check_multiqc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/test/test_check_pedigree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7971 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/test/test_cohort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6085 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/test/test_large_cohort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6418 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/test/test_seqr_loader_dry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5470 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/test/test_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2022-12-21 07:03:21.000000 cpg-workflows-1.9.1/test/test_workflow.py
```

### Comparing `cpg-workflows-1.9.0/LICENSE` & `cpg-workflows-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/PKG-INFO` & `cpg-workflows-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpg-workflows
-Version: 1.9.0
+Version: 1.9.1
 Summary: CPG workflows for Hail Batch
 Home-page: https://github.com/populationgenomics/production-pipelines
 License: MIT
 Keywords: bioinformatics
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cpg-workflows-1.9.0/README.md` & `cpg-workflows-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/cpg_workflows/batch.py` & `cpg-workflows-1.9.1/cpg_workflows/batch.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/cpg_workflows/dataproc_scripts/annotate_cohort.py` & `cpg-workflows-1.9.1/cpg_workflows/dataproc_scripts/annotate_cohort.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/cpg_workflows/dataproc_scripts/annotate_dataset.py` & `cpg-workflows-1.9.1/cpg_workflows/dataproc_scripts/annotate_dataset.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/cpg_workflows/dataproc_scripts/mt_to_es.py` & `cpg-workflows-1.9.1/cpg_workflows/dataproc_scripts/mt_to_es.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/cpg_workflows/dataproc_scripts/vep_json_to_ht.py` & `cpg-workflows-1.9.1/cpg_workflows/dataproc_scripts/vep_json_to_ht.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/cpg_workflows/defaults.toml` & `cpg-workflows-1.9.1/cpg_workflows/defaults.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [images]
-cpg_workflows = 'australia-southeast1-docker.pkg.dev/cpg-common/images/cpg_workflows:1.9.0'
+cpg_workflows = 'australia-southeast1-docker.pkg.dev/cpg-common/images/cpg_workflows:1.9.1'
 
 [workflow]
 # Datasets to load inputs. If not provided, datasets will be determined
 # automatically based on the input provider implementation:
 #input_datasets = []
 
 # Datasets to skip:
```

### Comparing `cpg-workflows-1.9.0/cpg_workflows/filetypes.py` & `cpg-workflows-1.9.1/cpg_workflows/filetypes.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/cpg_workflows/inputs.py` & `cpg-workflows-1.9.1/cpg_workflows/inputs.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/cpg_workflows/jobs/align.py` & `cpg-workflows-1.9.1/cpg_workflows/jobs/align.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/cpg_workflows/jobs/fastqc.py` & `cpg-workflows-1.9.1/cpg_workflows/jobs/fastqc.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/cpg_workflows/jobs/genotype.py` & `cpg-workflows-1.9.1/cpg_workflows/jobs/genotype.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/cpg_workflows/jobs/happy.py` & `cpg-workflows-1.9.1/cpg_workflows/jobs/happy.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/cpg_workflows/jobs/joint_genotyping.py` & `cpg-workflows-1.9.1/cpg_workflows/jobs/joint_genotyping.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/cpg_workflows/jobs/multiqc.py` & `cpg-workflows-1.9.1/cpg_workflows/jobs/multiqc.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/cpg_workflows/jobs/picard.py` & `cpg-workflows-1.9.1/cpg_workflows/jobs/picard.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/cpg_workflows/jobs/samtools.py` & `cpg-workflows-1.9.1/cpg_workflows/jobs/samtools.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/cpg_workflows/jobs/seqr_loader.py` & `cpg-workflows-1.9.1/cpg_workflows/jobs/seqr_loader.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/cpg_workflows/jobs/somalier.py` & `cpg-workflows-1.9.1/cpg_workflows/jobs/somalier.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/cpg_workflows/jobs/stripy.py` & `cpg-workflows-1.9.1/cpg_workflows/jobs/stripy.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/cpg_workflows/jobs/vcf.py` & `cpg-workflows-1.9.1/cpg_workflows/jobs/vcf.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/cpg_workflows/jobs/vep.py` & `cpg-workflows-1.9.1/cpg_workflows/jobs/vep.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/cpg_workflows/jobs/verifybamid.py` & `cpg-workflows-1.9.1/cpg_workflows/jobs/verifybamid.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/cpg_workflows/jobs/vqsr.py` & `cpg-workflows-1.9.1/cpg_workflows/jobs/vqsr.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/cpg_workflows/large_cohort/ancestry_pca.py` & `cpg-workflows-1.9.1/cpg_workflows/large_cohort/ancestry_pca.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/cpg_workflows/large_cohort/ancestry_plots.py` & `cpg-workflows-1.9.1/cpg_workflows/large_cohort/ancestry_plots.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/cpg_workflows/large_cohort/combiner.py` & `cpg-workflows-1.9.1/cpg_workflows/large_cohort/combiner.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/cpg_workflows/large_cohort/dataproc_script.py` & `cpg-workflows-1.9.1/cpg_workflows/large_cohort/dataproc_script.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/cpg_workflows/large_cohort/dataproc_utils.py` & `cpg-workflows-1.9.1/cpg_workflows/large_cohort/dataproc_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -47,28 +47,39 @@
     import cpg_workflows
     from cpg_workflows.large_cohort import dataproc_script
 
     package_path = to_path(cpg_workflows.__file__).parent
     script_path = to_path(dataproc_script.__file__)
     rel_script_path = script_path.relative_to(package_path.parent)
 
+    if not to_path(gnomad_path := 'gnomad_methods/gnomad').exists():
+        raise ValueError(
+            f'Cannot find gnomad_methods Git submodule: {gnomad_path}. Make sure '
+            f'you cloned the repo recursively with `git clone --recurse-submodules '
+            f'git@github.com:populationgenomics/production-pipelines.git`.'
+        )
+    pyfiles = [
+        cpg_workflows.__name__,
+        gnomad_path,
+    ]
+
     script = (
         f'{rel_script_path} '
         f'{function.__module__} {function.__name__} '
         f'{" ".join([f"-p {p}" for p in function_path_args.values()])} '
         f'{" ".join([a for a in function_str_args or []])} '
     )
 
     if cluster_id := get_config()['hail'].get('dataproc', {}).get('cluster_id'):
         # noinspection PyProtectedMember
         return dataproc._add_submit_job(
             batch=get_batch(),
             cluster_id=cluster_id,
             script=script,
-            pyfiles=[cpg_workflows.__name__],
+            pyfiles=pyfiles,
             job_name=job_name,
             region='australia-southeast1',
         )
 
     if num_workers is None:
         num_workers = get_config()['workflow']['scatter_count']
 
@@ -107,13 +118,10 @@
         num_secondary_workers=num_secondary_workers,
         num_workers=num_primary_workers,
         autoscaling_policy=autoscaling_policy,
         depends_on=depends_on,
         worker_machine_type='n1-highmem-8' if use_highmem_workers else 'n1-standard-8',
         worker_boot_disk_size=worker_boot_disk_size,
         secondary_worker_boot_disk_size=secondary_worker_boot_disk_size,
-        pyfiles=[
-            cpg_workflows.__name__,
-            'gnomad_methods/gnomad',
-        ],
+        pyfiles=pyfiles,
         init=['gs://cpg-common-main/hail_dataproc/install_common.sh'],
     )
```

### Comparing `cpg-workflows-1.9.0/cpg_workflows/large_cohort/dense_subset.py` & `cpg-workflows-1.9.1/cpg_workflows/large_cohort/dense_subset.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/cpg_workflows/large_cohort/frequencies.py` & `cpg-workflows-1.9.1/cpg_workflows/large_cohort/frequencies.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/cpg_workflows/large_cohort/load_vqsr.py` & `cpg-workflows-1.9.1/cpg_workflows/large_cohort/load_vqsr.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/cpg_workflows/large_cohort/relatedness.py` & `cpg-workflows-1.9.1/cpg_workflows/large_cohort/relatedness.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/cpg_workflows/large_cohort/sample_qc.py` & `cpg-workflows-1.9.1/cpg_workflows/large_cohort/sample_qc.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/cpg_workflows/large_cohort/site_only_vcf.py` & `cpg-workflows-1.9.1/cpg_workflows/large_cohort/site_only_vcf.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/cpg_workflows/metamist.py` & `cpg-workflows-1.9.1/cpg_workflows/metamist.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/cpg_workflows/python_scripts/check_multiqc.py` & `cpg-workflows-1.9.1/cpg_workflows/python_scripts/check_multiqc.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/cpg_workflows/python_scripts/check_pedigree.py` & `cpg-workflows-1.9.1/cpg_workflows/python_scripts/check_pedigree.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/cpg_workflows/query_modules/seqr_loader.py` & `cpg-workflows-1.9.1/cpg_workflows/query_modules/seqr_loader.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/cpg_workflows/query_modules/vep.py` & `cpg-workflows-1.9.1/cpg_workflows/query_modules/vep.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/cpg_workflows/resources.py` & `cpg-workflows-1.9.1/cpg_workflows/resources.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/cpg_workflows/slack.py` & `cpg-workflows-1.9.1/cpg_workflows/slack.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/cpg_workflows/stages/align.py` & `cpg-workflows-1.9.1/cpg_workflows/stages/align.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/cpg_workflows/stages/cram_qc.py` & `cpg-workflows-1.9.1/cpg_workflows/stages/cram_qc.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/cpg_workflows/stages/fastqc.py` & `cpg-workflows-1.9.1/cpg_workflows/stages/fastqc.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/cpg_workflows/stages/gatk_sv.py` & `cpg-workflows-1.9.1/cpg_workflows/stages/gatk_sv.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/cpg_workflows/stages/genotype.py` & `cpg-workflows-1.9.1/cpg_workflows/stages/genotype.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/cpg_workflows/stages/gvcf_qc.py` & `cpg-workflows-1.9.1/cpg_workflows/stages/gvcf_qc.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/cpg_workflows/stages/joint_genotyping.py` & `cpg-workflows-1.9.1/cpg_workflows/stages/joint_genotyping.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/cpg_workflows/stages/joint_genotyping_qc.py` & `cpg-workflows-1.9.1/cpg_workflows/stages/joint_genotyping_qc.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/cpg_workflows/stages/large_cohort.py` & `cpg-workflows-1.9.1/cpg_workflows/stages/large_cohort.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/cpg_workflows/stages/seqr_loader.py` & `cpg-workflows-1.9.1/cpg_workflows/stages/seqr_loader.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/cpg_workflows/stages/stripy.py` & `cpg-workflows-1.9.1/cpg_workflows/stages/stripy.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/cpg_workflows/stages/vep.py` & `cpg-workflows-1.9.1/cpg_workflows/stages/vep.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/cpg_workflows/stages/vqsr.py` & `cpg-workflows-1.9.1/cpg_workflows/stages/vqsr.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/cpg_workflows/status.py` & `cpg-workflows-1.9.1/cpg_workflows/status.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/cpg_workflows/targets.py` & `cpg-workflows-1.9.1/cpg_workflows/targets.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/cpg_workflows/utils.py` & `cpg-workflows-1.9.1/cpg_workflows/utils.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/cpg_workflows/workflow.py` & `cpg-workflows-1.9.1/cpg_workflows/workflow.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/cpg_workflows.egg-info/PKG-INFO` & `cpg-workflows-1.9.1/cpg_workflows.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpg-workflows
-Version: 1.9.0
+Version: 1.9.1
 Summary: CPG workflows for Hail Batch
 Home-page: https://github.com/populationgenomics/production-pipelines
 License: MIT
 Keywords: bioinformatics
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cpg-workflows-1.9.0/cpg_workflows.egg-info/SOURCES.txt` & `cpg-workflows-1.9.1/cpg_workflows.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/setup.py` & `cpg-workflows-1.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 
 from setuptools import find_packages, setup
 
 setup(
     name='cpg-workflows',
     # This tag is automatically updated by bumpversion
-    version='1.9.0',
+    version='1.9.1',
     description='CPG workflows for Hail Batch',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url=f'https://github.com/populationgenomics/production-pipelines',
     license='MIT',
     packages=find_packages(),
     install_requires=[
```

### Comparing `cpg-workflows-1.9.0/test/__init__.py` & `cpg-workflows-1.9.1/test/__init__.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/test/conftest.py` & `cpg-workflows-1.9.1/test/conftest.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/test/stages/__init__.py` & `cpg-workflows-1.9.1/test/stages/__init__.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/test/stages/test_first_last_stages.py` & `cpg-workflows-1.9.1/test/stages/test_first_last_stages.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/test/stages/test_first_last_stages_misconfigured.py` & `cpg-workflows-1.9.1/test/stages/test_first_last_stages_misconfigured.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/test/stages/test_first_stages.py` & `cpg-workflows-1.9.1/test/stages/test_first_stages.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/test/stages/test_force_stages.py` & `cpg-workflows-1.9.1/test/stages/test_force_stages.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/test/stages/test_last_stages.py` & `cpg-workflows-1.9.1/test/stages/test_last_stages.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/test/stages/test_skip_stages.py` & `cpg-workflows-1.9.1/test/stages/test_skip_stages.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/test/stages/test_skip_stages_fail.py` & `cpg-workflows-1.9.1/test/stages/test_skip_stages_fail.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/test/test_batch.py` & `cpg-workflows-1.9.1/test/test_batch.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/test/test_check_multiqc.py` & `cpg-workflows-1.9.1/test/test_check_multiqc.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/test/test_check_pedigree.py` & `cpg-workflows-1.9.1/test/test_check_pedigree.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/test/test_cohort.py` & `cpg-workflows-1.9.1/test/test_cohort.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/test/test_large_cohort.py` & `cpg-workflows-1.9.1/test/test_large_cohort.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/test/test_seqr_loader_dry.py` & `cpg-workflows-1.9.1/test/test_seqr_loader_dry.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/test/test_status.py` & `cpg-workflows-1.9.1/test/test_status.py`

 * *Files identical despite different names*

### Comparing `cpg-workflows-1.9.0/test/test_workflow.py` & `cpg-workflows-1.9.1/test/test_workflow.py`

 * *Files identical despite different names*

