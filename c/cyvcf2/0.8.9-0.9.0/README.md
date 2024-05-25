# Comparing `tmp/cyvcf2-0.8.9.tar.gz` & `tmp/cyvcf2-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cyvcf2-0.8.9.tar", last modified: Sat May 12 16:45:08 2018, max compression
+gzip compressed data, was "dist/cyvcf2-0.9.0.tar", last modified: Wed May 30 22:52:53 2018, max compression
```

## Comparing `cyvcf2-0.8.9.tar` & `cyvcf2-0.9.0.tar`

### file list

```diff
@@ -1,149 +1,149 @@
-drwxrwxr-x   0 brentp    (1000) brentp    (1000)        0 2018-05-12 16:45:08.000000 cyvcf2-0.8.9/
-drwxrwxr-x   0 brentp    (1000) brentp    (1000)        0 2018-05-12 16:45:08.000000 cyvcf2-0.8.9/htslib/
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     6354 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/errmod.c
-drwxrwxr-x   0 brentp    (1000) brentp    (1000)        0 2018-05-12 16:45:08.000000 cyvcf2-0.8.9/htslib/htslib/
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     4579 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/htslib/faidx.h
--rw-rw-r--   0 brentp    (1000) brentp    (1000)    23336 2018-05-12 16:14:38.000000 cyvcf2-0.8.9/htslib/htslib/hts.h
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     5845 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/htslib/regidx.h
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     1602 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/htslib/vcf_sweep.h
--rw-rw-r--   0 brentp    (1000) brentp    (1000)    21540 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/htslib/khash.h
--rw-rw-r--   0 brentp    (1000) brentp    (1000)    17612 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/htslib/sam.h
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     3990 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/htslib/khash_str2int.h
--rw-rw-r--   0 brentp    (1000) brentp    (1000)    15393 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/htslib/cram.h
--rw-rw-r--   0 brentp    (1000) brentp    (1000)    10125 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/htslib/ksort.h
--rw-rw-r--   0 brentp    (1000) brentp    (1000)    41240 2017-04-12 15:52:12.000000 cyvcf2-0.8.9/htslib/htslib/vcf.h
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     4195 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/htslib/kbitset.h
--rw-rw-r--   0 brentp    (1000) brentp    (1000)    11481 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/htslib/bgzf.h
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     4675 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/htslib/vcfutils.h
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     5086 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/htslib/klist.h
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     2451 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/htslib/hts_defs.h
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     6868 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/htslib/kstring.h
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     7127 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/htslib/hfile.h
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     2997 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/htslib/tbx.h
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     2828 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/htslib/knetfile.h
--rw-rw-r--   0 brentp    (1000) brentp    (1000)    12682 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/htslib/synced_bcf_reader.h
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     2716 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/htslib/kfunc.h
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     8900 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/htslib/kseq.h
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     5321 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/vcf_sweep.c
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     3192 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/hfile_net.c
--rw-rw-r--   0 brentp    (1000) brentp    (1000)    70504 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/sam.c
--rw-rw-r--   0 brentp    (1000) brentp    (1000)    64261 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/hts.c
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     8634 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/realn.c
--rw-rw-r--   0 brentp    (1000) brentp    (1000)       41 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/version.h
--rw-rw-r--   0 brentp    (1000) brentp    (1000)    41894 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/bgzf.c
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     3748 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/hts_internal.h
--rw-rw-r--   0 brentp    (1000) brentp    (1000)    19907 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/tabix.c
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     9166 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/kfunc.c
--rw-rw-r--   0 brentp    (1000) brentp    (1000)    26673 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/vcfutils.c
--rw-rw-r--   0 brentp    (1000) brentp    (1000)    42027 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/synced_bcf_reader.c
--rw-rw-r--   0 brentp    (1000) brentp    (1000)    10622 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/tbx.c
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     4904 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/plugin.c
--rw-rw-r--   0 brentp    (1000) brentp    (1000)    11649 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/probaln.c
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     7363 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/hfile_irods.c
--rw-rw-r--   0 brentp    (1000) brentp    (1000)   121323 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/vcf.c
--rw-rw-r--   0 brentp    (1000) brentp    (1000)    18861 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/knetfile.c
-drwxrwxr-x   0 brentp    (1000) brentp    (1000)        0 2018-05-12 16:45:08.000000 cyvcf2-0.8.9/htslib/cram/
--rw-rw-r--   0 brentp    (1000) brentp    (1000)    21060 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/cram/rANS_static.c
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     2473 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/cram/files.c
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     2320 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/cram/string_alloc.h
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     2163 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/cram/pooled_alloc.h
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     3599 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/cram/cram_encode.h
--rw-rw-r--   0 brentp    (1000) brentp    (1000)    14040 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/cram/sam_header.h
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     6658 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/cram/thread_pool.h
--rw-rw-r--   0 brentp    (1000) brentp    (1000)    29679 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/cram/sam_header.c
--rw-rw-r--   0 brentp    (1000) brentp    (1000)    48438 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/cram/cram_codecs.c
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     2419 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/cram/cram.h
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     3020 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/cram/mFILE.h
--rw-rw-r--   0 brentp    (1000) brentp    (1000)    14862 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/cram/cram_index.c
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     2090 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/cram/zfio.h
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     4306 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/cram/misc.h
--rw-rw-r--   0 brentp    (1000) brentp    (1000)    11828 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/cram/rANS_byte.h
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     5025 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/cram/open_trace_file.h
--rw-rw-r--   0 brentp    (1000) brentp    (1000)    92213 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/cram/cram_encode.c
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     2033 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/cram/rANS_static.h
--rw-rw-r--   0 brentp    (1000) brentp    (1000)    12890 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/cram/cram_external.c
--rw-rw-r--   0 brentp    (1000) brentp    (1000)    11683 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/cram/open_trace_file.c
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     6052 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/cram/cram_codecs.h
--rw-rw-r--   0 brentp    (1000) brentp    (1000)    16775 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/cram/mFILE.c
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     5376 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/cram/cram_stats.c
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     3515 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/cram/cram_decode.h
--rw-rw-r--   0 brentp    (1000) brentp    (1000)    22888 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/cram/cram_structs.h
--rw-rw-r--   0 brentp    (1000) brentp    (1000)   114351 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/cram/cram_io.c
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     4585 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/cram/pooled_alloc.c
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     3363 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/cram/cram_index.h
--rw-rw-r--   0 brentp    (1000) brentp    (1000)    19054 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/cram/cram_io.h
--rw-rw-r--   0 brentp    (1000) brentp    (1000)    84373 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/cram/cram_decode.c
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     4912 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/cram/cram_samtools.c
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     3558 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/cram/cram_samtools.h
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     1815 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/cram/vlen.h
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     2279 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/cram/cram_stats.h
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     4178 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/cram/string_alloc.c
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     4237 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/cram/zfio.c
--rw-rw-r--   0 brentp    (1000) brentp    (1000)    17936 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/cram/thread_pool.c
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     9388 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/cram/os.h
--rw-rw-r--   0 brentp    (1000) brentp    (1000)    12210 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/cram/vlen.c
--rw-rw-r--   0 brentp    (1000) brentp    (1000)       43 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/config.h
--rw-rw-r--   0 brentp    (1000) brentp    (1000)    21033 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/hfile.c
--rw-rw-r--   0 brentp    (1000) brentp    (1000)    15162 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/faidx.c
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     5629 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/hfile_internal.h
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     7283 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/kstring.c
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     6809 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/htsfile.c
--rw-rw-r--   0 brentp    (1000) brentp    (1000)    10554 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/md5.c
--rw-rw-r--   0 brentp    (1000) brentp    (1000)    11538 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/bgzip.c
--rw-rw-r--   0 brentp    (1000) brentp    (1000)    10205 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/htslib/regidx.c
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     1099 2017-02-22 17:36:31.000000 cyvcf2-0.8.9/LICENSE
--rw-rw-r--   0 brentp    (1000) brentp    (1000)      244 2017-02-22 17:36:31.000000 cyvcf2-0.8.9/MANIFEST.in
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     3828 2017-06-27 18:25:30.000000 cyvcf2-0.8.9/README.md
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     5087 2018-05-12 16:45:08.000000 cyvcf2-0.8.9/PKG-INFO
-drwxrwxr-x   0 brentp    (1000) brentp    (1000)        0 2018-05-12 16:45:08.000000 cyvcf2-0.8.9/cyvcf2/
--rw-rw-r--   0 brentp    (1000) brentp    (1000)  2639298 2018-05-12 16:40:33.000000 cyvcf2-0.8.9/cyvcf2/cyvcf2.c
--rw-rw-r--   0 brentp    (1000) brentp    (1000)      326 2017-06-27 18:25:30.000000 cyvcf2-0.8.9/cyvcf2/__main__.py
-drwxrwxr-x   0 brentp    (1000) brentp    (1000)        0 2018-05-12 16:45:08.000000 cyvcf2-0.8.9/cyvcf2/tests/
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     2332 2017-10-09 19:40:29.000000 cyvcf2-0.8.9/cyvcf2/tests/test-alt-repr-1.vcf
--rw-rw-r--   0 brentp    (1000) brentp    (1000)      878 2017-04-12 16:10:43.000000 cyvcf2-0.8.9/cyvcf2/tests/seg.vcf.gz
--rw-rw-r--   0 brentp    (1000) brentp    (1000)    34898 2018-05-12 16:41:29.000000 cyvcf2-0.8.9/cyvcf2/tests/test_reader.pyc
--rw-rw-r--   0 brentp    (1000) brentp    (1000)      103 2017-06-27 18:25:30.000000 cyvcf2-0.8.9/cyvcf2/tests/test-strict-gt-option-flag.vcf.gz.tbi
--rw-rw-r--   0 brentp    (1000) brentp    (1000)    19144 2017-10-09 19:27:37.000000 cyvcf2-0.8.9/cyvcf2/tests/test.comp_het.3.vcf
--rw-rw-r--   0 brentp    (1000) brentp    (1000)    20052 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/cyvcf2/tests/test-hemi.vcf
--rw-rw-r--   0 brentp    (1000) brentp    (1000)      117 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/cyvcf2/tests/test.snpeff.bcf.csi
--rw-rw-r--   0 brentp    (1000) brentp    (1000)   174816 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/cyvcf2/tests/test.vcf.gz
--rw-rw-r--   0 brentp    (1000) brentp    (1000)      368 2017-06-27 18:25:30.000000 cyvcf2-0.8.9/cyvcf2/tests/test-strict-gt-option-flag.vcf.gz
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     5389 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/cyvcf2/tests/bug.vcf.gz
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     2721 2017-04-17 21:54:00.000000 cyvcf2-0.8.9/cyvcf2/tests/test-issue-48.vcf.gz
--rw-rw-r--   0 brentp    (1000) brentp    (1000)   597572 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/cyvcf2/tests/test-haploidX.vcf
--rw-rw-r--   0 brentp    (1000) brentp    (1000)      104 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/cyvcf2/tests/test-multiallelic-homozygous-alt.vcf.gz.tbi
--rw-rw-r--   0 brentp    (1000) brentp    (1000)      588 2017-05-01 14:52:21.000000 cyvcf2-0.8.9/cyvcf2/tests/issue_44.vcf
--rw-rw-r--   0 brentp    (1000) brentp    (1000)    48729 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/cyvcf2/tests/o.vcf.gz
--rw-rw-r--   0 brentp    (1000) brentp    (1000)      327 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/cyvcf2/tests/test-multiallelic-homozygous-alt.vcf.gz
--rw-rw-r--   0 brentp    (1000) brentp    (1000)      881 2018-02-20 17:04:23.000000 cyvcf2-0.8.9/cyvcf2/tests/test-format-string.vcf
--rw-rw-r--   0 brentp    (1000) brentp    (1000)      135 2017-03-17 14:09:56.000000 cyvcf2-0.8.9/cyvcf2/tests/__init__.pyc
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     6188 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/cyvcf2/tests/test_gt_bases.vcf.gz
--rw-rw-r--   0 brentp    (1000) brentp    (1000)   937104 2017-10-26 14:34:39.000000 cyvcf2-0.8.9/cyvcf2/tests/test.t.vcf
--rw-rw-r--   0 brentp    (1000) brentp    (1000)        0 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/cyvcf2/tests/empty.vcf
--rw-rw-r--   0 brentp    (1000) brentp    (1000)        2 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/cyvcf2/tests/__init__.py
--rw-rw-r--   0 brentp    (1000) brentp    (1000)      103 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/cyvcf2/tests/test.vcf.gz.tbi
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     1496 2017-10-09 20:18:59.000000 cyvcf2-0.8.9/cyvcf2/tests/test_hemi.pyc
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     5121 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/cyvcf2/tests/test.snpeff.bcf
--rw-rw-r--   0 brentp    (1000) brentp    (1000)    17254 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/cyvcf2/tests/test.snpeff.vcf
--rw-rw-r--   0 brentp    (1000) brentp    (1000)      767 2017-10-09 20:18:57.000000 cyvcf2-0.8.9/cyvcf2/tests/test_hemi.py
--rw-rw-r--   0 brentp    (1000) brentp    (1000)    21089 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/cyvcf2/tests/test_gt_alt_freqs.vcf
--rw-rw-r--   0 brentp    (1000) brentp    (1000)      456 2018-03-01 17:07:08.000000 cyvcf2-0.8.9/cyvcf2/tests/decomposed.vcf
--rw-rw-r--   0 brentp    (1000) brentp    (1000)    26045 2018-05-12 16:42:52.000000 cyvcf2-0.8.9/cyvcf2/tests/test_reader.py
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     2555 2017-12-06 16:17:08.000000 cyvcf2-0.8.9/cyvcf2/tests/test-alt-repr.vcf
--rw-rw-r--   0 brentp    (1000) brentp    (1000)    73755 2018-05-12 16:40:28.000000 cyvcf2-0.8.9/cyvcf2/cyvcf2.pyx
--rw-rw-r--   0 brentp    (1000) brentp    (1000)      248 2017-10-26 14:10:47.000000 cyvcf2-0.8.9/cyvcf2/helpers.h
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     6288 2018-03-22 16:23:34.000000 cyvcf2-0.8.9/cyvcf2/relatedness.h
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     3448 2017-10-26 14:33:27.000000 cyvcf2-0.8.9/cyvcf2/helpers.c
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     4099 2017-06-27 18:25:30.000000 cyvcf2-0.8.9/cyvcf2/cli.py
--rw-rw-r--   0 brentp    (1000) brentp    (1000)    12080 2018-05-12 16:33:59.000000 cyvcf2-0.8.9/cyvcf2/cyvcf2.pxd
--rw-rw-r--   0 brentp    (1000) brentp    (1000)      156 2018-05-12 16:44:02.000000 cyvcf2-0.8.9/cyvcf2/__init__.py
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     2844 2017-09-08 19:19:06.000000 cyvcf2-0.8.9/setup.py
-drwxrwxr-x   0 brentp    (1000) brentp    (1000)        0 2018-05-12 16:45:08.000000 cyvcf2-0.8.9/cyvcf2.egg-info/
--rw-rw-r--   0 brentp    (1000) brentp    (1000)        1 2017-02-22 17:39:45.000000 cyvcf2-0.8.9/cyvcf2.egg-info/not-zip-safe
--rw-rw-r--   0 brentp    (1000) brentp    (1000)        1 2018-05-12 16:45:08.000000 cyvcf2-0.8.9/cyvcf2.egg-info/dependency_links.txt
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     5087 2018-05-12 16:45:08.000000 cyvcf2-0.8.9/cyvcf2.egg-info/PKG-INFO
--rw-rw-r--   0 brentp    (1000) brentp    (1000)        6 2018-05-12 16:45:08.000000 cyvcf2-0.8.9/cyvcf2.egg-info/requires.txt
--rw-rw-r--   0 brentp    (1000) brentp    (1000)     3325 2018-05-12 16:45:08.000000 cyvcf2-0.8.9/cyvcf2.egg-info/SOURCES.txt
--rw-rw-r--   0 brentp    (1000) brentp    (1000)       48 2018-05-12 16:45:08.000000 cyvcf2-0.8.9/cyvcf2.egg-info/entry_points.txt
--rw-rw-r--   0 brentp    (1000) brentp    (1000)        7 2018-05-12 16:45:08.000000 cyvcf2-0.8.9/cyvcf2.egg-info/top_level.txt
--rw-rw-r--   0 brentp    (1000) brentp    (1000)      112 2018-05-12 16:45:08.000000 cyvcf2-0.8.9/setup.cfg
+drwxrwxr-x   0 brentp    (1000) brentp    (1000)        0 2018-05-30 22:52:53.000000 cyvcf2-0.9.0/
+drwxrwxr-x   0 brentp    (1000) brentp    (1000)        0 2018-05-30 22:52:53.000000 cyvcf2-0.9.0/htslib/
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     6354 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/errmod.c
+drwxrwxr-x   0 brentp    (1000) brentp    (1000)        0 2018-05-30 22:52:53.000000 cyvcf2-0.9.0/htslib/htslib/
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     4579 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/htslib/faidx.h
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)    23336 2018-05-12 16:14:38.000000 cyvcf2-0.9.0/htslib/htslib/hts.h
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     5845 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/htslib/regidx.h
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     1602 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/htslib/vcf_sweep.h
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)    21540 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/htslib/khash.h
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)    17612 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/htslib/sam.h
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     3990 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/htslib/khash_str2int.h
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)    15393 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/htslib/cram.h
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)    10125 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/htslib/ksort.h
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)    41240 2017-04-12 15:52:12.000000 cyvcf2-0.9.0/htslib/htslib/vcf.h
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     4195 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/htslib/kbitset.h
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)    11481 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/htslib/bgzf.h
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     4675 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/htslib/vcfutils.h
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     5086 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/htslib/klist.h
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     2451 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/htslib/hts_defs.h
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     6868 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/htslib/kstring.h
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     7127 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/htslib/hfile.h
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     2997 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/htslib/tbx.h
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     2828 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/htslib/knetfile.h
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)    12682 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/htslib/synced_bcf_reader.h
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     2716 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/htslib/kfunc.h
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     8900 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/htslib/kseq.h
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     5321 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/vcf_sweep.c
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     3192 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/hfile_net.c
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)    70504 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/sam.c
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)    64261 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/hts.c
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     8634 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/realn.c
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)       41 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/version.h
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)    41894 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/bgzf.c
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     3748 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/hts_internal.h
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)    19907 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/tabix.c
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     9166 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/kfunc.c
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)    26673 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/vcfutils.c
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)    42027 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/synced_bcf_reader.c
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)    10622 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/tbx.c
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     4904 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/plugin.c
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)    11649 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/probaln.c
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     7363 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/hfile_irods.c
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)   121323 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/vcf.c
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)    18861 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/knetfile.c
+drwxrwxr-x   0 brentp    (1000) brentp    (1000)        0 2018-05-30 22:52:53.000000 cyvcf2-0.9.0/htslib/cram/
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)    21060 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/cram/rANS_static.c
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     2473 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/cram/files.c
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     2320 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/cram/string_alloc.h
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     2163 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/cram/pooled_alloc.h
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     3599 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/cram/cram_encode.h
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)    14040 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/cram/sam_header.h
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     6658 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/cram/thread_pool.h
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)    29679 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/cram/sam_header.c
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)    48438 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/cram/cram_codecs.c
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     2419 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/cram/cram.h
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     3020 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/cram/mFILE.h
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)    14862 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/cram/cram_index.c
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     2090 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/cram/zfio.h
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     4306 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/cram/misc.h
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)    11828 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/cram/rANS_byte.h
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     5025 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/cram/open_trace_file.h
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)    92213 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/cram/cram_encode.c
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     2033 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/cram/rANS_static.h
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)    12890 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/cram/cram_external.c
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)    11683 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/cram/open_trace_file.c
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     6052 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/cram/cram_codecs.h
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)    16775 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/cram/mFILE.c
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     5376 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/cram/cram_stats.c
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     3515 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/cram/cram_decode.h
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)    22888 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/cram/cram_structs.h
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)   114351 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/cram/cram_io.c
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     4585 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/cram/pooled_alloc.c
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     3363 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/cram/cram_index.h
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)    19054 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/cram/cram_io.h
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)    84373 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/cram/cram_decode.c
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     4912 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/cram/cram_samtools.c
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     3558 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/cram/cram_samtools.h
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     1815 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/cram/vlen.h
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     2279 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/cram/cram_stats.h
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     4178 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/cram/string_alloc.c
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     4237 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/cram/zfio.c
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)    17936 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/cram/thread_pool.c
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     9388 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/cram/os.h
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)    12210 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/cram/vlen.c
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)       43 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/config.h
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)    21033 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/hfile.c
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)    15162 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/faidx.c
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     5629 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/hfile_internal.h
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     7283 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/kstring.c
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     6809 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/htsfile.c
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)    10554 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/md5.c
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)    11538 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/bgzip.c
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)    10205 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/htslib/regidx.c
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     1099 2017-02-22 17:36:31.000000 cyvcf2-0.9.0/LICENSE
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)      244 2017-02-22 17:36:31.000000 cyvcf2-0.9.0/MANIFEST.in
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     3828 2017-06-27 18:25:30.000000 cyvcf2-0.9.0/README.md
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     5087 2018-05-30 22:52:53.000000 cyvcf2-0.9.0/PKG-INFO
+drwxrwxr-x   0 brentp    (1000) brentp    (1000)        0 2018-05-30 22:52:53.000000 cyvcf2-0.9.0/cyvcf2/
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)  2639298 2018-05-30 22:50:38.000000 cyvcf2-0.9.0/cyvcf2/cyvcf2.c
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)      326 2017-06-27 18:25:30.000000 cyvcf2-0.9.0/cyvcf2/__main__.py
+drwxrwxr-x   0 brentp    (1000) brentp    (1000)        0 2018-05-30 22:52:53.000000 cyvcf2-0.9.0/cyvcf2/tests/
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     2332 2017-10-09 19:40:29.000000 cyvcf2-0.9.0/cyvcf2/tests/test-alt-repr-1.vcf
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)      878 2017-04-12 16:10:43.000000 cyvcf2-0.9.0/cyvcf2/tests/seg.vcf.gz
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)    34898 2018-05-12 16:41:29.000000 cyvcf2-0.9.0/cyvcf2/tests/test_reader.pyc
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)      103 2017-06-27 18:25:30.000000 cyvcf2-0.9.0/cyvcf2/tests/test-strict-gt-option-flag.vcf.gz.tbi
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)    19144 2017-10-09 19:27:37.000000 cyvcf2-0.9.0/cyvcf2/tests/test.comp_het.3.vcf
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)    20052 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/cyvcf2/tests/test-hemi.vcf
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)      117 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/cyvcf2/tests/test.snpeff.bcf.csi
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)   174816 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/cyvcf2/tests/test.vcf.gz
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)      368 2017-06-27 18:25:30.000000 cyvcf2-0.9.0/cyvcf2/tests/test-strict-gt-option-flag.vcf.gz
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     5389 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/cyvcf2/tests/bug.vcf.gz
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     2721 2017-04-17 21:54:00.000000 cyvcf2-0.9.0/cyvcf2/tests/test-issue-48.vcf.gz
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)   597572 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/cyvcf2/tests/test-haploidX.vcf
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)      104 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/cyvcf2/tests/test-multiallelic-homozygous-alt.vcf.gz.tbi
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)      588 2017-05-01 14:52:21.000000 cyvcf2-0.9.0/cyvcf2/tests/issue_44.vcf
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)    48729 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/cyvcf2/tests/o.vcf.gz
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)      327 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/cyvcf2/tests/test-multiallelic-homozygous-alt.vcf.gz
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)      881 2018-02-20 17:04:23.000000 cyvcf2-0.9.0/cyvcf2/tests/test-format-string.vcf
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)      135 2017-03-17 14:09:56.000000 cyvcf2-0.9.0/cyvcf2/tests/__init__.pyc
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     6188 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/cyvcf2/tests/test_gt_bases.vcf.gz
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)   937104 2017-10-26 14:34:39.000000 cyvcf2-0.9.0/cyvcf2/tests/test.t.vcf
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)        0 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/cyvcf2/tests/empty.vcf
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)        2 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/cyvcf2/tests/__init__.py
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)      103 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/cyvcf2/tests/test.vcf.gz.tbi
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     1496 2017-10-09 20:18:59.000000 cyvcf2-0.9.0/cyvcf2/tests/test_hemi.pyc
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     5121 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/cyvcf2/tests/test.snpeff.bcf
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)    17254 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/cyvcf2/tests/test.snpeff.vcf
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)      767 2017-10-09 20:18:57.000000 cyvcf2-0.9.0/cyvcf2/tests/test_hemi.py
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)    21089 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/cyvcf2/tests/test_gt_alt_freqs.vcf
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)      456 2018-03-01 17:07:08.000000 cyvcf2-0.9.0/cyvcf2/tests/decomposed.vcf
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)    26045 2018-05-12 16:42:52.000000 cyvcf2-0.9.0/cyvcf2/tests/test_reader.py
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     2555 2017-12-06 16:17:08.000000 cyvcf2-0.9.0/cyvcf2/tests/test-alt-repr.vcf
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)    73851 2018-05-30 22:51:34.000000 cyvcf2-0.9.0/cyvcf2/cyvcf2.pyx
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)      248 2017-10-26 14:10:47.000000 cyvcf2-0.9.0/cyvcf2/helpers.h
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     6288 2018-03-22 16:23:34.000000 cyvcf2-0.9.0/cyvcf2/relatedness.h
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     3448 2017-10-26 14:33:27.000000 cyvcf2-0.9.0/cyvcf2/helpers.c
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     4099 2017-06-27 18:25:30.000000 cyvcf2-0.9.0/cyvcf2/cli.py
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)    12080 2018-05-12 16:33:59.000000 cyvcf2-0.9.0/cyvcf2/cyvcf2.pxd
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)      156 2018-05-30 22:52:17.000000 cyvcf2-0.9.0/cyvcf2/__init__.py
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     2868 2018-05-12 16:48:41.000000 cyvcf2-0.9.0/setup.py
+drwxrwxr-x   0 brentp    (1000) brentp    (1000)        0 2018-05-30 22:52:53.000000 cyvcf2-0.9.0/cyvcf2.egg-info/
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)        1 2017-02-22 17:39:45.000000 cyvcf2-0.9.0/cyvcf2.egg-info/not-zip-safe
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)        1 2018-05-30 22:52:53.000000 cyvcf2-0.9.0/cyvcf2.egg-info/dependency_links.txt
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     5087 2018-05-30 22:52:53.000000 cyvcf2-0.9.0/cyvcf2.egg-info/PKG-INFO
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)        6 2018-05-30 22:52:53.000000 cyvcf2-0.9.0/cyvcf2.egg-info/requires.txt
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)     3325 2018-05-30 22:52:53.000000 cyvcf2-0.9.0/cyvcf2.egg-info/SOURCES.txt
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)       48 2018-05-30 22:52:53.000000 cyvcf2-0.9.0/cyvcf2.egg-info/entry_points.txt
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)        7 2018-05-30 22:52:53.000000 cyvcf2-0.9.0/cyvcf2.egg-info/top_level.txt
+-rw-rw-r--   0 brentp    (1000) brentp    (1000)      112 2018-05-30 22:52:53.000000 cyvcf2-0.9.0/setup.cfg
```

### Comparing `cyvcf2-0.8.9/htslib/errmod.c` & `cyvcf2-0.9.0/htslib/errmod.c`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/htslib/faidx.h` & `cyvcf2-0.9.0/htslib/htslib/faidx.h`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/htslib/hts.h` & `cyvcf2-0.9.0/htslib/htslib/hts.h`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/htslib/regidx.h` & `cyvcf2-0.9.0/htslib/htslib/regidx.h`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/htslib/vcf_sweep.h` & `cyvcf2-0.9.0/htslib/htslib/vcf_sweep.h`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/htslib/khash.h` & `cyvcf2-0.9.0/htslib/htslib/khash.h`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/htslib/sam.h` & `cyvcf2-0.9.0/htslib/htslib/sam.h`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/htslib/khash_str2int.h` & `cyvcf2-0.9.0/htslib/htslib/khash_str2int.h`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/htslib/cram.h` & `cyvcf2-0.9.0/htslib/htslib/cram.h`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/htslib/ksort.h` & `cyvcf2-0.9.0/htslib/htslib/ksort.h`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/htslib/vcf.h` & `cyvcf2-0.9.0/htslib/htslib/vcf.h`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/htslib/kbitset.h` & `cyvcf2-0.9.0/htslib/htslib/kbitset.h`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/htslib/bgzf.h` & `cyvcf2-0.9.0/htslib/htslib/bgzf.h`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/htslib/vcfutils.h` & `cyvcf2-0.9.0/htslib/htslib/vcfutils.h`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/htslib/klist.h` & `cyvcf2-0.9.0/htslib/htslib/klist.h`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/htslib/hts_defs.h` & `cyvcf2-0.9.0/htslib/htslib/hts_defs.h`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/htslib/kstring.h` & `cyvcf2-0.9.0/htslib/htslib/kstring.h`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/htslib/hfile.h` & `cyvcf2-0.9.0/htslib/htslib/hfile.h`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/htslib/tbx.h` & `cyvcf2-0.9.0/htslib/htslib/tbx.h`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/htslib/knetfile.h` & `cyvcf2-0.9.0/htslib/htslib/knetfile.h`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/htslib/synced_bcf_reader.h` & `cyvcf2-0.9.0/htslib/htslib/synced_bcf_reader.h`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/htslib/kfunc.h` & `cyvcf2-0.9.0/htslib/htslib/kfunc.h`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/htslib/kseq.h` & `cyvcf2-0.9.0/htslib/htslib/kseq.h`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/vcf_sweep.c` & `cyvcf2-0.9.0/htslib/vcf_sweep.c`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/hfile_net.c` & `cyvcf2-0.9.0/htslib/hfile_net.c`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/sam.c` & `cyvcf2-0.9.0/htslib/sam.c`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/hts.c` & `cyvcf2-0.9.0/htslib/hts.c`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/realn.c` & `cyvcf2-0.9.0/htslib/realn.c`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/bgzf.c` & `cyvcf2-0.9.0/htslib/bgzf.c`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/hts_internal.h` & `cyvcf2-0.9.0/htslib/hts_internal.h`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/tabix.c` & `cyvcf2-0.9.0/htslib/tabix.c`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/kfunc.c` & `cyvcf2-0.9.0/htslib/kfunc.c`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/vcfutils.c` & `cyvcf2-0.9.0/htslib/vcfutils.c`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/synced_bcf_reader.c` & `cyvcf2-0.9.0/htslib/synced_bcf_reader.c`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/tbx.c` & `cyvcf2-0.9.0/htslib/tbx.c`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/plugin.c` & `cyvcf2-0.9.0/htslib/plugin.c`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/probaln.c` & `cyvcf2-0.9.0/htslib/probaln.c`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/hfile_irods.c` & `cyvcf2-0.9.0/htslib/hfile_irods.c`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/vcf.c` & `cyvcf2-0.9.0/htslib/vcf.c`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/knetfile.c` & `cyvcf2-0.9.0/htslib/knetfile.c`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/cram/rANS_static.c` & `cyvcf2-0.9.0/htslib/cram/rANS_static.c`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/cram/files.c` & `cyvcf2-0.9.0/htslib/cram/files.c`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/cram/string_alloc.h` & `cyvcf2-0.9.0/htslib/cram/string_alloc.h`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/cram/pooled_alloc.h` & `cyvcf2-0.9.0/htslib/cram/pooled_alloc.h`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/cram/cram_encode.h` & `cyvcf2-0.9.0/htslib/cram/cram_encode.h`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/cram/sam_header.h` & `cyvcf2-0.9.0/htslib/cram/sam_header.h`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/cram/thread_pool.h` & `cyvcf2-0.9.0/htslib/cram/thread_pool.h`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/cram/sam_header.c` & `cyvcf2-0.9.0/htslib/cram/sam_header.c`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/cram/cram_codecs.c` & `cyvcf2-0.9.0/htslib/cram/cram_codecs.c`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/cram/cram.h` & `cyvcf2-0.9.0/htslib/cram/cram.h`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/cram/mFILE.h` & `cyvcf2-0.9.0/htslib/cram/mFILE.h`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/cram/cram_index.c` & `cyvcf2-0.9.0/htslib/cram/cram_index.c`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/cram/zfio.h` & `cyvcf2-0.9.0/htslib/cram/zfio.h`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/cram/misc.h` & `cyvcf2-0.9.0/htslib/cram/misc.h`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/cram/rANS_byte.h` & `cyvcf2-0.9.0/htslib/cram/rANS_byte.h`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/cram/open_trace_file.h` & `cyvcf2-0.9.0/htslib/cram/open_trace_file.h`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/cram/cram_encode.c` & `cyvcf2-0.9.0/htslib/cram/cram_encode.c`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/cram/rANS_static.h` & `cyvcf2-0.9.0/htslib/cram/rANS_static.h`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/cram/cram_external.c` & `cyvcf2-0.9.0/htslib/cram/cram_external.c`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/cram/open_trace_file.c` & `cyvcf2-0.9.0/htslib/cram/open_trace_file.c`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/cram/cram_codecs.h` & `cyvcf2-0.9.0/htslib/cram/cram_codecs.h`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/cram/mFILE.c` & `cyvcf2-0.9.0/htslib/cram/mFILE.c`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/cram/cram_stats.c` & `cyvcf2-0.9.0/htslib/cram/cram_stats.c`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/cram/cram_decode.h` & `cyvcf2-0.9.0/htslib/cram/cram_decode.h`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/cram/cram_structs.h` & `cyvcf2-0.9.0/htslib/cram/cram_structs.h`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/cram/cram_io.c` & `cyvcf2-0.9.0/htslib/cram/cram_io.c`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/cram/pooled_alloc.c` & `cyvcf2-0.9.0/htslib/cram/pooled_alloc.c`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/cram/cram_index.h` & `cyvcf2-0.9.0/htslib/cram/cram_index.h`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/cram/cram_io.h` & `cyvcf2-0.9.0/htslib/cram/cram_io.h`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/cram/cram_decode.c` & `cyvcf2-0.9.0/htslib/cram/cram_decode.c`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/cram/cram_samtools.c` & `cyvcf2-0.9.0/htslib/cram/cram_samtools.c`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/cram/cram_samtools.h` & `cyvcf2-0.9.0/htslib/cram/cram_samtools.h`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/cram/vlen.h` & `cyvcf2-0.9.0/htslib/cram/vlen.h`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/cram/cram_stats.h` & `cyvcf2-0.9.0/htslib/cram/cram_stats.h`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/cram/string_alloc.c` & `cyvcf2-0.9.0/htslib/cram/string_alloc.c`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/cram/zfio.c` & `cyvcf2-0.9.0/htslib/cram/zfio.c`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/cram/thread_pool.c` & `cyvcf2-0.9.0/htslib/cram/thread_pool.c`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/cram/os.h` & `cyvcf2-0.9.0/htslib/cram/os.h`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/cram/vlen.c` & `cyvcf2-0.9.0/htslib/cram/vlen.c`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/hfile.c` & `cyvcf2-0.9.0/htslib/hfile.c`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/faidx.c` & `cyvcf2-0.9.0/htslib/faidx.c`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/hfile_internal.h` & `cyvcf2-0.9.0/htslib/hfile_internal.h`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/kstring.c` & `cyvcf2-0.9.0/htslib/kstring.c`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/htsfile.c` & `cyvcf2-0.9.0/htslib/htsfile.c`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/md5.c` & `cyvcf2-0.9.0/htslib/md5.c`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/bgzip.c` & `cyvcf2-0.9.0/htslib/bgzip.c`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/htslib/regidx.c` & `cyvcf2-0.9.0/htslib/regidx.c`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/LICENSE` & `cyvcf2-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/README.md` & `cyvcf2-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/PKG-INFO` & `cyvcf2-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: cyvcf2
-Version: 0.8.9
+Version: 0.9.0
 Summary: fast vcf parsing with cython + htslib
 Home-page: https://github.com/brentp/cyvcf2/
 Author: Brent Pedersen
 Author-email: bpederse@gmail.com
 License: MIT
 Description: cyvcf2
         ======
```

### Comparing `cyvcf2-0.8.9/cyvcf2/cyvcf2.c` & `cyvcf2-0.9.0/cyvcf2/cyvcf2.c`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/cyvcf2/tests/test-alt-repr-1.vcf` & `cyvcf2-0.9.0/cyvcf2/tests/test-alt-repr-1.vcf`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/cyvcf2/tests/seg.vcf.gz` & `cyvcf2-0.9.0/cyvcf2/tests/seg.vcf.gz`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/cyvcf2/tests/test_reader.pyc` & `cyvcf2-0.9.0/cyvcf2/tests/test_reader.pyc`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/cyvcf2/tests/test.comp_het.3.vcf` & `cyvcf2-0.9.0/cyvcf2/tests/test.comp_het.3.vcf`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/cyvcf2/tests/test-hemi.vcf` & `cyvcf2-0.9.0/cyvcf2/tests/test-hemi.vcf`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/cyvcf2/tests/test.vcf.gz` & `cyvcf2-0.9.0/cyvcf2/tests/test.vcf.gz`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/cyvcf2/tests/bug.vcf.gz` & `cyvcf2-0.9.0/cyvcf2/tests/bug.vcf.gz`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/cyvcf2/tests/test-issue-48.vcf.gz` & `cyvcf2-0.9.0/cyvcf2/tests/test-issue-48.vcf.gz`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/cyvcf2/tests/test-haploidX.vcf` & `cyvcf2-0.9.0/cyvcf2/tests/test-haploidX.vcf`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/cyvcf2/tests/issue_44.vcf` & `cyvcf2-0.9.0/cyvcf2/tests/issue_44.vcf`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/cyvcf2/tests/o.vcf.gz` & `cyvcf2-0.9.0/cyvcf2/tests/o.vcf.gz`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/cyvcf2/tests/test-format-string.vcf` & `cyvcf2-0.9.0/cyvcf2/tests/test-format-string.vcf`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/cyvcf2/tests/test_gt_bases.vcf.gz` & `cyvcf2-0.9.0/cyvcf2/tests/test_gt_bases.vcf.gz`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/cyvcf2/tests/test.t.vcf` & `cyvcf2-0.9.0/cyvcf2/tests/test.t.vcf`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/cyvcf2/tests/test_hemi.pyc` & `cyvcf2-0.9.0/cyvcf2/tests/test_hemi.pyc`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/cyvcf2/tests/test.snpeff.bcf` & `cyvcf2-0.9.0/cyvcf2/tests/test.snpeff.bcf`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/cyvcf2/tests/test.snpeff.vcf` & `cyvcf2-0.9.0/cyvcf2/tests/test.snpeff.vcf`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/cyvcf2/tests/test_hemi.py` & `cyvcf2-0.9.0/cyvcf2/tests/test_hemi.py`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/cyvcf2/tests/test_gt_alt_freqs.vcf` & `cyvcf2-0.9.0/cyvcf2/tests/test_gt_alt_freqs.vcf`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/cyvcf2/tests/test_reader.py` & `cyvcf2-0.9.0/cyvcf2/tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/cyvcf2/tests/test-alt-repr.vcf` & `cyvcf2-0.9.0/cyvcf2/tests/test-alt-repr.vcf`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/cyvcf2/cyvcf2.pyx` & `cyvcf2-0.9.0/cyvcf2/cyvcf2.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -622,21 +622,23 @@
 
         seqnames = set(self.seqnames)
 
         if sites is not None:
             if isinstance(sites, basestring):
                 isites = []
                 for i in (x.strip().split(":") for x in open(sites)):
-                    # handle 'chr' prefix on incoming.
                     if not i[0] in seqnames and 'chr' + i[0] in seqnames:
                         i[0] = 'chr' + i[0]
                     i[1] = int(i[1])
                     isites.append(i)
             else:
                 isites = sites
+                for i in isites:
+                    if not i[0] in seqnames and 'chr' + i[0] in seqnames:
+                        i[0] = 'chr' + i[0]
 
         cdef Variant v
         cdef int k, last_pos
         if sites:
             isites = isites[offset::each]
             def gen():
                 ref, alt = None, None
```

### Comparing `cyvcf2-0.8.9/cyvcf2/relatedness.h` & `cyvcf2-0.9.0/cyvcf2/relatedness.h`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/cyvcf2/helpers.c` & `cyvcf2-0.9.0/cyvcf2/helpers.c`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/cyvcf2/cli.py` & `cyvcf2-0.9.0/cyvcf2/cli.py`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/cyvcf2/cyvcf2.pxd` & `cyvcf2-0.9.0/cyvcf2/cyvcf2.pxd`

 * *Files identical despite different names*

### Comparing `cyvcf2-0.8.9/setup.py` & `cyvcf2-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     to_install = list(specifiers)
     if to_install:
         cmd = [sys.executable, "-m", "pip", "install",
             "-t", "setup-requires"] + to_install
         subprocess.call(cmd)
 
 
-requires = ['cython', 'numpy']
+requires = ['cython', 'numpy', 'coloredlogs', 'click']
 install_requirements(missing_requirements(requires))
 
 
 excludes = ['irods', 'plugin']
 
 sources = [x for x in glob.glob('htslib/*.c') if not any(e in x for e in excludes)] + glob.glob('htslib/cram/*.c')
 # these have main()'s
```

### Comparing `cyvcf2-0.8.9/cyvcf2.egg-info/PKG-INFO` & `cyvcf2-0.9.0/cyvcf2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: cyvcf2
-Version: 0.8.9
+Version: 0.9.0
 Summary: fast vcf parsing with cython + htslib
 Home-page: https://github.com/brentp/cyvcf2/
 Author: Brent Pedersen
 Author-email: bpederse@gmail.com
 License: MIT
 Description: cyvcf2
         ======
```

### Comparing `cyvcf2-0.8.9/cyvcf2.egg-info/SOURCES.txt` & `cyvcf2-0.9.0/cyvcf2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

