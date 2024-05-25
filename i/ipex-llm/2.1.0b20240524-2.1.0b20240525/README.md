# Comparing `tmp/ipex_llm-2.1.0b20240524-py3-none-win_amd64.whl.zip` & `tmp/ipex_llm-2.1.0b20240525-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 5387647 bytes, number of entries: 202
+Zip file size: 5387679 bytes, number of entries: 202
 -rw-------  2.0 unx     1898 b- defN 24-Mar-25 11:36 ipex_llm/__init__.py
 -rw-------  2.0 unx     6816 b- defN 24-Mar-25 11:36 ipex_llm/convert_model.py
 -rw-------  2.0 unx     3232 b- defN 24-May-07 15:07 ipex_llm/llm_patching.py
 -rw-------  2.0 unx     1177 b- defN 24-Mar-25 11:36 ipex_llm/models.py
 -rw-------  2.0 unx    12466 b- defN 24-May-24 15:08 ipex_llm/optimize.py
 -rw-------  2.0 unx     2769 b- defN 24-Mar-25 11:36 ipex_llm/cli/llm-chat.ps1
 -rwx------  2.0 unx     3009 b- defN 24-Mar-25 11:36 ipex_llm/cli/llm-cli.ps1
@@ -40,47 +40,47 @@
 -rw-------  2.0 unx     7225 b- defN 24-Mar-25 11:36 ipex_llm/langchain/embeddings/transformersembeddings.py
 -rw-------  2.0 unx     1636 b- defN 24-Mar-25 11:36 ipex_llm/langchain/llms/__init__.py
 -rw-------  2.0 unx    24438 b- defN 24-Mar-25 11:36 ipex_llm/langchain/llms/bigdlllm.py
 -rw-------  2.0 unx    10576 b- defN 24-Apr-03 15:07 ipex_llm/langchain/llms/transformersllm.py
 -rw-------  2.0 unx     7379 b- defN 24-Mar-25 11:36 ipex_llm/langchain/llms/transformerspipelinellm.py
 -rw-------  2.0 unx      874 b- defN 24-May-24 15:08 ipex_llm/langchain/vllm/__init__.py
 -rw-------  2.0 unx     7793 b- defN 24-May-24 15:08 ipex_llm/langchain/vllm/vllm.py
--rw-------  2.0 unx        0 b- defN 24-May-24 15:08 ipex_llm/libs/__init__.py
--rw-------  2.0 unx    36352 b- defN 24-May-24 15:08 ipex_llm/libs/bloom-api.dll
--rw-------  2.0 unx   473088 b- defN 24-May-24 15:08 ipex_llm/libs/bloom.dll
--rw-------  2.0 unx   854016 b- defN 24-May-24 15:08 ipex_llm/libs/chatglm_C.cp310-win_amd64.pyd
--rw-------  2.0 unx   856576 b- defN 24-May-24 15:08 ipex_llm/libs/chatglm_C.cp311-win_amd64.pyd
--rw-------  2.0 unx   844288 b- defN 24-May-24 15:08 ipex_llm/libs/chatglm_C.cp39-win_amd64.pyd
--rw-------  2.0 unx    24576 b- defN 24-May-24 15:08 ipex_llm/libs/gptneox-api.dll
--rw-------  2.0 unx   532992 b- defN 24-May-24 15:08 ipex_llm/libs/gptneox.dll
--rw-------  2.0 unx   499712 b- defN 24-May-24 15:08 ipex_llm/libs/libbloom_avx.dll
--rw-------  2.0 unx   473600 b- defN 24-May-24 15:08 ipex_llm/libs/libbloom_vnni.dll
--rw-------  2.0 unx   559104 b- defN 24-May-24 15:08 ipex_llm/libs/libgptneox_avx.dll
--rw-------  2.0 unx   533504 b- defN 24-May-24 15:08 ipex_llm/libs/libgptneox_vnni.dll
--rw-------  2.0 unx   553472 b- defN 24-May-24 15:08 ipex_llm/libs/libllama_avx.dll
--rw-------  2.0 unx   527872 b- defN 24-May-24 15:08 ipex_llm/libs/libllama_vnni.dll
--rw-------  2.0 unx   590848 b- defN 24-May-24 15:08 ipex_llm/libs/libstarcoder_avx.dll
--rw-------  2.0 unx   564736 b- defN 24-May-24 15:08 ipex_llm/libs/libstarcoder_vnni.dll
--rw-------  2.0 unx    25088 b- defN 24-May-24 15:08 ipex_llm/libs/llama-api.dll
--rw-------  2.0 unx   526848 b- defN 24-May-24 15:08 ipex_llm/libs/llama.dll
--rw-------  2.0 unx   103424 b- defN 24-May-24 15:08 ipex_llm/libs/main-bloom.exe
--rw-------  2.0 unx   726016 b- defN 24-May-24 15:08 ipex_llm/libs/main-chatglm_vnni.exe
--rw-------  2.0 unx    98816 b- defN 24-May-24 15:08 ipex_llm/libs/main-gptneox.exe
--rw-------  2.0 unx    99840 b- defN 24-May-24 15:08 ipex_llm/libs/main-llama.exe
--rw-------  2.0 unx   157696 b- defN 24-May-24 15:08 ipex_llm/libs/main-starcoder.exe
--rw-------  2.0 unx   126464 b- defN 24-May-24 15:08 ipex_llm/libs/quantize-bloom.exe
--rw-------  2.0 unx   127488 b- defN 24-May-24 15:08 ipex_llm/libs/quantize-bloom_vnni.exe
--rw-------  2.0 unx   103936 b- defN 24-May-24 15:08 ipex_llm/libs/quantize-gptneox.exe
--rw-------  2.0 unx   104448 b- defN 24-May-24 15:08 ipex_llm/libs/quantize-gptneox_vnni.exe
--rw-------  2.0 unx   109056 b- defN 24-May-24 15:08 ipex_llm/libs/quantize-llama.exe
--rw-------  2.0 unx   110080 b- defN 24-May-24 15:08 ipex_llm/libs/quantize-llama_vnni.exe
--rw-------  2.0 unx   126976 b- defN 24-May-24 15:08 ipex_llm/libs/quantize-starcoder.exe
--rw-------  2.0 unx   128512 b- defN 24-May-24 15:08 ipex_llm/libs/quantize-starcoder_vnni.exe
--rw-------  2.0 unx    21504 b- defN 24-May-24 15:08 ipex_llm/libs/starcoder-api.dll
--rw-------  2.0 unx   564224 b- defN 24-May-24 15:08 ipex_llm/libs/starcoder.dll
+-rw-------  2.0 unx        0 b- defN 24-May-25 15:06 ipex_llm/libs/__init__.py
+-rw-------  2.0 unx    36352 b- defN 24-May-25 15:06 ipex_llm/libs/bloom-api.dll
+-rw-------  2.0 unx   473088 b- defN 24-May-25 15:06 ipex_llm/libs/bloom.dll
+-rw-------  2.0 unx   854016 b- defN 24-May-25 15:06 ipex_llm/libs/chatglm_C.cp310-win_amd64.pyd
+-rw-------  2.0 unx   856576 b- defN 24-May-25 15:06 ipex_llm/libs/chatglm_C.cp311-win_amd64.pyd
+-rw-------  2.0 unx   844288 b- defN 24-May-25 15:06 ipex_llm/libs/chatglm_C.cp39-win_amd64.pyd
+-rw-------  2.0 unx    24576 b- defN 24-May-25 15:06 ipex_llm/libs/gptneox-api.dll
+-rw-------  2.0 unx   532992 b- defN 24-May-25 15:06 ipex_llm/libs/gptneox.dll
+-rw-------  2.0 unx   499712 b- defN 24-May-25 15:06 ipex_llm/libs/libbloom_avx.dll
+-rw-------  2.0 unx   473600 b- defN 24-May-25 15:06 ipex_llm/libs/libbloom_vnni.dll
+-rw-------  2.0 unx   559104 b- defN 24-May-25 15:06 ipex_llm/libs/libgptneox_avx.dll
+-rw-------  2.0 unx   533504 b- defN 24-May-25 15:06 ipex_llm/libs/libgptneox_vnni.dll
+-rw-------  2.0 unx   553472 b- defN 24-May-25 15:06 ipex_llm/libs/libllama_avx.dll
+-rw-------  2.0 unx   527872 b- defN 24-May-25 15:06 ipex_llm/libs/libllama_vnni.dll
+-rw-------  2.0 unx   590848 b- defN 24-May-25 15:06 ipex_llm/libs/libstarcoder_avx.dll
+-rw-------  2.0 unx   564736 b- defN 24-May-25 15:06 ipex_llm/libs/libstarcoder_vnni.dll
+-rw-------  2.0 unx    25088 b- defN 24-May-25 15:06 ipex_llm/libs/llama-api.dll
+-rw-------  2.0 unx   526848 b- defN 24-May-25 15:06 ipex_llm/libs/llama.dll
+-rw-------  2.0 unx   103424 b- defN 24-May-25 15:06 ipex_llm/libs/main-bloom.exe
+-rw-------  2.0 unx   726016 b- defN 24-May-25 15:06 ipex_llm/libs/main-chatglm_vnni.exe
+-rw-------  2.0 unx    98816 b- defN 24-May-25 15:06 ipex_llm/libs/main-gptneox.exe
+-rw-------  2.0 unx    99840 b- defN 24-May-25 15:06 ipex_llm/libs/main-llama.exe
+-rw-------  2.0 unx   157696 b- defN 24-May-25 15:06 ipex_llm/libs/main-starcoder.exe
+-rw-------  2.0 unx   126464 b- defN 24-May-25 15:06 ipex_llm/libs/quantize-bloom.exe
+-rw-------  2.0 unx   127488 b- defN 24-May-25 15:06 ipex_llm/libs/quantize-bloom_vnni.exe
+-rw-------  2.0 unx   103936 b- defN 24-May-25 15:06 ipex_llm/libs/quantize-gptneox.exe
+-rw-------  2.0 unx   104448 b- defN 24-May-25 15:06 ipex_llm/libs/quantize-gptneox_vnni.exe
+-rw-------  2.0 unx   109056 b- defN 24-May-25 15:06 ipex_llm/libs/quantize-llama.exe
+-rw-------  2.0 unx   110080 b- defN 24-May-25 15:06 ipex_llm/libs/quantize-llama_vnni.exe
+-rw-------  2.0 unx   126976 b- defN 24-May-25 15:06 ipex_llm/libs/quantize-starcoder.exe
+-rw-------  2.0 unx   128512 b- defN 24-May-25 15:06 ipex_llm/libs/quantize-starcoder_vnni.exe
+-rw-------  2.0 unx    21504 b- defN 24-May-25 15:06 ipex_llm/libs/starcoder-api.dll
+-rw-------  2.0 unx   564224 b- defN 24-May-25 15:06 ipex_llm/libs/starcoder.dll
 -rw-------  2.0 unx      874 b- defN 24-Mar-25 11:36 ipex_llm/llamaindex/__init__.py
 -rw-------  2.0 unx     1139 b- defN 24-Apr-07 15:05 ipex_llm/llamaindex/llms/__init__.py
 -rw-------  2.0 unx    26314 b- defN 24-Apr-07 15:05 ipex_llm/llamaindex/llms/bigdlllm.py
 -rw-------  2.0 unx      586 b- defN 24-Mar-25 11:36 ipex_llm/serving/__init__.py
 -rw-------  2.0 unx      586 b- defN 24-Mar-25 11:36 ipex_llm/serving/fastchat/__init__.py
 -rw-------  2.0 unx    10084 b- defN 24-Mar-25 11:36 ipex_llm/serving/fastchat/bigdl_llm_model.py
 -rw-------  2.0 unx    19605 b- defN 24-May-20 15:06 ipex_llm/serving/fastchat/ipex_llm_worker.py
@@ -189,16 +189,16 @@
 -rw-------  2.0 unx     6944 b- defN 24-May-24 15:08 ipex_llm/vllm/cpu/entrypoints/openai/api_server.py
 -rw-------  2.0 unx      585 b- defN 24-May-24 15:08 ipex_llm/vllm/xpu/__init__.py
 -rw-------  2.0 unx    18506 b- defN 24-May-24 15:08 ipex_llm/vllm/xpu/ipex_llm_gpu_executor.py
 -rw-------  2.0 unx     7172 b- defN 24-May-24 15:08 ipex_llm/vllm/xpu/model_convert.py
 -rw-------  2.0 unx      747 b- defN 24-May-24 15:08 ipex_llm/vllm/xpu/engine/__init__.py
 -rw-------  2.0 unx     5953 b- defN 24-May-24 15:08 ipex_llm/vllm/xpu/engine/engine.py
 -rw-------  2.0 unx    10568 b- defN 24-May-24 15:08 ipex_llm/vllm/xpu/entrypoints/openai/api_server.py
--rwxr-xr-x  2.0 unx     2578 b- defN 24-May-24 15:08 ipex_llm-2.1.0b20240524.data/scripts/ipex-llm-init.bat
--rwxr-xr-x  2.0 unx     2769 b- defN 24-Mar-25 11:36 ipex_llm-2.1.0b20240524.data/scripts/llm-chat.ps1
--rwxr-xr-x  2.0 unx     3009 b- defN 24-Mar-25 11:36 ipex_llm-2.1.0b20240524.data/scripts/llm-cli.ps1
--rw-------  2.0 unx     5341 b- defN 24-May-24 15:09 ipex_llm-2.1.0b20240524.dist-info/METADATA
--rw-------  2.0 unx       98 b- defN 24-May-24 15:09 ipex_llm-2.1.0b20240524.dist-info/WHEEL
--rw-------  2.0 unx       61 b- defN 24-May-24 15:09 ipex_llm-2.1.0b20240524.dist-info/entry_points.txt
--rw-------  2.0 unx        9 b- defN 24-May-24 15:09 ipex_llm-2.1.0b20240524.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    19166 b- defN 24-May-24 15:09 ipex_llm-2.1.0b20240524.dist-info/RECORD
-202 files, 13353780 bytes uncompressed, 5357017 bytes compressed:  59.9%
+-rwxr-xr-x  2.0 unx     2578 b- defN 24-May-24 15:08 ipex_llm-2.1.0b20240525.data/scripts/ipex-llm-init.bat
+-rwxr-xr-x  2.0 unx     2769 b- defN 24-Mar-25 11:36 ipex_llm-2.1.0b20240525.data/scripts/llm-chat.ps1
+-rwxr-xr-x  2.0 unx     3009 b- defN 24-Mar-25 11:36 ipex_llm-2.1.0b20240525.data/scripts/llm-cli.ps1
+-rw-------  2.0 unx     5341 b- defN 24-May-25 15:06 ipex_llm-2.1.0b20240525.dist-info/METADATA
+-rw-------  2.0 unx       98 b- defN 24-May-25 15:06 ipex_llm-2.1.0b20240525.dist-info/WHEEL
+-rw-------  2.0 unx       61 b- defN 24-May-25 15:06 ipex_llm-2.1.0b20240525.dist-info/entry_points.txt
+-rw-------  2.0 unx        9 b- defN 24-May-25 15:06 ipex_llm-2.1.0b20240525.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    19166 b- defN 24-May-25 15:06 ipex_llm-2.1.0b20240525.dist-info/RECORD
+202 files, 13353780 bytes uncompressed, 5357049 bytes compressed:  59.9%
```

## zipnote {}

```diff
@@ -576,32 +576,32 @@
 
 Filename: ipex_llm/vllm/xpu/engine/engine.py
 Comment: 
 
 Filename: ipex_llm/vllm/xpu/entrypoints/openai/api_server.py
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240524.data/scripts/ipex-llm-init.bat
+Filename: ipex_llm-2.1.0b20240525.data/scripts/ipex-llm-init.bat
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240524.data/scripts/llm-chat.ps1
+Filename: ipex_llm-2.1.0b20240525.data/scripts/llm-chat.ps1
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240524.data/scripts/llm-cli.ps1
+Filename: ipex_llm-2.1.0b20240525.data/scripts/llm-cli.ps1
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240524.dist-info/METADATA
+Filename: ipex_llm-2.1.0b20240525.dist-info/METADATA
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240524.dist-info/WHEEL
+Filename: ipex_llm-2.1.0b20240525.dist-info/WHEEL
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240524.dist-info/entry_points.txt
+Filename: ipex_llm-2.1.0b20240525.dist-info/entry_points.txt
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240524.dist-info/top_level.txt
+Filename: ipex_llm-2.1.0b20240525.dist-info/top_level.txt
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240524.dist-info/RECORD
+Filename: ipex_llm-2.1.0b20240525.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ipex_llm/libs/bloom-api.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800036cc
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Fri May 24 15:02:53 2024
+Time/Date		Sat May 25 15:02:43 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000003200
 SizeOfInitializedData	0000000000005e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000036cc
@@ -6375,17 +6375,20 @@
    180005621:	push   %rdx
    180005622:	add    %al,0x1(%rax)
    180005628:	pop    %rax
    180005629:	push   %rdx
    18000562a:	add    %al,0x1(%rax)
    180005630:	add    %al,(%rax)
    180005632:	add    %al,(%rax)
-   180005634:	sbb    $0x6650ac,%eax
-   180005639:	add    %al,(%rax)
-   18000563b:	add    %cl,-0x20000000(%rip)        # 0x160005641
+   180005634:	xchg   %eax,%ebx
+   180005635:	std
+   180005636:	push   %rcx
+   180005637:	data16 add %al,(%rax)
+   18000563a:	add    %al,(%rax)
+   18000563c:	or     $0xe0000000,%eax
    180005641:	add    (%rax),%al
    180005643:	add    %cl,(%rcx,%rbx,2)
    180005646:	add    %al,(%rax)
    180005648:	or     $0x3f,%al
 	...
    18000567e:	add    %al,(%rax)
    180005680:	add    %eax,(%rax)
```

## ipex_llm/libs/bloom.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180055a08
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Fri May 24 15:02:53 2024
+Time/Date		Sat May 25 15:02:44 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000056000
 SizeOfInitializedData	00000000000bf400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000055a08
@@ -106743,32 +106743,30 @@
    18005aeb9:	jae    0x18005aee8
    18005aebb:	jb     0x18005af32
    18005aebd:	outsb  %ds:(%rsi),(%dx)
    18005aebe:	outsb  %ds:(%rsi),(%dx)
    18005aebf:	gs jb  0x18005af1e
    18005aec2:	(bad)
    18005aec7:	sub    $0x6c697562,%eax
-   18005aecc:	fs pop %rsp
-   18005aece:	pop    %rdi
-   18005aecf:	ja     0x18005af40
-   18005aed1:	jb     0x18005af3e
-   18005aed3:	pop    %rsp
-   18005aed4:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   18005aedb:	insl   (%dx),%es:(%rdi)
-   18005aedc:	pop    %rsp
-   18005aedd:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   18005aee4:	insl   (%dx),%es:(%rdi)
-   18005aee5:	pop    %rsp
-   18005aee6:	jae    0x18005af5a
-   18005aee8:	movsxd 0x67(%rdi,%riz,2),%ebx
-   18005aeec:	insl   (%dx),%es:(%rdi)
-   18005aeed:	insb   (%dx),%es:(%rdi)
-   18005aeee:	cs movsxd (%rax),%eax
-   18005aef1:	add    %al,(%rax)
-   18005aef3:	add    %al,(%rax)
+   18005aecc:	fs sub $0x5c77656e,%eax
+   18005aed2:	pop    %rdi
+   18005aed3:	ja     0x18005af44
+   18005aed5:	jb     0x18005af42
+   18005aed7:	pop    %rsp
+   18005aed8:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   18005aedf:	insl   (%dx),%es:(%rdi)
+   18005aee0:	pop    %rsp
+   18005aee1:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   18005aee8:	insl   (%dx),%es:(%rdi)
+   18005aee9:	pop    %rsp
+   18005aeea:	jae    0x18005af5e
+   18005aeec:	movsxd 0x67(%rdi,%riz,2),%ebx
+   18005aef0:	insl   (%dx),%es:(%rdi)
+   18005aef1:	insb   (%dx),%es:(%rdi)
+   18005aef2:	cs movsxd (%rax),%eax
    18005aef5:	add    %al,(%rax)
    18005aef7:	add    %al,0x47(%rdi)
    18005aefa:	rex.WRB
    18005aefb:	rex.WR pop %rdi
    18005aefd:	push   %r11
    18005aeff:	push   %rbx
    18005af00:	rex.RB push %r10
@@ -112379,17 +112377,17 @@
    18005e85d:	add    %al,(%rax)
    18005e85f:	add    %dh,0x76(%rax)
    18005e862:	add    $0x180,%eax
    18005e867:	add    %bh,0x76(%rax)
    18005e86a:	add    $0x180,%eax
    18005e86f:	add    %al,(%rax)
    18005e871:	add    %al,(%rax)
-   18005e873:	add    %bl,0x6650ac(%rip)        # 0x1806c3925
-   18005e879:	add    %al,(%rax)
-   18005e87b:	add    %cl,0x50000000(%rip)        # 0x1d005e881
+   18005e873:	add    %dl,0x6651(%rbp,%rdi,8)
+   18005e87a:	add    %al,(%rax)
+   18005e87c:	or     $0x50000000,%eax
    18005e881:	add    (%rax),%eax
    18005e883:	add    %ah,-0x5ffffa0e(%rax)
    18005e889:	out    %al,$0x5
 	...
    18005e8ff:	add    %dl,(%rax)
    18005e901:	testb  $0x0,0x180(%rip)        # 0x18005ea88
    18005e908:	sbb    %dh,%dh
```

## ipex_llm/libs/gptneox-api.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180002cbc
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Fri May 24 15:02:53 2024
+Time/Date		Sat May 25 15:02:43 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000002600
 SizeOfInitializedData	0000000000003e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000002cbc
@@ -5058,17 +5058,20 @@
    1800049c0:	cmp    %al,0x0(%rdx)
    1800049c3:	addb   $0x0,(%rcx)
    1800049c6:	add    %al,(%rax)
    1800049c8:	rex
    1800049c9:	rex.X add %al,0x1(%rax)
    1800049d0:	add    %al,(%rax)
    1800049d2:	add    %al,(%rax)
-   1800049d4:	sbb    $0x6650ac,%eax
-   1800049d9:	add    %al,(%rax)
-   1800049db:	add    %cl,-0x20000000(%rip)        # 0x1600049e1
+   1800049d4:	xchg   %eax,%ebx
+   1800049d5:	std
+   1800049d6:	push   %rcx
+   1800049d7:	data16 add %al,(%rax)
+   1800049da:	add    %al,(%rax)
+   1800049dc:	or     $0xe0000000,%eax
    1800049e1:	add    (%rax),%al
    1800049e3:	add    %ah,0x0(%rsp,%rcx,2)
    1800049e7:	add    %ah,0x0(%rsi,%rsi,1)
 	...
    1800049ff:	add    %al,(%rcx)
 	...
    180004a09:	add    %al,(%rax)
```

## ipex_llm/libs/gptneox.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005d168
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Fri May 24 15:02:54 2024
+Time/Date		Sat May 25 15:02:45 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005da00
 SizeOfInitializedData	00000000000c6600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005d168
@@ -24983,15 +24983,15 @@
    180007cf0:	xor    %rsp,%rax
    180007cf3:	mov    %rax,0x50(%rsp)
    180007cf8:	mov    %r9,%rbp
    180007cfb:	mov    %r8,%rsi
    180007cfe:	mov    %rdx,%rbx
    180007d01:	mov    %rcx,%rdi
    180007d04:	mov    %rcx,0x28(%rsp)
-   180007d09:	lea    0x57fa0(%rip),%r8        # 0x18005fcb0
+   180007d09:	lea    0x57fa4(%rip),%r8        # 0x18005fcb4
    180007d10:	call   0x180007b70
    180007d15:	nop
    180007d16:	movl   $0xc470,0x14(%rdi)
    180007d1d:	movl   $0x1000,0x18(%rdi)
    180007d24:	movl   $0x1400,0x1c(%rdi)
    180007d2b:	movl   $0x28,0x20(%rdi)
    180007d32:	movl   $0x24,0x24(%rdi)
@@ -41854,15 +41854,15 @@
    180017743:	sub    $0x80,%rsp
    18001774a:	mov    0x67d37(%rip),%rax        # 0x18007f488
    180017751:	xor    %rsp,%rax
    180017754:	mov    %rax,-0x8(%rbp)
    180017758:	mov    0x60(%rbp),%r13
    18001775c:	mov    %r8,%r12
    18001775f:	mov    %rcx,%rdi
-   180017762:	lea    0x48547(%rip),%r8        # 0x18005fcb0
+   180017762:	lea    0x4854b(%rip),%r8        # 0x18005fcb4
    180017769:	lea    -0x28(%rbp),%rcx
    18001776d:	mov    %r9,%r15
    180017770:	call   0x180007b70
    180017775:	call   *0x47dad(%rip)        # 0x18005f528
    18001777b:	mov    -0x28(%rbp),%rbx
    18001777f:	lea    -0x50(%rbp),%rcx
    180017783:	xor    %r14d,%r14d
@@ -113644,38 +113644,36 @@
    18005f7d9:	jae    0x18005f808
    18005f7db:	jb     0x18005f852
    18005f7dd:	outsb  %ds:(%rsi),(%dx)
    18005f7de:	outsb  %ds:(%rsi),(%dx)
    18005f7df:	gs jb  0x18005f83e
    18005f7e2:	(bad)
    18005f7e7:	sub    $0x6c697562,%eax
-   18005f7ec:	fs pop %rsp
-   18005f7ee:	pop    %rdi
-   18005f7ef:	ja     0x18005f860
-   18005f7f1:	jb     0x18005f85e
-   18005f7f3:	pop    %rsp
-   18005f7f4:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   18005f7fb:	insl   (%dx),%es:(%rdi)
-   18005f7fc:	pop    %rsp
-   18005f7fd:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   18005f804:	insl   (%dx),%es:(%rdi)
-   18005f805:	pop    %rsp
-   18005f806:	jae    0x18005f87a
-   18005f808:	movsxd 0x70(%rdi,%riz,2),%ebx
-   18005f80c:	je     0x18005f87c
-   18005f80e:	outsl  %gs:(%rsi),(%dx)
-   18005f810:	js     0x18005f86e
-   18005f812:	addr32 jo 0x18005f889
-   18005f815:	outsb  %ds:(%rsi),(%dx)
-   18005f816:	outsl  %gs:(%rsi),(%dx)
-   18005f818:	js     0x18005f847
-   18005f81a:	jne    0x18005f890
-   18005f81c:	imul   $0x0,0x68(%rsi,%rbp,1),%ebp
-   18005f824:	add    %al,(%rax)
-   18005f826:	add    %al,(%rax)
+   18005f7ec:	fs sub $0x5c77656e,%eax
+   18005f7f2:	pop    %rdi
+   18005f7f3:	ja     0x18005f864
+   18005f7f5:	jb     0x18005f862
+   18005f7f7:	pop    %rsp
+   18005f7f8:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   18005f7ff:	insl   (%dx),%es:(%rdi)
+   18005f800:	pop    %rsp
+   18005f801:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   18005f808:	insl   (%dx),%es:(%rdi)
+   18005f809:	pop    %rsp
+   18005f80a:	jae    0x18005f87e
+   18005f80c:	movsxd 0x70(%rdi,%riz,2),%ebx
+   18005f810:	je     0x18005f880
+   18005f812:	outsl  %gs:(%rsi),(%dx)
+   18005f814:	js     0x18005f872
+   18005f816:	addr32 jo 0x18005f88d
+   18005f819:	outsb  %ds:(%rsi),(%dx)
+   18005f81a:	outsl  %gs:(%rsi),(%dx)
+   18005f81c:	js     0x18005f84b
+   18005f81e:	jne    0x18005f894
+   18005f820:	imul   $0x0,0x68(%rsi,%rbp,1),%ebp
    18005f828:	rex.RXB push %r8
    18005f82a:	push   %rsp
    18005f82b:	rex.WRX
    18005f82c:	rex.RB
    18005f82d:	rex.WRXB pop %r8
    18005f82f:	pop    %rdi
    18005f830:	push   %r11
@@ -114038,39 +114036,37 @@
    18005fc69:	jae    0x18005fc98
    18005fc6b:	jb     0x18005fce2
    18005fc6d:	outsb  %ds:(%rsi),(%dx)
    18005fc6e:	outsb  %ds:(%rsi),(%dx)
    18005fc6f:	gs jb  0x18005fcce
    18005fc72:	(bad)
    18005fc77:	sub    $0x6c697562,%eax
-   18005fc7c:	fs pop %rsp
-   18005fc7e:	pop    %rdi
-   18005fc7f:	ja     0x18005fcf0
-   18005fc81:	jb     0x18005fcee
-   18005fc83:	pop    %rsp
-   18005fc84:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   18005fc8b:	insl   (%dx),%es:(%rdi)
-   18005fc8c:	pop    %rsp
-   18005fc8d:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   18005fc94:	insl   (%dx),%es:(%rdi)
-   18005fc95:	pop    %rsp
-   18005fc96:	jae    0x18005fd0a
-   18005fc98:	movsxd 0x70(%rdi,%riz,2),%ebx
-   18005fc9c:	je     0x18005fd0c
-   18005fc9e:	outsl  %gs:(%rsi),(%dx)
-   18005fca0:	js     0x18005fcfe
-   18005fca2:	addr32 jo 0x18005fd19
-   18005fca5:	outsb  %ds:(%rsi),(%dx)
-   18005fca6:	outsl  %gs:(%rsi),(%dx)
-   18005fca8:	js     0x18005fcd8
-   18005fcaa:	movsxd 0x70(%rax),%esi
-   18005fcad:	add    %al,(%rax)
-   18005fcaf:	add    %dh,0x62(%rdx)
-   18005fcb2:	add    %al,(%rax)
-   18005fcb4:	add    %al,(%rax)
+   18005fc7c:	fs sub $0x5c77656e,%eax
+   18005fc82:	pop    %rdi
+   18005fc83:	ja     0x18005fcf4
+   18005fc85:	jb     0x18005fcf2
+   18005fc87:	pop    %rsp
+   18005fc88:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   18005fc8f:	insl   (%dx),%es:(%rdi)
+   18005fc90:	pop    %rsp
+   18005fc91:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   18005fc98:	insl   (%dx),%es:(%rdi)
+   18005fc99:	pop    %rsp
+   18005fc9a:	jae    0x18005fd0e
+   18005fc9c:	movsxd 0x70(%rdi,%riz,2),%ebx
+   18005fca0:	je     0x18005fd10
+   18005fca2:	outsl  %gs:(%rsi),(%dx)
+   18005fca4:	js     0x18005fd02
+   18005fca6:	addr32 jo 0x18005fd1d
+   18005fca9:	outsb  %ds:(%rsi),(%dx)
+   18005fcaa:	outsl  %gs:(%rsi),(%dx)
+   18005fcac:	js     0x18005fcdc
+   18005fcae:	movsxd 0x70(%rax),%esi
+   18005fcb1:	add    %al,(%rax)
+   18005fcb3:	add    %dh,0x62(%rdx)
    18005fcb6:	add    %al,(%rax)
    18005fcb8:	(bad)
    18005fcbd:	sub    $0x3a6d6c6c,%eax
    18005fcc2:	and    %ch,0x61(%rdi,%rbp,2)
    18005fcc6:	imul   $0x646f6d20,%fs:0x67(%rsi),%ebp
    18005fcce:	gs insb (%dx),%es:(%rdi)
    18005fcd0:	and    %ah,0x72(%rsi)
@@ -120403,32 +120399,30 @@
    180063f99:	jae    0x180063fc8
    180063f9b:	jb     0x180064012
    180063f9d:	outsb  %ds:(%rsi),(%dx)
    180063f9e:	outsb  %ds:(%rsi),(%dx)
    180063f9f:	gs jb  0x180063ffe
    180063fa2:	(bad)
    180063fa7:	sub    $0x6c697562,%eax
-   180063fac:	fs pop %rsp
-   180063fae:	pop    %rdi
-   180063faf:	ja     0x180064020
-   180063fb1:	jb     0x18006401e
-   180063fb3:	pop    %rsp
-   180063fb4:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   180063fbb:	insl   (%dx),%es:(%rdi)
-   180063fbc:	pop    %rsp
-   180063fbd:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   180063fc4:	insl   (%dx),%es:(%rdi)
-   180063fc5:	pop    %rsp
-   180063fc6:	jae    0x18006403a
-   180063fc8:	movsxd 0x67(%rdi,%riz,2),%ebx
-   180063fcc:	insl   (%dx),%es:(%rdi)
-   180063fcd:	insb   (%dx),%es:(%rdi)
-   180063fce:	cs movsxd (%rax),%eax
-   180063fd1:	add    %al,(%rax)
-   180063fd3:	add    %al,(%rax)
+   180063fac:	fs sub $0x5c77656e,%eax
+   180063fb2:	pop    %rdi
+   180063fb3:	ja     0x180064024
+   180063fb5:	jb     0x180064022
+   180063fb7:	pop    %rsp
+   180063fb8:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   180063fbf:	insl   (%dx),%es:(%rdi)
+   180063fc0:	pop    %rsp
+   180063fc1:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   180063fc8:	insl   (%dx),%es:(%rdi)
+   180063fc9:	pop    %rsp
+   180063fca:	jae    0x18006403e
+   180063fcc:	movsxd 0x67(%rdi,%riz,2),%ebx
+   180063fd0:	insl   (%dx),%es:(%rdi)
+   180063fd1:	insb   (%dx),%es:(%rdi)
+   180063fd2:	cs movsxd (%rax),%eax
    180063fd5:	add    %al,(%rax)
    180063fd7:	add    %al,0x47(%rdi)
    180063fda:	rex.WRB
    180063fdb:	rex.WR pop %rdi
    180063fdd:	push   %r11
    180063fdf:	push   %rbx
    180063fe0:	rex.RB push %r10
@@ -123727,17 +123721,17 @@
    18006611d:	add    %al,(%rax)
    18006611f:	add    %bh,0x18005f6(%rax)
    180066125:	add    %al,(%rax)
    180066127:	add    %al,%al
    180066129:	testb  $0x0,0x180(%rip)        # 0x1800662b0
    180066130:	add    %al,(%rax)
    180066132:	add    %al,(%rax)
-   180066134:	(bad)
-   180066135:	lods   %ds:(%rsi),%al
-   180066136:	push   %rax
+   180066134:	xchg   %eax,%ebp
+   180066135:	std
+   180066136:	push   %rcx
    180066137:	data16 add %al,(%rax)
    18006613a:	add    %al,(%rax)
    18006613c:	or     $0x50000000,%eax
    180066141:	add    (%rax),%eax
    180066143:	add    %al,0x5b840006(%rbp,%rbp,2)
    18006614a:	(bad)
 	...
```

## ipex_llm/libs/libbloom_avx.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005bb88
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Fri May 24 15:03:06 2024
+Time/Date		Sat May 25 15:04:19 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005c200
 SizeOfInitializedData	00000000000bfa00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005bb88
@@ -117886,17 +117886,17 @@
    18006578d:	add    %al,(%rax)
    18006578f:	add    %dh,-0x1a(%rax)
    180065792:	add    $0x180,%eax
    180065797:	add    %bh,-0x1a(%rax)
    18006579a:	add    $0x180,%eax
    18006579f:	add    %al,(%rax)
    1800657a1:	add    %al,(%rax)
-   1800657a3:	add    %ch,(%rdx)
-   1800657a5:	lods   %ds:(%rsi),%al
-   1800657a6:	push   %rax
+   1800657a3:	add    %dh,%bl
+   1800657a5:	std
+   1800657a6:	push   %rcx
    1800657a7:	data16 add %al,(%rax)
    1800657aa:	add    %al,(%rax)
    1800657ac:	or     $0x50000000,%eax
    1800657b1:	add    (%rax),%eax
    1800657b3:	add    %ah,-0x5ffff99f(%rax)
    1800657b9:	rex.RXB (bad)
 	...
```

## ipex_llm/libs/libbloom_vnni.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180055c18
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Fri May 24 15:03:59 2024
+Time/Date		Sat May 25 15:02:34 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000056200
 SizeOfInitializedData	00000000000bf400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000055c18
@@ -112474,19 +112474,17 @@
    18005f83a:	add    $0x180,%eax
    18005f83f:	add    %dh,-0x7a(%rax)
    18005f842:	add    $0x180,%eax
    18005f847:	add    %bh,-0x7a(%rax)
    18005f84a:	add    $0x180,%eax
    18005f84f:	add    %al,(%rax)
    18005f851:	add    %al,(%rax)
-   18005f853:	add    %bl,-0x54(%rdi)
-   18005f856:	push   %rax
-   18005f857:	data16 add %al,(%rax)
-   18005f85a:	add    %al,(%rax)
-   18005f85c:	or     $0x50000000,%eax
+   18005f853:	add    %cl,0x6651fd(%rdx)
+   18005f859:	add    %al,(%rax)
+   18005f85b:	add    %cl,0x50000000(%rip)        # 0x1d005f861
    18005f861:	add    (%rax),%eax
    18005f863:	add    %ah,(%rax)
    18005f865:	add    (%rsi),%al
    18005f867:	add    %ah,(%rax)
    18005f869:	call   0x18005f873
 	...
    18005f87e:	add    %al,(%rax)
```

## ipex_llm/libs/libgptneox_avx.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180063378
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Fri May 24 15:03:07 2024
+Time/Date		Sat May 25 15:04:20 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000063c00
 SizeOfInitializedData	00000000000c6a00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000063378
@@ -129351,16 +129351,20 @@
    18006c057:	add    %al,%al
    18006c059:	push   %rsi
    18006c05a:	(bad)
    18006c05b:	addb   $0x0,(%rcx)
    18006c05e:	add    %al,(%rax)
    18006c060:	add    %al,(%rax)
    18006c062:	add    %al,(%rax)
-   18006c064:	sub    0x66(%rax,%rdx,2),%ebp
-   18006c06b:	add    %cl,0x50000000(%rip)        # 0x1d006c071
+   18006c064:	hlt
+   18006c065:	std
+   18006c066:	push   %rcx
+   18006c067:	data16 add %al,(%rax)
+   18006c06a:	add    %al,(%rax)
+   18006c06c:	or     $0x50000000,%eax
    18006c071:	add    (%rax),%eax
    18006c073:	add    %al,-0x437bfffa(%rsp,%rcx,8)
    18006c07a:	(bad)
    18006c07b:	add    %al,(%rax)
    18006c07d:	add    %al,(%rax)
    18006c07f:	add    %bh,%al
    18006c081:	iret
```

## ipex_llm/libs/libgptneox_vnni.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005d378
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Fri May 24 15:03:59 2024
+Time/Date		Sat May 25 15:02:35 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005dc00
 SizeOfInitializedData	00000000000c6600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005d378
@@ -123910,17 +123910,16 @@
    1800660fd:	add    %al,(%rax)
    1800660ff:	add    %bh,0x18005f6(%rax)
    180066105:	add    %al,(%rax)
    180066107:	add    %al,%al
    180066109:	testb  $0x0,0x180(%rip)        # 0x180066290
    180066110:	add    %al,(%rax)
    180066112:	add    %al,(%rax)
-   180066114:	pop    %rdi
-   180066115:	lods   %ds:(%rsi),%al
-   180066116:	push   %rax
+   180066114:	mov    %ebp,%edi
+   180066116:	push   %rcx
    180066117:	data16 add %al,(%rax)
    18006611a:	add    %al,(%rax)
    18006611c:	or     $0x50000000,%eax
    180066121:	add    (%rax),%eax
    180066123:	add    %al,0x5d840006(%rbp,%rbp,2)
    18006612a:	(bad)
 	...
```

## ipex_llm/libs/libllama_avx.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180062088
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Fri May 24 15:03:07 2024
+Time/Date		Sat May 25 15:04:20 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000062800
 SizeOfInitializedData	00000000000c6800
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000062088
@@ -128098,16 +128098,20 @@
    18006b134:	add    %eax,(%rax)
    18006b136:	add    %al,(%rax)
    18006b138:	rolb   $1,0x6(%rsi)
    18006b13b:	addb   $0x0,(%rcx)
    18006b13e:	add    %al,(%rax)
    18006b140:	add    %al,(%rax)
    18006b142:	add    %al,(%rax)
-   18006b144:	sub    0x66(%rax,%rdx,2),%ebp
-   18006b14b:	add    %cl,0x50000000(%rip)        # 0x1d006b151
+   18006b144:	hlt
+   18006b145:	std
+   18006b146:	push   %rcx
+   18006b147:	data16 add %al,(%rax)
+   18006b14a:	add    %al,(%rax)
+   18006b14c:	or     $0x50000000,%eax
    18006b151:	add    (%rax),%eax
    18006b153:	add    %al,-0x7ffff943(%rax)
    18006b159:	test   $0x6,%eax
 	...
    18006b17e:	add    %al,(%rax)
    18006b180:	lock rolb $0x80,(%rsi)
    18006b184:	add    %eax,(%rax)
```

## ipex_llm/libs/libllama_vnni.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005c088
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Fri May 24 15:03:59 2024
+Time/Date		Sat May 25 15:02:35 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005c800
 SizeOfInitializedData	00000000000c6400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005c088
@@ -122606,19 +122606,17 @@
    1800651e0:	enter  $0x5e6,$0x80
    1800651e4:	add    %eax,(%rax)
    1800651e6:	add    %al,(%rax)
    1800651e8:	shl    $1,%dh
    1800651ea:	add    $0x180,%eax
    1800651ef:	add    %al,(%rax)
    1800651f1:	add    %al,(%rax)
-   1800651f3:	add    %bl,-0x54(%rdi)
-   1800651f6:	push   %rax
-   1800651f7:	data16 add %al,(%rax)
-   1800651fa:	add    %al,(%rax)
-   1800651fc:	or     $0x50000000,%eax
+   1800651f3:	add    %cl,0x6651fd(%rbx)
+   1800651f9:	add    %al,(%rax)
+   1800651fb:	add    %cl,0x50000000(%rip)        # 0x1d0065201
    180065201:	add    (%rax),%eax
    180065203:	add    %al,-0x7ffff9a2(%rax)
    180065209:	rex.WX (bad)
 	...
    18006527f:	add    %dh,%al
    180065281:	(bad)
    180065282:	(bad)
```

## ipex_llm/libs/libstarcoder_avx.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800694e8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Fri May 24 15:03:06 2024
+Time/Date		Sat May 25 15:04:19 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000069c00
 SizeOfInitializedData	00000000000c8600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000694e8
@@ -138532,16 +138532,19 @@
    180072c85:	add    %al,(%rax)
    180072c87:	add    %al,%al
    180072c89:	mov    $0x6,%dh
    180072c8b:	addb   $0x0,(%rcx)
    180072c8e:	add    %al,(%rax)
    180072c90:	add    %al,(%rax)
    180072c92:	add    %al,(%rax)
-   180072c94:	sub    0x66(%rax,%rdx,2),%ch
-   180072c9b:	add    %cl,0x50000000(%rip)        # 0x1d0072ca1
+   180072c94:	repz std
+   180072c96:	push   %rcx
+   180072c97:	data16 add %al,(%rax)
+   180072c9a:	add    %al,(%rax)
+   180072c9c:	or     $0x50000000,%eax
    180072ca1:	add    (%rax),%eax
    180072ca3:	add    %dl,0x3e(%rax)
    180072ca6:	(bad)
    180072ca7:	add    %dl,0x2e(%rax)
    180072caa:	(bad)
 	...
    180072cff:	add    %al,%al
```

## ipex_llm/libs/libstarcoder_vnni.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180063578
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Fri May 24 15:03:59 2024
+Time/Date		Sat May 25 15:02:34 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000063c00
 SizeOfInitializedData	00000000000c8000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000063578
@@ -133201,17 +133201,16 @@
    18006cd57:	add    %al,%al
    18006cd59:	push   %rsi
    18006cd5a:	(bad)
    18006cd5b:	addb   $0x0,(%rcx)
    18006cd5e:	add    %al,(%rax)
    18006cd60:	add    %al,(%rax)
    18006cd62:	add    %al,(%rax)
-   18006cd64:	pop    %rdi
-   18006cd65:	lods   %ds:(%rsi),%al
-   18006cd66:	push   %rax
+   18006cd64:	mov    %ch,%bh
+   18006cd66:	push   %rcx
    18006cd67:	data16 add %al,(%rax)
    18006cd6a:	add    %al,(%rax)
    18006cd6c:	or     $0x50000000,%eax
    18006cd71:	add    (%rax),%eax
    18006cd73:	add    %dl,%al
    18006cd75:	fiadds (%rsi)
    18006cd77:	add    %dl,%al
```

## ipex_llm/libs/llama-api.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180002dac
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Fri May 24 15:02:53 2024
+Time/Date		Sat May 25 15:02:43 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000002800
 SizeOfInitializedData	0000000000003e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000002dac
@@ -5355,17 +5355,20 @@
    180004a20:	cmp    %al,0x0(%rdx)
    180004a23:	addb   $0x0,(%rcx)
    180004a26:	add    %al,(%rax)
    180004a28:	rex
    180004a29:	rex.X add %al,0x1(%rax)
    180004a30:	add    %al,(%rax)
    180004a32:	add    %al,(%rax)
-   180004a34:	sbb    $0x6650ac,%eax
-   180004a39:	add    %al,(%rax)
-   180004a3b:	add    %cl,-0x20000000(%rip)        # 0x160004a41
+   180004a34:	xchg   %eax,%ebx
+   180004a35:	std
+   180004a36:	push   %rcx
+   180004a37:	data16 add %al,(%rax)
+   180004a3a:	add    %al,(%rax)
+   180004a3c:	or     $0xe0000000,%eax
    180004a41:	add    (%rax),%al
    180004a43:	add    %ah,%ah
    180004a45:	rex.WR add %r8b,(%rax)
    180004a48:	in     $0x38,%al
 	...
    180004a7e:	add    %al,(%rax)
    180004a80:	add    %eax,(%rax)
```

## ipex_llm/libs/llama.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005be78
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Fri May 24 15:02:54 2024
+Time/Date		Sat May 25 15:02:45 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005c600
 SizeOfInitializedData	00000000000c6200
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005be78
@@ -24654,52 +24654,52 @@
    18000795d:	mov    %rax,%rcx
    180007960:	call   *0x56cd2(%rip)        # 0x18005e638
    180007966:	test   %eax,%eax
    180007968:	je     0x1800079a4
    18000796a:	mov    $0x2,%ecx
    18000796f:	call   *0x56c9b(%rip)        # 0x18005e610
    180007975:	mov    %rax,%rcx
-   180007978:	lea    0x56f39(%rip),%rax        # 0x18005e8b8
+   180007978:	lea    0x56f41(%rip),%rax        # 0x18005e8c0
    18000797f:	mov    %rax,0x20(%rsp)
    180007984:	mov    $0x65,%r9d
    18000798a:	lea    0x56e7f(%rip),%r8        # 0x18005e810
-   180007991:	lea    0x56ec8(%rip),%rdx        # 0x18005e860
+   180007991:	lea    0x56ed0(%rip),%rdx        # 0x18005e868
    180007998:	call   0x1800157c0
    18000799d:	call   *0x56bb5(%rip)        # 0x18005e558
    1800079a3:	int3
    1800079a4:	mov    (%rbx),%rcx
    1800079a7:	call   *0x56c83(%rip)        # 0x18005e630
    1800079ad:	cmp    $0xffffffffffffffff,%rax
    1800079b1:	jne    0x1800079eb
    1800079b3:	lea    0x3(%rax),%ecx
    1800079b6:	call   *0x56c54(%rip)        # 0x18005e610
    1800079bc:	mov    %rax,%rcx
-   1800079bf:	lea    0x56ee2(%rip),%rax        # 0x18005e8a8
+   1800079bf:	lea    0x56eea(%rip),%rax        # 0x18005e8b0
    1800079c6:	mov    %rax,0x20(%rsp)
    1800079cb:	mov    $0x5b,%r9d
    1800079d1:	lea    0x56e38(%rip),%r8        # 0x18005e810
-   1800079d8:	lea    0x56e81(%rip),%rdx        # 0x18005e860
+   1800079d8:	lea    0x56e89(%rip),%rdx        # 0x18005e868
    1800079df:	call   0x1800157c0
    1800079e4:	call   *0x56b6e(%rip)        # 0x18005e558
    1800079ea:	int3
    1800079eb:	mov    %rax,0x8(%rbx)
    1800079ef:	xor    %r8d,%r8d
    1800079f2:	xor    %edx,%edx
    1800079f4:	mov    (%rbx),%rcx
    1800079f7:	call   *0x56c3b(%rip)        # 0x18005e638
    1800079fd:	test   %eax,%eax
    1800079ff:	je     0x180007a3b
    180007a01:	mov    $0x2,%ecx
    180007a06:	call   *0x56c04(%rip)        # 0x18005e610
    180007a0c:	mov    %rax,%rcx
-   180007a0f:	lea    0x56ea2(%rip),%rax        # 0x18005e8b8
+   180007a0f:	lea    0x56eaa(%rip),%rax        # 0x18005e8c0
    180007a16:	mov    %rax,0x20(%rsp)
    180007a1b:	mov    $0x65,%r9d
    180007a21:	lea    0x56de8(%rip),%r8        # 0x18005e810
-   180007a28:	lea    0x56e31(%rip),%rdx        # 0x18005e860
+   180007a28:	lea    0x56e39(%rip),%rdx        # 0x18005e868
    180007a2f:	call   0x1800157c0
    180007a34:	call   *0x56b1e(%rip)        # 0x18005e558
    180007a3a:	int3
    180007a3b:	mov    %rbx,%rax
    180007a3e:	mov    0x68(%rsp),%rcx
    180007a43:	xor    %rsp,%rcx
    180007a46:	call   0x18005b870
@@ -24708,15 +24708,15 @@
    180007a57:	pop    %rdi
    180007a58:	ret
    180007a59:	call   *0x56ad9(%rip)        # 0x18005e538
    180007a5f:	mov    (%rax),%ecx
    180007a61:	call   *0x56ae9(%rip)        # 0x18005e550
    180007a67:	mov    %rax,%r9
    180007a6a:	mov    %rdi,%r8
-   180007a6d:	lea    0x56e1c(%rip),%rdx        # 0x18005e890
+   180007a6d:	lea    0x56e24(%rip),%rdx        # 0x18005e898
    180007a74:	lea    0x48(%rsp),%rcx
    180007a79:	call   0x18000c070
    180007a7e:	nop
    180007a7f:	mov    %rax,%rdx
    180007a82:	lea    0x30(%rsp),%rcx
    180007a87:	call   0x1800086c0
    180007a8c:	lea    0x6493d(%rip),%rdx        # 0x18006c3d0
@@ -24734,15 +24734,15 @@
    180007ab0:	xor    %rsp,%rax
    180007ab3:	mov    %rax,0x50(%rsp)
    180007ab8:	mov    %r9,%rbp
    180007abb:	mov    %r8,%rsi
    180007abe:	mov    %rdx,%rbx
    180007ac1:	mov    %rcx,%rdi
    180007ac4:	mov    %rcx,0x28(%rsp)
-   180007ac9:	lea    0x571fc(%rip),%r8        # 0x18005eccc
+   180007ac9:	lea    0x57200(%rip),%r8        # 0x18005ecd0
    180007ad0:	call   0x180007920
    180007ad5:	nop
    180007ad6:	movl   $0x7d00,0x14(%rdi)
    180007add:	movl   $0x200,0x18(%rdi)
    180007ae4:	movl   $0x1000,0x1c(%rdi)
    180007aeb:	movl   $0x100,0x20(%rdi)
    180007af2:	movl   $0x20,0x24(%rdi)
@@ -24753,15 +24753,15 @@
    180007b15:	lea    0x38(%rdi),%rcx
    180007b19:	call   0x1800085f0
    180007b1e:	nop
    180007b1f:	mov    $0x2,%ecx
    180007b24:	call   *0x56ae6(%rip)        # 0x18005e610
    180007b2a:	mov    %rax,%rcx
    180007b2d:	mov    %rbx,%r8
-   180007b30:	lea    0x57199(%rip),%rdx        # 0x18005ecd0
+   180007b30:	lea    0x571a1(%rip),%rdx        # 0x18005ecd8
    180007b37:	call   0x1800157c0
    180007b3c:	mov    $0x4,%r8d
    180007b42:	lea    0x20(%rsp),%rdx
    180007b47:	mov    %rdi,%rcx
    180007b4a:	call   0x180012f40
    180007b4f:	mov    0x20(%rsp),%ebx
    180007b53:	cmp    $0x67676d6c,%ebx
@@ -24935,15 +24935,15 @@
    180007df2:	cmpq   $0x10,0x18(%rax)
    180007df7:	jb     0x180007dfc
    180007df9:	mov    (%rax),%rbx
    180007dfc:	mov    $0x2,%ecx
    180007e01:	call   *0x56809(%rip)        # 0x18005e610
    180007e07:	mov    %rax,%rcx
    180007e0a:	mov    %rbx,%r8
-   180007e0d:	lea    0x56b54(%rip),%rdx        # 0x18005e968
+   180007e0d:	lea    0x56b5c(%rip),%rdx        # 0x18005e970
    180007e14:	call   0x1800157c0
    180007e19:	mov    0x60(%rsp),%rdx
    180007e1e:	cmp    $0x10,%rdx
    180007e22:	jb     0x180007e59
    180007e24:	inc    %rdx
    180007e27:	mov    0x48(%rsp),%rcx
    180007e2c:	mov    %rcx,%rax
@@ -24971,15 +24971,15 @@
    180007e7f:	mov    %ebp,%edx
    180007e81:	lea    0x68(%rsp),%rcx
    180007e86:	call   0x18000ef50
    180007e8b:	nop
    180007e8c:	mov    %rax,%rcx
    180007e8f:	call   0x18000b930
    180007e94:	mov    %rax,%r8
-   180007e97:	lea    0x56aaa(%rip),%rdx        # 0x18005e948
+   180007e97:	lea    0x56ab2(%rip),%rdx        # 0x18005e950
    180007e9e:	lea    0x48(%rsp),%rcx
    180007ea3:	call   0x18000c070
    180007ea8:	nop
    180007ea9:	mov    %rax,%rdx
    180007eac:	lea    0x30(%rsp),%rcx
    180007eb1:	call   0x1800086c0
    180007eb6:	lea    0x64513(%rip),%rdx        # 0x18006c3d0
@@ -24989,15 +24989,15 @@
    180007ec8:	mov    %eax,%edx
    180007eca:	lea    0x48(%rsp),%rcx
    180007ecf:	call   0x18000ef50
    180007ed4:	nop
    180007ed5:	mov    %rax,%rcx
    180007ed8:	call   0x18000b930
    180007edd:	mov    %rax,%r8
-   180007ee0:	lea    0x56a41(%rip),%rdx        # 0x18005e928
+   180007ee0:	lea    0x56a49(%rip),%rdx        # 0x18005e930
    180007ee7:	lea    0x68(%rsp),%rcx
    180007eec:	call   0x18000c070
    180007ef1:	nop
    180007ef2:	mov    %rax,%rdx
    180007ef5:	lea    0x30(%rsp),%rcx
    180007efa:	call   0x1800086c0
    180007eff:	lea    0x644ca(%rip),%rdx        # 0x18006c3d0
@@ -27186,15 +27186,15 @@
    180009ae7:	cmpq   $0x10,0x18(%rax)
    180009aec:	jb     0x180009af1
    180009aee:	mov    (%rax),%rbx
    180009af1:	mov    $0x2,%ecx
    180009af6:	call   *0x54b14(%rip)        # 0x18005e610
    180009afc:	mov    %rax,%rcx
    180009aff:	mov    %rbx,%r8
-   180009b02:	lea    0x54e8f(%rip),%rdx        # 0x18005e998
+   180009b02:	lea    0x54e97(%rip),%rdx        # 0x18005e9a0
    180009b09:	call   0x1800157c0
    180009b0e:	mov    0x38(%rsp),%rdx
    180009b13:	cmp    $0x10,%rdx
    180009b17:	jb     0x180009b4f
    180009b19:	inc    %rdx
    180009b1c:	mov    0x20(%rsp),%rcx
    180009b21:	mov    %rcx,%rax
@@ -29477,15 +29477,15 @@
    18000ba26:	mov    $0x2,%ecx
    18000ba2b:	call   *0x52bdf(%rip)        # 0x18005e610
    18000ba31:	mov    %rax,%rcx
    18000ba34:	lea    0x5321d(%rip),%rax        # 0x18005ec58
    18000ba3b:	mov    %rax,0x20(%rsp)
    18000ba40:	mov    $0x187,%r9d
    18000ba46:	lea    0x53233(%rip),%r8        # 0x18005ec80
-   18000ba4d:	lea    0x52e0c(%rip),%rdx        # 0x18005e860
+   18000ba4d:	lea    0x52e14(%rip),%rdx        # 0x18005e868
    18000ba54:	call   0x1800157c0
    18000ba59:	call   *0x52af9(%rip)        # 0x18005e558
    18000ba5f:	int3
    18000ba60:	mov    0x3c(%r14),%ecx
    18000ba64:	test   %ecx,%ecx
    18000ba66:	je     0x18000bac5
    18000ba68:	sub    $0x1,%ecx
@@ -30098,19 +30098,19 @@
    18000c184:	mov    %r14,%rcx
    18000c187:	call   0x1800199e0
    18000c18c:	cmp    %r15d,%eax
    18000c18f:	je     0x18000c1cb
    18000c191:	mov    $0x2,%ecx
    18000c196:	call   *0x52474(%rip)        # 0x18005e610
    18000c19c:	mov    %rax,%rcx
-   18000c19f:	lea    0x526da(%rip),%rax        # 0x18005e880
+   18000c19f:	lea    0x526e2(%rip),%rax        # 0x18005e888
    18000c1a6:	mov    %rax,0x20(%rsp)
    18000c1ab:	mov    $0x40,%r9d
    18000c1b1:	lea    0x52658(%rip),%r8        # 0x18005e810
-   18000c1b8:	lea    0x526a1(%rip),%rdx        # 0x18005e860
+   18000c1b8:	lea    0x526a9(%rip),%rdx        # 0x18005e868
    18000c1bf:	call   0x1800157c0
    18000c1c4:	call   *0x5238e(%rip)        # 0x18005e558
    18000c1ca:	int3
    18000c1cb:	vpxor  %xmm0,%xmm0,%xmm0
    18000c1cf:	vmovups %xmm0,0x0(%rbp)
    18000c1d4:	mov    %r12,0x10(%rbp)
    18000c1d8:	mov    %r12,0x18(%rbp)
@@ -30150,15 +30150,15 @@
    18000c23a:	mov    $0x2,%ecx
    18000c23f:	call   *0x523cb(%rip)        # 0x18005e610
    18000c245:	mov    %rax,%rcx
    18000c248:	lea    0x52599(%rip),%rax        # 0x18005e7e8
    18000c24f:	mov    %rax,0x20(%rsp)
    18000c254:	mov    $0x3d,%r9d
    18000c25a:	lea    0x525af(%rip),%r8        # 0x18005e810
-   18000c261:	lea    0x525f8(%rip),%rdx        # 0x18005e860
+   18000c261:	lea    0x52600(%rip),%rdx        # 0x18005e868
    18000c268:	call   0x1800157c0
    18000c26d:	call   *0x522e5(%rip)        # 0x18005e558
    18000c273:	int3
    18000c274:	call   0x18000b150
    18000c279:	int3
    18000c27a:	call   0x18000b5a0
    18000c27f:	int3
@@ -30248,15 +30248,15 @@
    18000c3c0:	mov    $0x2,%ecx
    18000c3c5:	call   *0x52245(%rip)        # 0x18005e610
    18000c3cb:	mov    %rax,%rcx
    18000c3ce:	lea    0x52be3(%rip),%rax        # 0x18005efb8
    18000c3d5:	mov    %rax,0x20(%rsp)
    18000c3da:	mov    $0x2b2,%r9d
    18000c3e0:	lea    0x52899(%rip),%r8        # 0x18005ec80
-   18000c3e7:	lea    0x52472(%rip),%rdx        # 0x18005e860
+   18000c3e7:	lea    0x5247a(%rip),%rdx        # 0x18005e868
    18000c3ee:	call   0x1800157c0
    18000c3f3:	call   *0x5215f(%rip)        # 0x18005e558
    18000c3f9:	int3
    18000c3fa:	mov    (%r14),%r8d
    18000c3fd:	mov    0x38(%rdi),%edx
    18000c400:	mov    0x80(%rbx),%rcx
    18000c407:	call   0x18003b2c0
@@ -30272,15 +30272,15 @@
    18000c42c:	mov    $0x2,%ecx
    18000c431:	call   *0x521d9(%rip)        # 0x18005e610
    18000c437:	mov    %rax,%rcx
    18000c43a:	lea    0x52b8f(%rip),%rax        # 0x18005efd0
    18000c441:	mov    %rax,0x20(%rsp)
    18000c446:	mov    $0x2b6,%r9d
    18000c44c:	lea    0x5282d(%rip),%r8        # 0x18005ec80
-   18000c453:	lea    0x52406(%rip),%rdx        # 0x18005e860
+   18000c453:	lea    0x5240e(%rip),%rdx        # 0x18005e868
    18000c45a:	call   0x1800157c0
    18000c45f:	call   *0x520f3(%rip)        # 0x18005e558
    18000c465:	int3
    18000c466:	mov    %r13d,0x4(%rsi)
    18000c46a:	mov    %rsi,0x60(%rdi)
    18000c46e:	incq   0x78(%rbx)
    18000c472:	mov    %rsi,%rax
@@ -30354,16 +30354,16 @@
    18000c561:	mov    %rcx,%rbx
    18000c564:	jne    0x18000c5a0
    18000c566:	mov    $0x2,%ecx
    18000c56b:	call   *0x5209f(%rip)        # 0x18005e610
    18000c571:	mov    $0x114,%r9d
    18000c577:	lea    0x52292(%rip),%r8        # 0x18005e810
    18000c57e:	mov    %rax,%rcx
-   18000c581:	lea    0x522d8(%rip),%rdx        # 0x18005e860
-   18000c588:	lea    0x5244d(%rip),%rax        # 0x18005e9dc
+   18000c581:	lea    0x522e0(%rip),%rdx        # 0x18005e868
+   18000c588:	lea    0x52455(%rip),%rax        # 0x18005e9e4
    18000c58f:	mov    %rax,0x20(%rsp)
    18000c594:	call   0x1800157c0
    18000c599:	call   *0x51fb9(%rip)        # 0x18005e558
    18000c59f:	int3
    18000c5a0:	cmpb   $0x0,0x10(%rcx)
    18000c5a4:	jne    0x18000c5f8
    18000c5a6:	lea    0x30(%rsp),%rcx
@@ -30579,16 +30579,16 @@
    18000c894:	add    $0x38,%rsp
    18000c898:	ret
    18000c899:	mov    $0x2,%ecx
    18000c89e:	call   *0x51d6c(%rip)        # 0x18005e610
    18000c8a4:	mov    $0x10f,%r9d
    18000c8aa:	lea    0x51f5f(%rip),%r8        # 0x18005e810
    18000c8b1:	mov    %rax,%rcx
-   18000c8b4:	lea    0x51fa5(%rip),%rdx        # 0x18005e860
-   18000c8bb:	lea    0x520fe(%rip),%rax        # 0x18005e9c0
+   18000c8b4:	lea    0x51fad(%rip),%rdx        # 0x18005e868
+   18000c8bb:	lea    0x52106(%rip),%rax        # 0x18005e9c8
    18000c8c2:	mov    %rax,0x20(%rsp)
    18000c8c7:	call   0x1800157c0
    18000c8cc:	call   *0x51c86(%rip)        # 0x18005e558
    18000c8d2:	int3
    18000c8d3:	int3
    18000c8d4:	int3
    18000c8d5:	int3
@@ -32089,15 +32089,15 @@
    18000e2e0:	mov    %rax,-0x30(%rbp)
    18000e2e4:	jne    0x18000e320
    18000e2e6:	mov    $0x2,%ecx
    18000e2eb:	call   *0x5031f(%rip)        # 0x18005e610
    18000e2f1:	mov    $0x4e8,%r9d
    18000e2f7:	lea    0x50982(%rip),%r8        # 0x18005ec80
    18000e2fe:	mov    %rax,%rcx
-   18000e301:	lea    0x50558(%rip),%rdx        # 0x18005e860
+   18000e301:	lea    0x50560(%rip),%rdx        # 0x18005e868
    18000e308:	lea    0x512f1(%rip),%rax        # 0x18005f600
    18000e30f:	mov    %rax,0x20(%rsp)
    18000e314:	call   0x1800157c0
    18000e319:	call   *0x50239(%rip)        # 0x18005e558
    18000e31f:	int3
    18000e320:	mov    0x13e0(%r14),%ecx
    18000e327:	mov    0x13e4(%r14),%eax
@@ -32845,19 +32845,19 @@
    18000efb1:	mov    %rdi,0x10(%rbx)
    18000efb5:	mov    %rbx,%rcx
    18000efb8:	movq   $0xf,0x18(%rbx)
    18000efc0:	call   0x18000b600
    18000efc5:	mov    %rax,(%rbx)
    18000efc8:	movq   $0x15,0x10(%rbx)
    18000efd0:	movq   $0x1f,0x18(%rbx)
-   18000efd8:	vmovups 0x4f930(%rip),%xmm0        # 0x18005e910
+   18000efd8:	vmovups 0x4f938(%rip),%xmm0        # 0x18005e918
    18000efe0:	vmovups %xmm0,(%rax)
-   18000efe4:	mov    0x4f936(%rip),%ecx        # 0x18005e920
+   18000efe4:	mov    0x4f93e(%rip),%ecx        # 0x18005e928
    18000efea:	mov    %ecx,0x10(%rax)
-   18000efed:	movzbl 0x4f930(%rip),%ecx        # 0x18005e924
+   18000efed:	movzbl 0x4f938(%rip),%ecx        # 0x18005e92c
    18000eff4:	mov    %cl,0x14(%rax)
    18000eff7:	mov    %dil,0x15(%rax)
    18000effb:	jmp    0x18000f031
    18000effd:	mov    0x40(%rsp),%rdx
    18000f002:	lea    0x50(%rsp),%rcx
    18000f007:	vpxor  %xmm1,%xmm1,%xmm1
    18000f00b:	vmovdqu %xmm1,0x60(%rsp)
@@ -34552,15 +34552,15 @@
    180010bfe:	mov    $0x2,%ecx
    180010c03:	call   *0x4da07(%rip)        # 0x18005e610
    180010c09:	mov    %rax,%rcx
    180010c0c:	lea    0x4df61(%rip),%rax        # 0x18005eb74
    180010c13:	mov    %rax,0x20(%rsp)
    180010c18:	mov    $0x39e,%r9d
    180010c1e:	lea    0x4e05b(%rip),%r8        # 0x18005ec80
-   180010c25:	lea    0x4dc34(%rip),%rdx        # 0x18005e860
+   180010c25:	lea    0x4dc3c(%rip),%rdx        # 0x18005e868
    180010c2c:	call   0x1800157c0
    180010c31:	call   *0x4d921(%rip)        # 0x18005e558
    180010c37:	int3
    180010c38:	lea    0x4f491(%rip),%rcx        # 0x1800600d0
    180010c3f:	call   0x18005b018
    180010c44:	int3
    180010c45:	lea    0x4e794(%rip),%rdx        # 0x18005f3e0
@@ -35429,48 +35429,48 @@
    180011a02:	mov    $0x2,%ecx
    180011a07:	call   *0x4cc03(%rip)        # 0x18005e610
    180011a0d:	mov    %rax,%rcx
    180011a10:	lea    0x4d429(%rip),%rax        # 0x18005ee40
    180011a17:	mov    %rax,0x20(%rsp)
    180011a1c:	mov    $0x25d,%r9d
    180011a22:	lea    0x4d257(%rip),%r8        # 0x18005ec80
-   180011a29:	lea    0x4ce30(%rip),%rdx        # 0x18005e860
+   180011a29:	lea    0x4ce38(%rip),%rdx        # 0x18005e868
    180011a30:	call   0x1800157c0
    180011a35:	call   *0x4cb1d(%rip)        # 0x18005e558
    180011a3b:	int3
    180011a3c:	mov    $0x2,%ecx
    180011a41:	call   *0x4cbc9(%rip)        # 0x18005e610
    180011a47:	mov    %rax,%rcx
-   180011a4a:	lea    0x4ce67(%rip),%rax        # 0x18005e8b8
+   180011a4a:	lea    0x4ce6f(%rip),%rax        # 0x18005e8c0
    180011a51:	mov    %rax,0x20(%rsp)
    180011a56:	mov    $0x65,%r9d
    180011a5c:	lea    0x4cdad(%rip),%r8        # 0x18005e810
-   180011a63:	lea    0x4cdf6(%rip),%rdx        # 0x18005e860
+   180011a63:	lea    0x4cdfe(%rip),%rdx        # 0x18005e868
    180011a6a:	call   0x1800157c0
    180011a6f:	call   *0x4cae3(%rip)        # 0x18005e558
    180011a75:	int3
    180011a76:	mov    $0x2,%ecx
    180011a7b:	call   *0x4cb8f(%rip)        # 0x18005e610
    180011a81:	mov    %rax,%rcx
-   180011a84:	lea    0x4ce1d(%rip),%rax        # 0x18005e8a8
+   180011a84:	lea    0x4ce25(%rip),%rax        # 0x18005e8b0
    180011a8b:	mov    %rax,0x20(%rsp)
    180011a90:	mov    $0x5b,%r9d
    180011a96:	lea    0x4cd73(%rip),%r8        # 0x18005e810
-   180011a9d:	lea    0x4cdbc(%rip),%rdx        # 0x18005e860
+   180011a9d:	lea    0x4cdc4(%rip),%rdx        # 0x18005e868
    180011aa4:	call   0x1800157c0
    180011aa9:	call   *0x4caa9(%rip)        # 0x18005e558
    180011aaf:	int3
    180011ab0:	mov    $0x2,%ecx
    180011ab5:	call   *0x4cb55(%rip)        # 0x18005e610
    180011abb:	mov    %rax,%rcx
    180011abe:	lea    0x4d0af(%rip),%rax        # 0x18005eb74
    180011ac5:	mov    %rax,0x20(%rsp)
    180011aca:	mov    $0x255,%r9d
    180011ad0:	lea    0x4d1a9(%rip),%r8        # 0x18005ec80
-   180011ad7:	lea    0x4cd82(%rip),%rdx        # 0x18005e860
+   180011ad7:	lea    0x4cd8a(%rip),%rdx        # 0x18005e868
    180011ade:	call   0x1800157c0
    180011ae3:	call   *0x4ca6f(%rip)        # 0x18005e558
    180011ae9:	nop
    180011aea:	mov    -0x50(%rbp),%rsi
    180011aee:	jmp    0x180011b09
    180011af0:	mov    0x100(%rbp),%rdi
    180011af7:	mov    0x40(%rsp),%rsi
@@ -35763,19 +35763,19 @@
    180011f4b:	test   %rsi,%rsi
    180011f4e:	js     0x180011f91
    180011f50:	vcvtsi2ss %rsi,%xmm1,%xmm1
    180011f55:	jmp    0x180011fa9
    180011f57:	mov    $0x2,%ecx
    180011f5c:	call   *0x4c6ae(%rip)        # 0x18005e610
    180011f62:	mov    %rax,%rcx
-   180011f65:	lea    0x4ca54(%rip),%rax        # 0x18005e9c0
+   180011f65:	lea    0x4ca5c(%rip),%rax        # 0x18005e9c8
    180011f6c:	mov    %rax,0x20(%rsp)
    180011f71:	mov    $0x10f,%r9d
    180011f77:	lea    0x4c892(%rip),%r8        # 0x18005e810
-   180011f7e:	lea    0x4c8db(%rip),%rdx        # 0x18005e860
+   180011f7e:	lea    0x4c8e3(%rip),%rdx        # 0x18005e868
    180011f85:	call   0x1800157c0
    180011f8a:	call   *0x4c5c8(%rip)        # 0x18005e558
    180011f90:	int3
    180011f91:	mov    %rsi,%rcx
    180011f94:	shr    $1,%rcx
    180011f97:	mov    %rsi,%rax
    180011f9a:	and    $0x1,%eax
@@ -35842,30 +35842,30 @@
    180012077:	cmp    %r13,%rbx
    18001207a:	je     0x180012101
    180012080:	mov    0xb0(%rsp),%r8
    180012088:	jmp    0x180011f30
    18001208d:	mov    $0x2,%ecx
    180012092:	call   *0x4c578(%rip)        # 0x18005e610
    180012098:	mov    %rax,%rcx
-   18001209b:	lea    0x4c93a(%rip),%rax        # 0x18005e9dc
+   18001209b:	lea    0x4c942(%rip),%rax        # 0x18005e9e4
    1800120a2:	mov    %rax,0x20(%rsp)
    1800120a7:	mov    $0x114,%r9d
    1800120ad:	lea    0x4c75c(%rip),%r8        # 0x18005e810
-   1800120b4:	lea    0x4c7a5(%rip),%rdx        # 0x18005e860
+   1800120b4:	lea    0x4c7ad(%rip),%rdx        # 0x18005e868
    1800120bb:	call   0x1800157c0
    1800120c0:	call   *0x4c492(%rip)        # 0x18005e558
    1800120c6:	int3
    1800120c7:	mov    $0x2,%ecx
    1800120cc:	call   *0x4c53e(%rip)        # 0x18005e610
    1800120d2:	mov    %rax,%rcx
    1800120d5:	lea    0x4cf44(%rip),%rax        # 0x18005f020
    1800120dc:	mov    %rax,0x20(%rsp)
    1800120e1:	mov    $0x2e1,%r9d
    1800120e7:	lea    0x4cb92(%rip),%r8        # 0x18005ec80
-   1800120ee:	lea    0x4c76b(%rip),%rdx        # 0x18005e860
+   1800120ee:	lea    0x4c773(%rip),%rdx        # 0x18005e868
    1800120f5:	call   0x1800157c0
    1800120fa:	call   *0x4c458(%rip)        # 0x18005e558
    180012100:	int3
    180012101:	mov    0xa8(%rsp),%rbx
    180012109:	add    $0x60,%rsp
    18001210d:	pop    %r15
    18001210f:	pop    %r14
@@ -35900,15 +35900,15 @@
    180012158:	mov    $0x2,%ecx
    18001215d:	call   *0x4c4ad(%rip)        # 0x18005e610
    180012163:	mov    %rax,%rcx
    180012166:	lea    0x4cec3(%rip),%rax        # 0x18005f030
    18001216d:	mov    %rax,0x20(%rsp)
    180012172:	mov    $0x2ee,%r9d
    180012178:	lea    0x4cb01(%rip),%r8        # 0x18005ec80
-   18001217f:	lea    0x4c6da(%rip),%rdx        # 0x18005e860
+   18001217f:	lea    0x4c6e2(%rip),%rdx        # 0x18005e868
    180012186:	call   0x1800157c0
    18001218b:	call   *0x4c3c7(%rip)        # 0x18005e558
    180012191:	int3
    180012192:	movabs $0x4924924924924925,%rax
    18001219c:	imul   %rcx
    18001219f:	sar    $0x4,%rdx
    1800121a3:	mov    %rdx,%rax
@@ -35946,19 +35946,19 @@
    180012226:	mov    (%rbx),%rcx
    180012229:	call   *0x4c409(%rip)        # 0x18005e638
    18001222f:	test   %eax,%eax
    180012231:	je     0x18001226d
    180012233:	mov    $0x2,%ecx
    180012238:	call   *0x4c3d2(%rip)        # 0x18005e610
    18001223e:	mov    %rax,%rcx
-   180012241:	lea    0x4c670(%rip),%rax        # 0x18005e8b8
+   180012241:	lea    0x4c678(%rip),%rax        # 0x18005e8c0
    180012248:	mov    %rax,0x20(%rsp)
    18001224d:	mov    $0x65,%r9d
    180012253:	lea    0x4c5b6(%rip),%r8        # 0x18005e810
-   18001225a:	lea    0x4c5ff(%rip),%rdx        # 0x18005e860
+   18001225a:	lea    0x4c607(%rip),%rdx        # 0x18005e868
    180012261:	call   0x1800157c0
    180012266:	call   *0x4c2ec(%rip)        # 0x18005e558
    18001226c:	int3
    18001226d:	mov    0x58(%r14),%r8
    180012271:	mov    0x68(%r14),%rdx
    180012275:	mov    %rbx,%rcx
    180012278:	call   0x180012f40
@@ -35999,26 +35999,26 @@
    1800122fd:	mov    $0x2,%ecx
    180012302:	call   *0x4c308(%rip)        # 0x18005e610
    180012308:	mov    %rax,%rcx
    18001230b:	lea    0x4cd36(%rip),%rax        # 0x18005f048
    180012312:	mov    %rax,0x20(%rsp)
    180012317:	mov    $0x2fc,%r9d
    18001231d:	lea    0x4c95c(%rip),%r8        # 0x18005ec80
-   180012324:	lea    0x4c535(%rip),%rdx        # 0x18005e860
+   180012324:	lea    0x4c53d(%rip),%rdx        # 0x18005e868
    18001232b:	call   0x1800157c0
    180012330:	call   *0x4c222(%rip)        # 0x18005e558
    180012336:	int3
    180012337:	mov    $0x2,%ecx
    18001233c:	call   *0x4c2ce(%rip)        # 0x18005e610
    180012342:	mov    %rax,%rcx
-   180012345:	lea    0x4c56c(%rip),%rax        # 0x18005e8b8
+   180012345:	lea    0x4c574(%rip),%rax        # 0x18005e8c0
    18001234c:	mov    %rax,0x20(%rsp)
    180012351:	mov    $0x65,%r9d
    180012357:	lea    0x4c4b2(%rip),%r8        # 0x18005e810
-   18001235e:	lea    0x4c4fb(%rip),%rdx        # 0x18005e860
+   18001235e:	lea    0x4c503(%rip),%rdx        # 0x18005e868
    180012365:	call   0x1800157c0
    18001236a:	call   *0x4c1e8(%rip)        # 0x18005e558
    180012370:	int3
    180012371:	cmp    $0x1,%eax
    180012374:	jne    0x18001272c
    18001237a:	mov    0x8(%rdx),%rcx
    18001237e:	sub    (%rdx),%rcx
@@ -36208,26 +36208,26 @@
    18001265a:	mov    $0x2,%ecx
    18001265f:	call   *0x4bfab(%rip)        # 0x18005e610
    180012665:	mov    %rax,%rcx
    180012668:	lea    0x4c9f1(%rip),%rax        # 0x18005f060
    18001266f:	mov    %rax,0x20(%rsp)
    180012674:	mov    $0x313,%r9d
    18001267a:	lea    0x4c5ff(%rip),%r8        # 0x18005ec80
-   180012681:	lea    0x4c1d8(%rip),%rdx        # 0x18005e860
+   180012681:	lea    0x4c1e0(%rip),%rdx        # 0x18005e868
    180012688:	call   0x1800157c0
    18001268d:	call   *0x4bec5(%rip)        # 0x18005e558
    180012693:	int3
    180012694:	mov    $0x2,%ecx
    180012699:	call   *0x4bf71(%rip)        # 0x18005e610
    18001269f:	mov    %rax,%rcx
-   1800126a2:	lea    0x4c20f(%rip),%rax        # 0x18005e8b8
+   1800126a2:	lea    0x4c217(%rip),%rax        # 0x18005e8c0
    1800126a9:	mov    %rax,0x20(%rsp)
    1800126ae:	mov    $0x65,%r9d
    1800126b4:	lea    0x4c155(%rip),%r8        # 0x18005e810
-   1800126bb:	lea    0x4c19e(%rip),%rdx        # 0x18005e860
+   1800126bb:	lea    0x4c1a6(%rip),%rdx        # 0x18005e868
    1800126c2:	call   0x1800157c0
    1800126c7:	call   *0x4be8b(%rip)        # 0x18005e558
    1800126cd:	nop
    1800126ce:	test   %r12,%r12
    1800126d1:	je     0x18001272c
    1800126d3:	mov    %r12,%rbx
    1800126d6:	cmp    %rsi,%r12
@@ -36886,30 +36886,30 @@
    180012fa0:	xor    %rsp,%rcx
    180012fa3:	call   0x18005b870
    180012fa8:	add    $0x60,%rsp
    180012fac:	pop    %rdi
    180012fad:	pop    %rsi
    180012fae:	pop    %rbx
    180012faf:	ret
-   180012fb0:	lea    0x4b921(%rip),%rdx        # 0x18005e8d8
+   180012fb0:	lea    0x4b929(%rip),%rdx        # 0x18005e8e0
    180012fb7:	lea    0x38(%rsp),%rcx
    180012fbc:	call   0x180007010
    180012fc1:	nop
    180012fc2:	mov    %rax,%rdx
    180012fc5:	lea    0x20(%rsp),%rcx
    180012fca:	call   0x1800086c0
    180012fcf:	lea    0x593fa(%rip),%rdx        # 0x18006c3d0
    180012fd6:	lea    0x20(%rsp),%rcx
    180012fdb:	call   0x18005c3e2
    180012fe0:	nop
    180012fe1:	call   *0x4b551(%rip)        # 0x18005e538
    180012fe7:	mov    (%rax),%ecx
    180012fe9:	call   *0x4b561(%rip)        # 0x18005e550
    180012fef:	mov    %rax,%r8
-   180012ff2:	lea    0x4b8cf(%rip),%rdx        # 0x18005e8c8
+   180012ff2:	lea    0x4b8d7(%rip),%rdx        # 0x18005e8d0
    180012ff9:	lea    0x38(%rsp),%rcx
    180012ffe:	call   0x18000c070
    180013003:	nop
    180013004:	mov    %rax,%rdx
    180013007:	lea    0x20(%rsp),%rcx
    18001300c:	call   0x1800086c0
    180013011:	lea    0x593b8(%rip),%rdx        # 0x18006c3d0
@@ -37517,69 +37517,69 @@
    180013962:	call   0x18005b254
    180013967:	mov    -0x48(%rbp),%r12
    18001396b:	mov    (%r12),%rcx
    18001396f:	jmp    0x180013070
    180013974:	mov    $0x2,%ecx
    180013979:	call   *0x4ac91(%rip)        # 0x18005e610
    18001397f:	mov    %rax,%rcx
-   180013982:	lea    0x4af2f(%rip),%rax        # 0x18005e8b8
+   180013982:	lea    0x4af37(%rip),%rax        # 0x18005e8c0
    180013989:	mov    %rax,0x20(%rsp)
    18001398e:	mov    $0x65,%r9d
    180013994:	lea    0x4ae75(%rip),%r8        # 0x18005e810
-   18001399b:	lea    0x4aebe(%rip),%rdx        # 0x18005e860
+   18001399b:	lea    0x4aec6(%rip),%rdx        # 0x18005e868
    1800139a2:	call   0x1800157c0
    1800139a7:	call   *0x4abab(%rip)        # 0x18005e558
    1800139ad:	int3
    1800139ae:	mov    $0x2,%ecx
    1800139b3:	call   *0x4ac57(%rip)        # 0x18005e610
    1800139b9:	mov    %rax,%rcx
-   1800139bc:	lea    0x4aee5(%rip),%rax        # 0x18005e8a8
+   1800139bc:	lea    0x4aeed(%rip),%rax        # 0x18005e8b0
    1800139c3:	mov    %rax,0x20(%rsp)
    1800139c8:	mov    $0x5b,%r9d
    1800139ce:	lea    0x4ae3b(%rip),%r8        # 0x18005e810
-   1800139d5:	lea    0x4ae84(%rip),%rdx        # 0x18005e860
+   1800139d5:	lea    0x4ae8c(%rip),%rdx        # 0x18005e868
    1800139dc:	call   0x1800157c0
    1800139e1:	call   *0x4ab71(%rip)        # 0x18005e558
    1800139e7:	nop
    1800139e8:	call   *0x4abb2(%rip)        # 0x18005e5a0
    1800139ee:	nop
    1800139ef:	call   *0x4abab(%rip)        # 0x18005e5a0
    1800139f5:	nop
    1800139f6:	call   *0x4aba4(%rip)        # 0x18005e5a0
    1800139fc:	nop
    1800139fd:	mov    $0x2,%ecx
    180013a02:	call   *0x4ac08(%rip)        # 0x18005e610
    180013a08:	mov    %rax,%rcx
-   180013a0b:	lea    0x4aea6(%rip),%rax        # 0x18005e8b8
+   180013a0b:	lea    0x4aeae(%rip),%rax        # 0x18005e8c0
    180013a12:	mov    %rax,0x20(%rsp)
    180013a17:	mov    $0x65,%r9d
    180013a1d:	lea    0x4adec(%rip),%r8        # 0x18005e810
-   180013a24:	lea    0x4ae35(%rip),%rdx        # 0x18005e860
+   180013a24:	lea    0x4ae3d(%rip),%rdx        # 0x18005e868
    180013a2b:	call   0x1800157c0
    180013a30:	call   *0x4ab22(%rip)        # 0x18005e558
    180013a36:	int3
    180013a37:	mov    $0x2,%ecx
    180013a3c:	call   *0x4abce(%rip)        # 0x18005e610
    180013a42:	mov    %rax,%rcx
-   180013a45:	lea    0x4ae5c(%rip),%rax        # 0x18005e8a8
+   180013a45:	lea    0x4ae64(%rip),%rax        # 0x18005e8b0
    180013a4c:	mov    %rax,0x20(%rsp)
    180013a51:	mov    $0x5b,%r9d
    180013a57:	lea    0x4adb2(%rip),%r8        # 0x18005e810
-   180013a5e:	lea    0x4adfb(%rip),%rdx        # 0x18005e860
+   180013a5e:	lea    0x4ae03(%rip),%rdx        # 0x18005e868
    180013a65:	call   0x1800157c0
    180013a6a:	call   *0x4aae8(%rip)        # 0x18005e558
    180013a70:	nop
    180013a71:	mov    $0x2,%ecx
    180013a76:	call   *0x4ab94(%rip)        # 0x18005e610
    180013a7c:	mov    %rax,%rcx
-   180013a7f:	lea    0x4ae22(%rip),%rax        # 0x18005e8a8
+   180013a7f:	lea    0x4ae2a(%rip),%rax        # 0x18005e8b0
    180013a86:	mov    %rax,0x20(%rsp)
    180013a8b:	mov    $0x5b,%r9d
    180013a91:	lea    0x4ad78(%rip),%r8        # 0x18005e810
-   180013a98:	lea    0x4adc1(%rip),%rdx        # 0x18005e860
+   180013a98:	lea    0x4adc9(%rip),%rdx        # 0x18005e868
    180013a9f:	call   0x1800157c0
    180013aa4:	call   *0x4aaae(%rip)        # 0x18005e558
    180013aaa:	int3
    180013aab:	mov    0x30(%rbp),%rcx
    180013aaf:	xor    %rsp,%rcx
    180013ab2:	call   0x18005b870
    180013ab7:	mov    0x198(%rsp),%rbx
@@ -37599,30 +37599,30 @@
    180013ae1:	lea    0x4b278(%rip),%rdx        # 0x18005ed60
    180013ae8:	lea    -0x10(%rbp),%rcx
    180013aec:	call   0x18000c070
    180013af1:	lea    0x58a08(%rip),%rdx        # 0x18006c500
    180013af8:	lea    -0x10(%rbp),%rcx
    180013afc:	call   0x18005c3e2
    180013b01:	nop
-   180013b02:	lea    0x4adcf(%rip),%rdx        # 0x18005e8d8
+   180013b02:	lea    0x4add7(%rip),%rdx        # 0x18005e8e0
    180013b09:	lea    0x10(%rbp),%rcx
    180013b0d:	call   0x180007010
    180013b12:	nop
    180013b13:	mov    %rax,%rdx
    180013b16:	lea    -0x10(%rbp),%rcx
    180013b1a:	call   0x1800086c0
    180013b1f:	lea    0x588aa(%rip),%rdx        # 0x18006c3d0
    180013b26:	lea    -0x10(%rbp),%rcx
    180013b2a:	call   0x18005c3e2
    180013b2f:	nop
    180013b30:	call   *0x4aa02(%rip)        # 0x18005e538
    180013b36:	mov    (%rax),%ecx
    180013b38:	call   *0x4aa12(%rip)        # 0x18005e550
    180013b3e:	mov    %rax,%r8
-   180013b41:	lea    0x4ad80(%rip),%rdx        # 0x18005e8c8
+   180013b41:	lea    0x4ad88(%rip),%rdx        # 0x18005e8d0
    180013b48:	lea    0x10(%rbp),%rcx
    180013b4c:	call   0x18000c070
    180013b51:	nop
    180013b52:	mov    %rax,%rdx
    180013b55:	lea    -0x10(%rbp),%rcx
    180013b59:	call   0x1800086c0
    180013b5e:	lea    0x5886b(%rip),%rdx        # 0x18006c3d0
@@ -37907,26 +37907,26 @@
    180013f56:	vzeroupper
    180013f59:	call   *0x4a641(%rip)        # 0x18005e5a0
    180013f5f:	nop
    180013f60:	call   *0x4a5d2(%rip)        # 0x18005e538
    180013f66:	mov    (%rax),%ecx
    180013f68:	call   *0x4a5e2(%rip)        # 0x18005e550
    180013f6e:	mov    %rax,%r8
-   180013f71:	lea    0x4a950(%rip),%rdx        # 0x18005e8c8
+   180013f71:	lea    0x4a958(%rip),%rdx        # 0x18005e8d0
    180013f78:	lea    -0x1(%rbp),%rcx
    180013f7c:	call   0x18000c070
    180013f81:	nop
    180013f82:	mov    %rax,%rdx
    180013f85:	lea    -0x39(%rbp),%rcx
    180013f89:	call   0x1800086c0
    180013f8e:	lea    0x5843b(%rip),%rdx        # 0x18006c3d0
    180013f95:	lea    -0x39(%rbp),%rcx
    180013f99:	call   0x18005c3e2
    180013f9e:	nop
-   180013f9f:	lea    0x4a932(%rip),%rdx        # 0x18005e8d8
+   180013f9f:	lea    0x4a93a(%rip),%rdx        # 0x18005e8e0
    180013fa6:	lea    -0x1(%rbp),%rcx
    180013faa:	call   0x180007010
    180013faf:	nop
    180013fb0:	mov    %rax,%rdx
    180013fb3:	lea    -0x39(%rbp),%rcx
    180013fb7:	call   0x1800086c0
    180013fbc:	lea    0x5840d(%rip),%rdx        # 0x18006c3d0
@@ -39405,15 +39405,15 @@
    18001536d:	pop    %rsi
    18001536e:	pop    %rbx
    18001536f:	ret
    180015370:	call   *0x491c2(%rip)        # 0x18005e538
    180015376:	mov    (%rax),%ecx
    180015378:	call   *0x491d2(%rip)        # 0x18005e550
    18001537e:	mov    %rax,%r8
-   180015381:	lea    0x49578(%rip),%rdx        # 0x18005e900
+   180015381:	lea    0x49580(%rip),%rdx        # 0x18005e908
    180015388:	lea    0x38(%rsp),%rcx
    18001538d:	call   0x18000c070
    180015392:	nop
    180015393:	mov    %rax,%rdx
    180015396:	lea    0x20(%rsp),%rcx
    18001539b:	call   0x1800086c0
    1800153a0:	lea    0x57029(%rip),%rdx        # 0x18006c3d0
@@ -39525,15 +39525,15 @@
    180015520:	pop    %r12
    180015522:	pop    %rdi
    180015523:	ret
    180015524:	call   *0x4900e(%rip)        # 0x18005e538
    18001552a:	mov    (%rax),%ecx
    18001552c:	call   *0x4901e(%rip)        # 0x18005e550
    180015532:	mov    %rax,%r8
-   180015535:	lea    0x493c4(%rip),%rdx        # 0x18005e900
+   180015535:	lea    0x493cc(%rip),%rdx        # 0x18005e908
    18001553c:	lea    0x40(%rsp),%rcx
    180015541:	call   0x18000c070
    180015546:	nop
    180015547:	mov    %rax,%rdx
    18001554a:	lea    0x28(%rsp),%rcx
    18001554f:	call   0x1800086c0
    180015554:	lea    0x56e75(%rip),%rdx        # 0x18006c3d0
@@ -39542,15 +39542,15 @@
    180015565:	nop
    180015566:	call   0x18000b5e0
    18001556b:	int3
    18001556c:	call   *0x48fc6(%rip)        # 0x18005e538
    180015572:	mov    (%rax),%ecx
    180015574:	call   *0x48fd6(%rip)        # 0x18005e550
    18001557a:	mov    %rax,%r8
-   18001557d:	lea    0x4937c(%rip),%rdx        # 0x18005e900
+   18001557d:	lea    0x49384(%rip),%rdx        # 0x18005e908
    180015584:	lea    0x40(%rsp),%rcx
    180015589:	call   0x18000c070
    18001558e:	nop
    18001558f:	mov    %rax,%rdx
    180015592:	lea    0x28(%rsp),%rcx
    180015597:	call   0x1800086c0
    18001559c:	lea    0x56e2d(%rip),%rdx        # 0x18006c3d0
@@ -40112,15 +40112,15 @@
    180015de0:	cmp    %rcx,%r15
    180015de3:	jbe    0x180015e1f
    180015de5:	mov    $0x2,%ecx
    180015dea:	call   *0x48820(%rip)        # 0x18005e610
    180015df0:	mov    $0xac1,%r9d
    180015df6:	lea    0x48e83(%rip),%r8        # 0x18005ec80
    180015dfd:	mov    %rax,%rcx
-   180015e00:	lea    0x48a59(%rip),%rdx        # 0x18005e860
+   180015e00:	lea    0x48a61(%rip),%rdx        # 0x18005e868
    180015e07:	lea    0x49f3a(%rip),%rax        # 0x18005fd48
    180015e0e:	mov    %rax,0x20(%rsp)
    180015e13:	call   0x1800157c0
    180015e18:	call   *0x4873a(%rip)        # 0x18005e558
    180015e1e:	int3
    180015e1f:	mov    %r15,%rax
    180015e22:	mov    0x18ff0(%rbp),%rcx
@@ -40751,15 +40751,15 @@
    1800167a2:	sub    $0xb8,%rsp
    1800167a9:	mov    0x66cd8(%rip),%rax        # 0x18007d488
    1800167b0:	xor    %rsp,%rax
    1800167b3:	mov    %rax,-0x1(%rbp)
    1800167b7:	mov    0x7f(%rbp),%r13
    1800167bb:	mov    %r8,%r12
    1800167be:	mov    %rcx,%rdi
-   1800167c1:	lea    0x48504(%rip),%r8        # 0x18005eccc
+   1800167c1:	lea    0x48508(%rip),%r8        # 0x18005ecd0
    1800167c8:	lea    -0x21(%rbp),%rcx
    1800167cc:	mov    %r9,%r15
    1800167cf:	call   0x180007920
    1800167d4:	call   *0x47d5e(%rip)        # 0x18005e538
    1800167da:	mov    -0x21(%rbp),%rbx
    1800167de:	lea    -0x6d(%rbp),%rcx
    1800167e2:	xor    %r14d,%r14d
@@ -40856,16 +40856,16 @@
    180016982:	cmp    $0xffffffffffffffff,%rax
    180016986:	jne    0x1800169c0
    180016988:	lea    0x3(%rax),%ecx
    18001698b:	call   *0x47c7f(%rip)        # 0x18005e610
    180016991:	mov    $0x5b,%r9d
    180016997:	lea    0x47e72(%rip),%r8        # 0x18005e810
    18001699e:	mov    %rax,%rcx
-   1800169a1:	lea    0x47eb8(%rip),%rdx        # 0x18005e860
-   1800169a8:	lea    0x47ef9(%rip),%rax        # 0x18005e8a8
+   1800169a1:	lea    0x47ec0(%rip),%rdx        # 0x18005e868
+   1800169a8:	lea    0x47f01(%rip),%rax        # 0x18005e8b0
    1800169af:	mov    %rax,0x20(%rsp)
    1800169b4:	call   0x1800157c0
    1800169b9:	call   *0x47b99(%rip)        # 0x18005e558
    1800169bf:	int3
    1800169c0:	mov    -0x19(%rbp),%rsi
    1800169c4:	mov    0x1540(%rdi),%r14
    1800169cb:	sub    %rax,%rsi
@@ -40944,77 +40944,77 @@
    180016af9:	pop    %r13
    180016afb:	pop    %r12
    180016afd:	pop    %rdi
    180016afe:	pop    %rsi
    180016aff:	pop    %rbx
    180016b00:	pop    %rbp
    180016b01:	ret
-   180016b02:	lea    0x47dcf(%rip),%rdx        # 0x18005e8d8
+   180016b02:	lea    0x47dd7(%rip),%rdx        # 0x18005e8e0
    180016b09:	lea    -0x21(%rbp),%rcx
    180016b0d:	call   0x180007010
    180016b12:	mov    %rax,%rdx
    180016b15:	lea    -0x69(%rbp),%rcx
    180016b19:	call   0x1800086c0
    180016b1e:	lea    0x558ab(%rip),%rdx        # 0x18006c3d0
    180016b25:	lea    -0x69(%rbp),%rcx
    180016b29:	call   0x18005c3e2
    180016b2e:	int3
    180016b2f:	call   *0x47a03(%rip)        # 0x18005e538
    180016b35:	mov    (%rax),%ecx
    180016b37:	call   *0x47a13(%rip)        # 0x18005e550
    180016b3d:	mov    %rax,%r8
-   180016b40:	lea    0x47d81(%rip),%rdx        # 0x18005e8c8
+   180016b40:	lea    0x47d89(%rip),%rdx        # 0x18005e8d0
    180016b47:	lea    -0x21(%rbp),%rcx
    180016b4b:	call   0x18000c070
    180016b50:	mov    %rax,%rdx
    180016b53:	lea    -0x69(%rbp),%rcx
    180016b57:	call   0x1800086c0
    180016b5c:	lea    0x5586d(%rip),%rdx        # 0x18006c3d0
    180016b63:	lea    -0x69(%rbp),%rcx
    180016b67:	call   0x18005c3e2
    180016b6c:	int3
-   180016b6d:	lea    0x47d64(%rip),%rdx        # 0x18005e8d8
+   180016b6d:	lea    0x47d6c(%rip),%rdx        # 0x18005e8e0
    180016b74:	lea    -0x21(%rbp),%rcx
    180016b78:	call   0x180007010
    180016b7d:	mov    %rax,%rdx
    180016b80:	lea    -0x69(%rbp),%rcx
    180016b84:	call   0x1800086c0
    180016b89:	lea    0x55840(%rip),%rdx        # 0x18006c3d0
    180016b90:	lea    -0x69(%rbp),%rcx
    180016b94:	call   0x18005c3e2
    180016b99:	int3
    180016b9a:	call   *0x47998(%rip)        # 0x18005e538
    180016ba0:	mov    (%rax),%ecx
    180016ba2:	call   *0x479a8(%rip)        # 0x18005e550
    180016ba8:	mov    %rax,%r8
-   180016bab:	lea    0x47d16(%rip),%rdx        # 0x18005e8c8
+   180016bab:	lea    0x47d1e(%rip),%rdx        # 0x18005e8d0
    180016bb2:	lea    -0x21(%rbp),%rcx
    180016bb6:	call   0x18000c070
    180016bbb:	mov    %rax,%rdx
    180016bbe:	lea    -0x69(%rbp),%rcx
    180016bc2:	call   0x1800086c0
    180016bc7:	lea    0x55802(%rip),%rdx        # 0x18006c3d0
    180016bce:	lea    -0x69(%rbp),%rcx
    180016bd2:	call   0x18005c3e2
    180016bd7:	int3
-   180016bd8:	lea    0x47cf9(%rip),%rdx        # 0x18005e8d8
+   180016bd8:	lea    0x47d01(%rip),%rdx        # 0x18005e8e0
    180016bdf:	lea    -0x21(%rbp),%rcx
    180016be3:	call   0x180007010
    180016be8:	mov    %rax,%rdx
    180016beb:	lea    -0x69(%rbp),%rcx
    180016bef:	call   0x1800086c0
    180016bf4:	lea    0x557d5(%rip),%rdx        # 0x18006c3d0
    180016bfb:	lea    -0x69(%rbp),%rcx
    180016bff:	call   0x18005c3e2
    180016c04:	int3
    180016c05:	call   *0x4792d(%rip)        # 0x18005e538
    180016c0b:	mov    (%rax),%ecx
    180016c0d:	call   *0x4793d(%rip)        # 0x18005e550
    180016c13:	mov    %rax,%r8
-   180016c16:	lea    0x47cab(%rip),%rdx        # 0x18005e8c8
+   180016c16:	lea    0x47cb3(%rip),%rdx        # 0x18005e8d0
    180016c1d:	lea    -0x21(%rbp),%rcx
    180016c21:	call   0x18000c070
    180016c26:	mov    %rax,%rdx
    180016c29:	lea    -0x69(%rbp),%rcx
    180016c2d:	call   0x1800086c0
    180016c32:	lea    0x55797(%rip),%rdx        # 0x18006c3d0
    180016c39:	lea    -0x69(%rbp),%rcx
@@ -43184,85 +43184,85 @@
    180018c2d:	ret
    180018c2e:	call   *0x4596c(%rip)        # 0x18005e5a0
    180018c34:	int3
    180018c35:	call   *0x458fd(%rip)        # 0x18005e538
    180018c3b:	mov    (%rax),%ecx
    180018c3d:	call   *0x4590d(%rip)        # 0x18005e550
    180018c43:	mov    %rax,%r8
-   180018c46:	lea    0x45cb3(%rip),%rdx        # 0x18005e900
+   180018c46:	lea    0x45cbb(%rip),%rdx        # 0x18005e908
    180018c4d:	lea    -0x38(%rbp),%rcx
    180018c51:	call   0x18000c070
    180018c56:	mov    %rax,%rdx
    180018c59:	lea    -0x50(%rbp),%rcx
    180018c5d:	call   0x1800086c0
    180018c62:	lea    0x53767(%rip),%rdx        # 0x18006c3d0
    180018c69:	lea    -0x50(%rbp),%rcx
    180018c6d:	call   0x18005c3e2
    180018c72:	int3
    180018c73:	call   *0x458bf(%rip)        # 0x18005e538
    180018c79:	mov    (%rax),%ecx
    180018c7b:	call   *0x458cf(%rip)        # 0x18005e550
    180018c81:	mov    %rax,%r8
-   180018c84:	lea    0x45c75(%rip),%rdx        # 0x18005e900
+   180018c84:	lea    0x45c7d(%rip),%rdx        # 0x18005e908
    180018c8b:	lea    -0x38(%rbp),%rcx
    180018c8f:	call   0x18000c070
    180018c94:	mov    %rax,%rdx
    180018c97:	lea    -0x50(%rbp),%rcx
    180018c9b:	call   0x1800086c0
    180018ca0:	lea    0x53729(%rip),%rdx        # 0x18006c3d0
    180018ca7:	lea    -0x50(%rbp),%rcx
    180018cab:	call   0x18005c3e2
    180018cb0:	int3
    180018cb1:	call   *0x45881(%rip)        # 0x18005e538
    180018cb7:	mov    (%rax),%ecx
    180018cb9:	call   *0x45891(%rip)        # 0x18005e550
    180018cbf:	mov    %rax,%r8
-   180018cc2:	lea    0x45c37(%rip),%rdx        # 0x18005e900
+   180018cc2:	lea    0x45c3f(%rip),%rdx        # 0x18005e908
    180018cc9:	lea    -0x38(%rbp),%rcx
    180018ccd:	call   0x18000c070
    180018cd2:	mov    %rax,%rdx
    180018cd5:	lea    -0x50(%rbp),%rcx
    180018cd9:	call   0x1800086c0
    180018cde:	lea    0x536eb(%rip),%rdx        # 0x18006c3d0
    180018ce5:	lea    -0x50(%rbp),%rcx
    180018ce9:	call   0x18005c3e2
    180018cee:	int3
    180018cef:	call   *0x45843(%rip)        # 0x18005e538
    180018cf5:	mov    (%rax),%ecx
    180018cf7:	call   *0x45853(%rip)        # 0x18005e550
    180018cfd:	mov    %rax,%r8
-   180018d00:	lea    0x45bf9(%rip),%rdx        # 0x18005e900
+   180018d00:	lea    0x45c01(%rip),%rdx        # 0x18005e908
    180018d07:	lea    -0x38(%rbp),%rcx
    180018d0b:	call   0x18000c070
    180018d10:	mov    %rax,%rdx
    180018d13:	lea    -0x50(%rbp),%rcx
    180018d17:	call   0x1800086c0
    180018d1c:	lea    0x536ad(%rip),%rdx        # 0x18006c3d0
    180018d23:	lea    -0x50(%rbp),%rcx
    180018d27:	call   0x18005c3e2
    180018d2c:	int3
    180018d2d:	call   *0x45805(%rip)        # 0x18005e538
    180018d33:	mov    (%rax),%ecx
    180018d35:	call   *0x45815(%rip)        # 0x18005e550
    180018d3b:	mov    %rax,%r8
-   180018d3e:	lea    0x45bbb(%rip),%rdx        # 0x18005e900
+   180018d3e:	lea    0x45bc3(%rip),%rdx        # 0x18005e908
    180018d45:	lea    -0x38(%rbp),%rcx
    180018d49:	call   0x18000c070
    180018d4e:	mov    %rax,%rdx
    180018d51:	lea    -0x50(%rbp),%rcx
    180018d55:	call   0x1800086c0
    180018d5a:	lea    0x5366f(%rip),%rdx        # 0x18006c3d0
    180018d61:	lea    -0x50(%rbp),%rcx
    180018d65:	call   0x18005c3e2
    180018d6a:	int3
    180018d6b:	call   *0x457c7(%rip)        # 0x18005e538
    180018d71:	mov    (%rax),%ecx
    180018d73:	call   *0x457d7(%rip)        # 0x18005e550
    180018d79:	mov    %rax,%r8
-   180018d7c:	lea    0x45b7d(%rip),%rdx        # 0x18005e900
+   180018d7c:	lea    0x45b85(%rip),%rdx        # 0x18005e908
    180018d83:	lea    -0x38(%rbp),%rcx
    180018d87:	call   0x18000c070
    180018d8c:	mov    %rax,%rdx
    180018d8f:	lea    -0x50(%rbp),%rcx
    180018d93:	call   0x1800086c0
    180018d98:	lea    0x53631(%rip),%rdx        # 0x18006c3d0
    180018d9f:	lea    -0x50(%rbp),%rcx
@@ -43488,15 +43488,15 @@
    180019121:	test   %al,%al
    180019123:	je     0x18001915f
    180019125:	mov    $0x2,%ecx
    18001912a:	call   *0x454e0(%rip)        # 0x18005e610
    180019130:	mov    $0xad6,%r9d
    180019136:	lea    0x45b43(%rip),%r8        # 0x18005ec80
    18001913d:	mov    %rax,%rcx
-   180019140:	lea    0x45719(%rip),%rdx        # 0x18005e860
+   180019140:	lea    0x45721(%rip),%rdx        # 0x18005e868
    180019147:	lea    0x46c12(%rip),%rax        # 0x18005fd60
    18001914e:	mov    %rax,0x20(%rsp)
    180019153:	call   0x1800157c0
    180019158:	call   *0x453fa(%rip)        # 0x18005e558
    18001915e:	int3
    18001915f:	mov    0x17ff0(%rbp),%rax
    180019166:	movslq 0x4(%rax),%rcx
@@ -43527,15 +43527,15 @@
    1800191fe:	cmp    %rdi,%rax
    180019201:	je     0x18001923d
    180019203:	mov    $0x2,%ecx
    180019208:	call   *0x45402(%rip)        # 0x18005e610
    18001920e:	mov    $0xae1,%r9d
    180019214:	lea    0x45a65(%rip),%r8        # 0x18005ec80
    18001921b:	mov    %rax,%rcx
-   18001921e:	lea    0x4563b(%rip),%rdx        # 0x18005e860
+   18001921e:	lea    0x45643(%rip),%rdx        # 0x18005e868
    180019225:	lea    0x46b4c(%rip),%rax        # 0x18005fd78
    18001922c:	mov    %rax,0x20(%rsp)
    180019231:	call   0x1800157c0
    180019236:	call   *0x4531c(%rip)        # 0x18005e558
    18001923c:	int3
    18001923d:	test   %rbx,%rbx
    180019240:	je     0x180019260
@@ -43556,15 +43556,15 @@
    180019281:	cmp    %rdi,%rax
    180019284:	je     0x1800192c0
    180019286:	mov    $0x2,%ecx
    18001928b:	call   *0x4537f(%rip)        # 0x18005e610
    180019291:	mov    $0xaf1,%r9d
    180019297:	lea    0x459e2(%rip),%r8        # 0x18005ec80
    18001929e:	mov    %rax,%rcx
-   1800192a1:	lea    0x455b8(%rip),%rdx        # 0x18005e860
+   1800192a1:	lea    0x455c0(%rip),%rdx        # 0x18005e868
    1800192a8:	lea    0x46af1(%rip),%rax        # 0x18005fda0
    1800192af:	mov    %rax,0x20(%rsp)
    1800192b4:	call   0x1800157c0
    1800192b9:	call   *0x45299(%rip)        # 0x18005e558
    1800192bf:	int3
    1800192c0:	test   %rdi,%rdi
    1800192c3:	je     0x1800192db
@@ -43587,15 +43587,15 @@
    180019310:	cmp    %rax,0x1448(%r15)
    180019317:	je     0x180019353
    180019319:	mov    $0x2,%ecx
    18001931e:	call   *0x452ec(%rip)        # 0x18005e610
    180019324:	mov    $0xb08,%r9d
    18001932a:	lea    0x4594f(%rip),%r8        # 0x18005ec80
    180019331:	mov    %rax,%rcx
-   180019334:	lea    0x45525(%rip),%rdx        # 0x18005e860
+   180019334:	lea    0x4552d(%rip),%rdx        # 0x18005e868
    18001933b:	lea    0x46a8e(%rip),%rax        # 0x18005fdd0
    180019342:	mov    %rax,0x20(%rsp)
    180019347:	call   0x1800157c0
    18001934c:	call   *0x45206(%rip)        # 0x18005e558
    180019352:	int3
    180019353:	mov    0x1428(%r15),%rcx
    18001935a:	call   0x180037740
@@ -43709,15 +43709,15 @@
    180019554:	cmp    %rcx,%rbx
    180019557:	jbe    0x180019593
    180019559:	mov    $0x2,%ecx
    18001955e:	call   *0x450ac(%rip)        # 0x18005e610
    180019564:	mov    $0xb2f,%r9d
    18001956a:	lea    0x4570f(%rip),%r8        # 0x18005ec80
    180019571:	mov    %rax,%rcx
-   180019574:	lea    0x452e5(%rip),%rdx        # 0x18005e860
+   180019574:	lea    0x452ed(%rip),%rdx        # 0x18005e868
    18001957b:	lea    0x4686e(%rip),%rax        # 0x18005fdf0
    180019582:	mov    %rax,0x20(%rsp)
    180019587:	call   0x1800157c0
    18001958c:	call   *0x44fc6(%rip)        # 0x18005e558
    180019592:	int3
    180019593:	mov    %rbx,%rax
    180019596:	mov    0x18ff0(%rbp),%rcx
@@ -112265,168 +112265,171 @@
    18005e819:	jae    0x18005e848
    18005e81b:	jb     0x18005e892
    18005e81d:	outsb  %ds:(%rsi),(%dx)
    18005e81e:	outsb  %ds:(%rsi),(%dx)
    18005e81f:	gs jb  0x18005e87e
    18005e822:	(bad)
    18005e827:	sub    $0x6c697562,%eax
-   18005e82c:	fs pop %rsp
-   18005e82e:	pop    %rdi
-   18005e82f:	ja     0x18005e8a0
-   18005e831:	jb     0x18005e89e
-   18005e833:	pop    %rsp
-   18005e834:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   18005e83b:	insl   (%dx),%es:(%rdi)
-   18005e83c:	pop    %rsp
-   18005e83d:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   18005e844:	insl   (%dx),%es:(%rdi)
-   18005e845:	pop    %rsp
-   18005e846:	jae    0x18005e8ba
-   18005e848:	movsxd 0x6c(%rsp,%rbp,2),%ebx
-   18005e84c:	(bad)
-   18005e84d:	insl   (%dx),%es:(%rdi)
-   18005e84e:	(bad)
-   18005e84f:	pop    %rsp
-   18005e850:	insb   (%dx),%es:(%rdi)
-   18005e851:	insb   (%dx),%es:(%rdi)
+   18005e82c:	fs sub $0x5c77656e,%eax
+   18005e832:	pop    %rdi
+   18005e833:	ja     0x18005e8a4
+   18005e835:	jb     0x18005e8a2
+   18005e837:	pop    %rsp
+   18005e838:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   18005e83f:	insl   (%dx),%es:(%rdi)
+   18005e840:	pop    %rsp
+   18005e841:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   18005e848:	insl   (%dx),%es:(%rdi)
+   18005e849:	pop    %rsp
+   18005e84a:	jae    0x18005e8be
+   18005e84c:	movsxd 0x6c(%rsp,%rbp,2),%ebx
+   18005e850:	(bad)
+   18005e851:	insl   (%dx),%es:(%rdi)
    18005e852:	(bad)
-   18005e853:	insl   (%dx),%es:(%rdi)
-   18005e854:	(bad)
-   18005e855:	sub    $0x6c697475,%eax
-   18005e85a:	cs push $0x0
-   18005e860:	rex.WR
-   18005e861:	rex.WR
-   18005e862:	rex.B
-   18005e863:	rex.WRB
-   18005e864:	pop    %r15
-   18005e866:	push   %r11
-   18005e868:	push   %rbx
-   18005e869:	rex.RB push %r10
-   18005e86b:	push   %rsp
-   18005e86c:	cmp    (%rax),%ah
-   18005e86e:	and    $0x64253a73,%eax
-   18005e873:	cmp    (%rax),%ah
-   18005e875:	and    $0xa73,%eax
-   18005e87a:	add    %al,(%rax)
-   18005e87c:	add    %al,(%rax)
-   18005e87e:	add    %al,(%rax)
-   18005e880:	jae    0x18005e8eb
-   18005e882:	jp     0x18005e8e9
-   18005e884:	xor    (%rax),%ah
-   18005e886:	cmp    $0x6973203d,%eax
-   18005e88b:	jp     0x18005e8f2
-   18005e88d:	add    %al,(%rax)
-   18005e88f:	add    %ah,0x61(%rsi)
-   18005e892:	imul   $0x206f7420,0x64(%rbp,%riz,2),%ebp
-   18005e89a:	outsl  %ds:(%rsi),(%dx)
-   18005e89b:	jo     0x18005e902
-   18005e89d:	outsb  %ds:(%rsi),(%dx)
-   18005e89e:	and    %ah,0x25203a73(%rip)        # 0x1a5262317
-   18005e8a4:	jae    0x18005e8a6
-   18005e8a6:	add    %al,(%rax)
-   18005e8a8:	jb     0x18005e90f
-   18005e8aa:	je     0x18005e8cc
-   18005e8ac:	and    %edi,0x312d20(%rip)        # 0x1803715d2
-   18005e8b2:	add    %al,(%rax)
-   18005e8b4:	add    %al,(%rax)
-   18005e8b6:	add    %al,(%rax)
-   18005e8b8:	jb     0x18005e91f
-   18005e8ba:	je     0x18005e8dc
-   18005e8bc:	cmp    $0x30203d,%eax
-   18005e8c1:	add    %al,(%rax)
-   18005e8c3:	add    %al,(%rax)
-   18005e8c5:	add    %al,(%rax)
-   18005e8c7:	add    %dh,0x65(%rdx)
-   18005e8ca:	(bad)
-   18005e8cb:	and    %ah,%fs:0x72(%rbp)
-   18005e8cf:	jb     0x18005e940
-   18005e8d1:	jb     0x18005e90d
-   18005e8d3:	and    %ah,0x75000073(%rip)        # 0x1f505e94c
-   18005e8d9:	outsb  %ds:(%rsi),(%dx)
-   18005e8da:	gs js  0x18005e94d
-   18005e8dd:	movsxd %gs:0x64(%rbp,%riz,2),%esi
-   18005e8e2:	insb   (%dx),%es:(%rdi)
-   18005e8e3:	jns    0x18005e905
-   18005e8e5:	jb     0x18005e94c
-   18005e8e7:	(bad)
-   18005e8e8:	movsxd 0x65(%rax),%ebp
-   18005e8eb:	and    %ah,%fs:0x6e(%rbp)
-   18005e8ef:	and    %ch,%fs:0x66(%rdi)
-   18005e8f3:	and    %ah,0x69(%rsi)
-   18005e8f6:	insb   (%dx),%es:(%rdi)
-   18005e8f7:	add    %al,%gs:(%rax)
-   18005e8fa:	add    %al,(%rax)
-   18005e8fc:	add    %al,(%rax)
-   18005e8fe:	add    %al,(%rax)
-   18005e900:	ja     0x18005e974
-   18005e902:	imul   $0x6f727265,0x20(%rbp,%riz,2),%esi
-   18005e90a:	jb     0x18005e946
-   18005e90c:	and    %ah,0x6f460073(%rip)        # 0x1ef4be985
-   18005e912:	jb     0x18005e981
-   18005e914:	(bad)
-   18005e915:	je     0x18005e964
-   18005e917:	gs jae 0x18005e98d
-   18005e91a:	(bad)
-   18005e91b:	and    %spl,%gs:0x61(%r14d)
-   18005e921:	imul   $0x43000000,0x64(%rbp,%riz,2),%ebp
-   18005e929:	jb     0x18005e990
-   18005e92b:	(bad)
-   18005e92c:	je     0x18005e993
-   18005e92e:	imul   $0x69707061,0x4d(%rbp,%r12,2),%r13d
-   18005e937:	outsb  %ds:(%rsi),(%dx)
-   18005e938:	and    %spl,0x61(%r14d)
-   18005e93d:	imul   $0x7325203a,0x64(%rbp,%riz,2),%ebp
-   18005e945:	add    %al,(%rax)
-   18005e947:	add    %cl,0x61(%rbp)
-   18005e94a:	jo     0x18005e9a2
-   18005e94c:	imul   $0x6946664f,0x77(%rbp),%esp
-   18005e953:	insb   (%dx),%es:(%rdi)
-   18005e954:	and    %ah,%gs:0x61(%rsi)
-   18005e958:	imul   $0x7325203a,0x64(%rbp,%riz,2),%ebp
-	...
-   18005e968:	ja     0x18005e9cb
-   18005e96a:	jb     0x18005e9da
-   18005e96c:	imul   $0x7250203a,0x67(%rsi),%ebp
-   18005e973:	gs data16 gs je 0x18005e9db
-   18005e978:	push   $0x74726956
-   18005e97d:	jne    0x18005e9e0
-   18005e97f:	insb   (%dx),%es:(%rdi)
-   18005e980:	rex.WRB
-   18005e981:	gs insl (%dx),%es:(%rdi)
-   18005e983:	outsl  %ds:(%rsi),(%dx)
-   18005e984:	jb     0x18005e9ff
-   18005e986:	and    %ah,0x61(%rsi)
-   18005e989:	imul   $0x7325203a,0x64(%rbp,%riz,2),%ebp
-   18005e991:	or     (%rax),%al
-   18005e993:	add    %al,(%rax)
-   18005e995:	add    %al,(%rax)
-   18005e997:	add    %dh,0x61(%rdi)
-   18005e99a:	jb     0x18005ea0a
-   18005e99c:	imul   $0x6e55203a,0x67(%rsi),%ebp
-   18005e9a3:	insl   (%dx),%es:(%rdi)
-   18005e9a4:	(bad)
-   18005e9a5:	jo     0x18005e9fd
-   18005e9a7:	imul   $0x6946664f,0x77(%rbp),%esp
-   18005e9ae:	insb   (%dx),%es:(%rdi)
-   18005e9af:	and    %ah,%gs:0x61(%rsi)
-   18005e9b3:	imul   $0x7325203a,0x64(%rbp,%riz,2),%ebp
-   18005e9bb:	or     (%rax),%al
-   18005e9bd:	add    %al,(%rax)
-   18005e9bf:	add    %ah,0x64(%rcx)
-   18005e9c2:	fs jb  0x18005e9e5
-   18005e9c5:	cmp    $0x554e203d,%eax
-   18005e9ca:	rex.WR
-   18005e9cb:	rex.WR and %r12b,(%rsi)
-   18005e9ce:	es and %dh,0x69(%rbx)
-   18005e9d2:	jp     0x18005ea39
-   18005e9d4:	and    %bh,0x30203d(%rip)        # 0x180360a17
-   18005e9da:	add    %al,(%rax)
-   18005e9dc:	(bad)
-   18005e9dd:	fs fs jb 0x18005e9e1
+   18005e853:	pop    %rsp
+   18005e854:	insb   (%dx),%es:(%rdi)
+   18005e855:	insb   (%dx),%es:(%rdi)
+   18005e856:	(bad)
+   18005e857:	insl   (%dx),%es:(%rdi)
+   18005e858:	(bad)
+   18005e859:	sub    $0x6c697475,%eax
+   18005e85e:	cs push $0x0
+   18005e864:	add    %al,(%rax)
+   18005e866:	add    %al,(%rax)
+   18005e868:	rex.WR
+   18005e869:	rex.WR
+   18005e86a:	rex.B
+   18005e86b:	rex.WRB
+   18005e86c:	pop    %r15
+   18005e86e:	push   %r11
+   18005e870:	push   %rbx
+   18005e871:	rex.RB push %r10
+   18005e873:	push   %rsp
+   18005e874:	cmp    (%rax),%ah
+   18005e876:	and    $0x64253a73,%eax
+   18005e87b:	cmp    (%rax),%ah
+   18005e87d:	and    $0xa73,%eax
+   18005e882:	add    %al,(%rax)
+   18005e884:	add    %al,(%rax)
+   18005e886:	add    %al,(%rax)
+   18005e888:	jae    0x18005e8f3
+   18005e88a:	jp     0x18005e8f1
+   18005e88c:	xor    (%rax),%ah
+   18005e88e:	cmp    $0x6973203d,%eax
+   18005e893:	jp     0x18005e8fa
+   18005e895:	add    %al,(%rax)
+   18005e897:	add    %ah,0x61(%rsi)
+   18005e89a:	imul   $0x206f7420,0x64(%rbp,%riz,2),%ebp
+   18005e8a2:	outsl  %ds:(%rsi),(%dx)
+   18005e8a3:	jo     0x18005e90a
+   18005e8a5:	outsb  %ds:(%rsi),(%dx)
+   18005e8a6:	and    %ah,0x25203a73(%rip)        # 0x1a526231f
+   18005e8ac:	jae    0x18005e8ae
+   18005e8ae:	add    %al,(%rax)
+   18005e8b0:	jb     0x18005e917
+   18005e8b2:	je     0x18005e8d4
+   18005e8b4:	and    %edi,0x312d20(%rip)        # 0x1803715da
+   18005e8ba:	add    %al,(%rax)
+   18005e8bc:	add    %al,(%rax)
+   18005e8be:	add    %al,(%rax)
+   18005e8c0:	jb     0x18005e927
+   18005e8c2:	je     0x18005e8e4
+   18005e8c4:	cmp    $0x30203d,%eax
+   18005e8c9:	add    %al,(%rax)
+   18005e8cb:	add    %al,(%rax)
+   18005e8cd:	add    %al,(%rax)
+   18005e8cf:	add    %dh,0x65(%rdx)
+   18005e8d2:	(bad)
+   18005e8d3:	and    %ah,%fs:0x72(%rbp)
+   18005e8d7:	jb     0x18005e948
+   18005e8d9:	jb     0x18005e915
+   18005e8db:	and    %ah,0x75000073(%rip)        # 0x1f505e954
+   18005e8e1:	outsb  %ds:(%rsi),(%dx)
+   18005e8e2:	gs js  0x18005e955
+   18005e8e5:	movsxd %gs:0x64(%rbp,%riz,2),%esi
+   18005e8ea:	insb   (%dx),%es:(%rdi)
+   18005e8eb:	jns    0x18005e90d
+   18005e8ed:	jb     0x18005e954
+   18005e8ef:	(bad)
+   18005e8f0:	movsxd 0x65(%rax),%ebp
+   18005e8f3:	and    %ah,%fs:0x6e(%rbp)
+   18005e8f7:	and    %ch,%fs:0x66(%rdi)
+   18005e8fb:	and    %ah,0x69(%rsi)
+   18005e8fe:	insb   (%dx),%es:(%rdi)
+   18005e8ff:	add    %al,%gs:(%rax)
+   18005e902:	add    %al,(%rax)
+   18005e904:	add    %al,(%rax)
+   18005e906:	add    %al,(%rax)
+   18005e908:	ja     0x18005e97c
+   18005e90a:	imul   $0x6f727265,0x20(%rbp,%riz,2),%esi
+   18005e912:	jb     0x18005e94e
+   18005e914:	and    %ah,0x6f460073(%rip)        # 0x1ef4be98d
+   18005e91a:	jb     0x18005e989
+   18005e91c:	(bad)
+   18005e91d:	je     0x18005e96c
+   18005e91f:	gs jae 0x18005e995
+   18005e922:	(bad)
+   18005e923:	and    %spl,%gs:0x61(%r14d)
+   18005e929:	imul   $0x43000000,0x64(%rbp,%riz,2),%ebp
+   18005e931:	jb     0x18005e998
+   18005e933:	(bad)
+   18005e934:	je     0x18005e99b
+   18005e936:	imul   $0x69707061,0x4d(%rbp,%r12,2),%r13d
+   18005e93f:	outsb  %ds:(%rsi),(%dx)
+   18005e940:	and    %spl,0x61(%r14d)
+   18005e945:	imul   $0x7325203a,0x64(%rbp,%riz,2),%ebp
+   18005e94d:	add    %al,(%rax)
+   18005e94f:	add    %cl,0x61(%rbp)
+   18005e952:	jo     0x18005e9aa
+   18005e954:	imul   $0x6946664f,0x77(%rbp),%esp
+   18005e95b:	insb   (%dx),%es:(%rdi)
+   18005e95c:	and    %ah,%gs:0x61(%rsi)
+   18005e960:	imul   $0x7325203a,0x64(%rbp,%riz,2),%ebp
 	...
+   18005e970:	ja     0x18005e9d3
+   18005e972:	jb     0x18005e9e2
+   18005e974:	imul   $0x7250203a,0x67(%rsi),%ebp
+   18005e97b:	gs data16 gs je 0x18005e9e3
+   18005e980:	push   $0x74726956
+   18005e985:	jne    0x18005e9e8
+   18005e987:	insb   (%dx),%es:(%rdi)
+   18005e988:	rex.WRB
+   18005e989:	gs insl (%dx),%es:(%rdi)
+   18005e98b:	outsl  %ds:(%rsi),(%dx)
+   18005e98c:	jb     0x18005ea07
+   18005e98e:	and    %ah,0x61(%rsi)
+   18005e991:	imul   $0x7325203a,0x64(%rbp,%riz,2),%ebp
+   18005e999:	or     (%rax),%al
+   18005e99b:	add    %al,(%rax)
+   18005e99d:	add    %al,(%rax)
+   18005e99f:	add    %dh,0x61(%rdi)
+   18005e9a2:	jb     0x18005ea12
+   18005e9a4:	imul   $0x6e55203a,0x67(%rsi),%ebp
+   18005e9ab:	insl   (%dx),%es:(%rdi)
+   18005e9ac:	(bad)
+   18005e9ad:	jo     0x18005ea05
+   18005e9af:	imul   $0x6946664f,0x77(%rbp),%esp
+   18005e9b6:	insb   (%dx),%es:(%rdi)
+   18005e9b7:	and    %ah,%gs:0x61(%rsi)
+   18005e9bb:	imul   $0x7325203a,0x64(%rbp,%riz,2),%ebp
+   18005e9c3:	or     (%rax),%al
+   18005e9c5:	add    %al,(%rax)
+   18005e9c7:	add    %ah,0x64(%rcx)
+   18005e9ca:	fs jb  0x18005e9ed
+   18005e9cd:	cmp    $0x554e203d,%eax
+   18005e9d2:	rex.WR
+   18005e9d3:	rex.WR and %r12b,(%rsi)
+   18005e9d6:	es and %dh,0x69(%rbx)
+   18005e9da:	jp     0x18005ea41
+   18005e9dc:	and    %bh,0x30203d(%rip)        # 0x180360a1f
+   18005e9e2:	add    %al,(%rax)
+   18005e9e4:	(bad)
+   18005e9e5:	fs fs jb 0x18005e9e9
+   18005e9e9:	add    %al,(%rax)
+   18005e9eb:	add    %al,(%rax)
    18005e9ed:	add    %al,(%rax)
    18005e9ef:	add    %dh,0x61(%rdi)
    18005e9f2:	jb     0x18005ea62
    18005e9f4:	imul   $0x6166203a,0x67(%rsi),%ebp
    18005e9fb:	imul   $0x206f7420,0x64(%rbp,%riz,2),%ebp
    18005ea03:	push   %rsi
    18005ea04:	imul   $0x4c6c6175,0x74(%rdx),%esi
@@ -112653,50 +112656,53 @@
    18005ec89:	jae    0x18005ecb8
    18005ec8b:	jb     0x18005ed02
    18005ec8d:	outsb  %ds:(%rsi),(%dx)
    18005ec8e:	outsb  %ds:(%rsi),(%dx)
    18005ec8f:	gs jb  0x18005ecee
    18005ec92:	(bad)
    18005ec97:	sub    $0x6c697562,%eax
-   18005ec9c:	fs pop %rsp
-   18005ec9e:	pop    %rdi
-   18005ec9f:	ja     0x18005ed10
-   18005eca1:	jb     0x18005ed0e
-   18005eca3:	pop    %rsp
-   18005eca4:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   18005ecab:	insl   (%dx),%es:(%rdi)
-   18005ecac:	pop    %rsp
-   18005ecad:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   18005ecb4:	insl   (%dx),%es:(%rdi)
-   18005ecb5:	pop    %rsp
-   18005ecb6:	jae    0x18005ed2a
-   18005ecb8:	movsxd 0x6c(%rsp,%rbp,2),%ebx
-   18005ecbc:	(bad)
-   18005ecbd:	insl   (%dx),%es:(%rdi)
-   18005ecbe:	(bad)
-   18005ecbf:	pop    %rsp
-   18005ecc0:	insb   (%dx),%es:(%rdi)
-   18005ecc1:	insb   (%dx),%es:(%rdi)
+   18005ec9c:	fs sub $0x5c77656e,%eax
+   18005eca2:	pop    %rdi
+   18005eca3:	ja     0x18005ed14
+   18005eca5:	jb     0x18005ed12
+   18005eca7:	pop    %rsp
+   18005eca8:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   18005ecaf:	insl   (%dx),%es:(%rdi)
+   18005ecb0:	pop    %rsp
+   18005ecb1:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   18005ecb8:	insl   (%dx),%es:(%rdi)
+   18005ecb9:	pop    %rsp
+   18005ecba:	jae    0x18005ed2e
+   18005ecbc:	movsxd 0x6c(%rsp,%rbp,2),%ebx
+   18005ecc0:	(bad)
+   18005ecc1:	insl   (%dx),%es:(%rdi)
    18005ecc2:	(bad)
-   18005ecc3:	insl   (%dx),%es:(%rdi)
-   18005ecc4:	(bad)
-   18005ecc5:	cs movsxd 0x70(%rax),%esi
-   18005ecc9:	add    %al,(%rax)
-   18005eccb:	add    %dh,0x62(%rdx)
-   18005ecce:	add    %al,(%rax)
-   18005ecd0:	(bad)
-   18005ecd5:	sub    $0x3a6d6c6c,%eax
-   18005ecda:	and    %ch,0x61(%rdi,%rbp,2)
-   18005ecde:	imul   $0x646f6d20,%fs:0x67(%rsi),%ebp
-   18005ece6:	gs insb (%dx),%es:(%rdi)
-   18005ece8:	and    %ah,0x72(%rsi)
-   18005eceb:	outsl  %ds:(%rsi),(%dx)
-   18005ecec:	insl   (%dx),%es:(%rdi)
-   18005eced:	and    %ah,0xa73(%rip)        # 0x18005f766
-	...
+   18005ecc3:	pop    %rsp
+   18005ecc4:	insb   (%dx),%es:(%rdi)
+   18005ecc5:	insb   (%dx),%es:(%rdi)
+   18005ecc6:	(bad)
+   18005ecc7:	insl   (%dx),%es:(%rdi)
+   18005ecc8:	(bad)
+   18005ecc9:	cs movsxd 0x70(%rax),%esi
+   18005eccd:	add    %al,(%rax)
+   18005eccf:	add    %dh,0x62(%rdx)
+   18005ecd2:	add    %al,(%rax)
+   18005ecd4:	add    %al,(%rax)
+   18005ecd6:	add    %al,(%rax)
+   18005ecd8:	(bad)
+   18005ecdd:	sub    $0x3a6d6c6c,%eax
+   18005ece2:	and    %ch,0x61(%rdi,%rbp,2)
+   18005ece6:	imul   $0x646f6d20,%fs:0x67(%rsi),%ebp
+   18005ecee:	gs insb (%dx),%es:(%rdi)
+   18005ecf0:	and    %ah,0x72(%rsi)
+   18005ecf3:	outsl  %ds:(%rsi),(%dx)
+   18005ecf4:	insl   (%dx),%es:(%rdi)
+   18005ecf5:	and    %ah,0xa73(%rip)        # 0x18005f76e
+   18005ecfb:	add    %al,(%rax)
+   18005ecfd:	add    %al,(%rax)
    18005ecff:	add    %dh,0x6e(%rbp)
    18005ed02:	imul   $0x77,0x6f(%rsi),%ebp
    18005ed06:	outsb  %ds:(%rsi),(%dx)
    18005ed07:	and    %ch,(%rax)
    18005ed09:	insl   (%dx),%es:(%rdi)
    18005ed0a:	(bad)
    18005ed0b:	imul   $0x72657620,0x2c(%ebx),%esp
@@ -119153,32 +119159,30 @@
    180063089:	jae    0x1800630b8
    18006308b:	jb     0x180063102
    18006308d:	outsb  %ds:(%rsi),(%dx)
    18006308e:	outsb  %ds:(%rsi),(%dx)
    18006308f:	gs jb  0x1800630ee
    180063092:	(bad)
    180063097:	sub    $0x6c697562,%eax
-   18006309c:	fs pop %rsp
-   18006309e:	pop    %rdi
-   18006309f:	ja     0x180063110
-   1800630a1:	jb     0x18006310e
-   1800630a3:	pop    %rsp
-   1800630a4:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   1800630ab:	insl   (%dx),%es:(%rdi)
-   1800630ac:	pop    %rsp
-   1800630ad:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   1800630b4:	insl   (%dx),%es:(%rdi)
-   1800630b5:	pop    %rsp
-   1800630b6:	jae    0x18006312a
-   1800630b8:	movsxd 0x67(%rdi,%riz,2),%ebx
-   1800630bc:	insl   (%dx),%es:(%rdi)
-   1800630bd:	insb   (%dx),%es:(%rdi)
-   1800630be:	cs movsxd (%rax),%eax
-   1800630c1:	add    %al,(%rax)
-   1800630c3:	add    %al,(%rax)
+   18006309c:	fs sub $0x5c77656e,%eax
+   1800630a2:	pop    %rdi
+   1800630a3:	ja     0x180063114
+   1800630a5:	jb     0x180063112
+   1800630a7:	pop    %rsp
+   1800630a8:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   1800630af:	insl   (%dx),%es:(%rdi)
+   1800630b0:	pop    %rsp
+   1800630b1:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   1800630b8:	insl   (%dx),%es:(%rdi)
+   1800630b9:	pop    %rsp
+   1800630ba:	jae    0x18006312e
+   1800630bc:	movsxd 0x67(%rdi,%riz,2),%ebx
+   1800630c0:	insl   (%dx),%es:(%rdi)
+   1800630c1:	insb   (%dx),%es:(%rdi)
+   1800630c2:	cs movsxd (%rax),%eax
    1800630c5:	add    %al,(%rax)
    1800630c7:	add    %al,0x47(%rdi)
    1800630ca:	rex.WRB
    1800630cb:	rex.WR pop %rdi
    1800630cd:	push   %r11
    1800630cf:	push   %rbx
    1800630d0:	rex.RB push %r10
@@ -122475,20 +122479,17 @@
    180065200:	enter  $0x5e6,$0x80
    180065204:	add    %eax,(%rax)
    180065206:	add    %al,(%rax)
    180065208:	shl    $1,%dh
    18006520a:	add    $0x180,%eax
    18006520f:	add    %al,(%rax)
    180065211:	add    %al,(%rax)
-   180065213:	add    %bl,(%rsi)
-   180065215:	lods   %ds:(%rsi),%al
-   180065216:	push   %rax
-   180065217:	data16 add %al,(%rax)
-   18006521a:	add    %al,(%rax)
-   18006521c:	or     $0x50000000,%eax
+   180065213:	add    %dl,0x6651fd(%rbp)
+   180065219:	add    %al,(%rax)
+   18006521b:	add    %cl,0x50000000(%rip)        # 0x1d0065221
    180065221:	add    (%rax),%eax
    180065223:	add    %al,-0x7ffff9a2(%rax)
    180065229:	rex.W (bad)
 	...
    18006527f:	add    %dh,%al
    180065281:	(bad)
    180065282:	(bad)
```

## ipex_llm/libs/main-bloom.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x000000014001045c
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Fri May 24 15:02:53 2024
+Time/Date		Sat May 25 15:02:44 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000010800
 SizeOfInitializedData	0000000000008e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000001045c
@@ -25509,17 +25509,20 @@
    140014ab0:	enter  $0x125,$0x40
    140014ab4:	add    %eax,(%rax)
    140014ab6:	add    %al,(%rax)
    140014ab8:	shlb   $1,0x14001(%rip)        # 0x140028abf
    140014abe:	add    %al,(%rax)
    140014ac0:	add    %al,(%rax)
    140014ac2:	add    %al,(%rax)
-   140014ac4:	sbb    $0x6650ac,%eax
-   140014ac9:	add    %al,(%rax)
-   140014acb:	add    %cl,0x20000000(%rip)        # 0x160014ad1
+   140014ac4:	xchg   %eax,%esp
+   140014ac5:	std
+   140014ac6:	push   %rcx
+   140014ac7:	data16 add %al,(%rax)
+   140014aca:	add    %al,(%rax)
+   140014acc:	or     $0x20000000,%eax
    140014ad1:	add    (%rax),%eax
    140014ad3:	add    %cl,%ah
    140014ad5:	push   %rsp
    140014ad6:	add    %eax,(%rax)
    140014ad8:	int3
    140014ad9:	rex add %eax,(%rax)
 	...
```

## ipex_llm/libs/main-chatglm_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x00000001400836cc
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Fri May 24 15:04:27 2024
+Time/Date		Sat May 25 15:03:02 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000087c00
 SizeOfInitializedData	00000000000cbe00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000836cc
@@ -189048,19 +189048,17 @@
    140093f25:	add    %al,(%rax)
    140093f27:	add    %al,(%rax)
    140093f29:	cltd
    140093f2a:	or     %al,0x1(%rax)
    140093f2d:	add    %al,(%rax)
    140093f2f:	add    %al,(%rax)
    140093f31:	add    %al,(%rax)
-   140093f33:	add    %bh,-0x54(%rbx)
-   140093f36:	push   %rax
-   140093f37:	data16 add %al,(%rax)
-   140093f3a:	add    %al,(%rax)
-   140093f3c:	or     $0xcc000000,%eax
+   140093f33:	add    %ah,0x6651fd(%rsi)
+   140093f39:	add    %al,(%rax)
+   140093f3b:	add    %cl,-0x34000000(%rip)        # 0x10c093f41
    140093f41:	add    (%rax),%eax
    140093f43:	add    %dl,-0x6ffff68d(%rax)
    140093f49:	movsxd (%rcx),%ecx
 	...
    140093f7f:	add    %al,0x1400977(%rax)
    140093f85:	add    %al,(%rax)
    140093f87:	add    %al,-0x61(%rbp)
```

## ipex_llm/libs/main-gptneox.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x000000014000ef6c
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Fri May 24 15:02:53 2024
+Time/Date		Sat May 25 15:02:44 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000000f200
 SizeOfInitializedData	0000000000009400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000000ef6c
@@ -24136,17 +24136,20 @@
    140013edf:	add    %ch,%al
    140013ee1:	adc    $0x14001,%eax
    140013ee6:	add    %al,(%rax)
    140013ee8:	lock adc $0x14001,%eax
    140013eee:	add    %al,(%rax)
    140013ef0:	add    %al,(%rax)
    140013ef2:	add    %al,(%rax)
-   140013ef4:	sbb    $0x6650ac,%eax
-   140013ef9:	add    %al,(%rax)
-   140013efb:	add    %cl,-0x70000000(%rip)        # 0xd0013f01
+   140013ef4:	xchg   %eax,%esp
+   140013ef5:	std
+   140013ef6:	push   %rcx
+   140013ef7:	data16 add %al,(%rax)
+   140013efa:	add    %al,(%rax)
+   140013efc:	or     $0x90000000,%eax
    140013f01:	add    (%rax),%eax
    140013f03:	add    %ch,0x1(%rcx,%rcx,2)
    140013f07:	add    %ch,0x1(%rdi,%rbp,1)
 	...
    140013f7f:	add    %ah,(%rax)
    140013f81:	add    %r8,0x1(%r8)
    140013f85:	add    %al,(%rax)
```

## ipex_llm/libs/main-llama.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x000000014000f32c
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Fri May 24 15:02:53 2024
+Time/Date		Sat May 25 15:02:44 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000000f600
 SizeOfInitializedData	0000000000009400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000000f32c
@@ -24679,17 +24679,20 @@
    140013faf:	add    %ch,%al
    140013fb1:	adc    $0x14001,%eax
    140013fb6:	add    %al,(%rax)
    140013fb8:	lock adc $0x14001,%eax
    140013fbe:	add    %al,(%rax)
    140013fc0:	add    %al,(%rax)
    140013fc2:	add    %al,(%rax)
-   140013fc4:	sbb    $0x6650ac,%eax
-   140013fc9:	add    %al,(%rax)
-   140013fcb:	add    %cl,-0x70000000(%rip)        # 0xd0013fd1
+   140013fc4:	xchg   %eax,%esp
+   140013fc5:	std
+   140013fc6:	push   %rcx
+   140013fc7:	data16 add %al,(%rax)
+   140013fca:	add    %al,(%rax)
+   140013fcc:	or     $0x90000000,%eax
    140013fd1:	add    (%rax),%eax
    140013fd3:	add    %ch,%ah
    140013fd5:	add    %rax,(%r8)
    140013fd8:	in     (%dx),%al
    140013fd9:	xor    (%rcx),%eax
 	...
    140013fff:	add    %ah,0x140014d(%rax)
```

## ipex_llm/libs/main-starcoder.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x000000014001a85c
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Fri May 24 15:02:53 2024
+Time/Date		Sat May 25 15:02:44 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000001b000
 SizeOfInitializedData	000000000000bc00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000001a85c
@@ -40341,17 +40341,17 @@
    14001f111:	movb   $0x40,(%rcx)
    14001f114:	add    %eax,(%rax)
    14001f116:	add    %al,(%rax)
    14001f118:	push   $0x14001c6
    14001f11d:	add    %al,(%rax)
    14001f11f:	add    %al,(%rax)
    14001f121:	add    %al,(%rax)
-   14001f123:	add    %bl,0x6650ac(%rip)        # 0x1406841d5
-   14001f129:	add    %al,(%rax)
-   14001f12b:	add    %cl,0x20000000(%rip)        # 0x16001f131
+   14001f123:	add    %dl,0x6651(%rbp,%rdi,8)
+   14001f12a:	add    %al,(%rax)
+   14001f12c:	or     $0x20000000,%eax
    14001f131:	add    (%rax),%eax
    14001f133:	add    %dl,(%rbx,%rax,1)
    14001f136:	add    (%rax),%al
    14001f138:	adc    $0xf7,%al
    14001f13a:	add    %eax,(%rax)
 	...
    14001f180:	add    %eax,(%rax)
```

## ipex_llm/libs/quantize-bloom.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140013918
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Fri May 24 15:02:53 2024
+Time/Date		Sat May 25 15:02:44 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000013a00
 SizeOfInitializedData	00000000000ace00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000013918
@@ -31946,32 +31946,30 @@
    140018e89:	jae    0x140018eb8
    140018e8b:	jb     0x140018f02
    140018e8d:	outsb  %ds:(%rsi),(%dx)
    140018e8e:	outsb  %ds:(%rsi),(%dx)
    140018e8f:	gs jb  0x140018eee
    140018e92:	(bad)
    140018e97:	sub    $0x6c697562,%eax
-   140018e9c:	fs pop %rsp
-   140018e9e:	pop    %rdi
-   140018e9f:	ja     0x140018f10
-   140018ea1:	jb     0x140018f0e
-   140018ea3:	pop    %rsp
-   140018ea4:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   140018eab:	insl   (%dx),%es:(%rdi)
-   140018eac:	pop    %rsp
-   140018ead:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   140018eb4:	insl   (%dx),%es:(%rdi)
-   140018eb5:	pop    %rsp
-   140018eb6:	jae    0x140018f2a
-   140018eb8:	movsxd 0x67(%rdi,%riz,2),%ebx
-   140018ebc:	insl   (%dx),%es:(%rdi)
-   140018ebd:	insb   (%dx),%es:(%rdi)
-   140018ebe:	cs movsxd (%rax),%eax
-   140018ec1:	add    %al,(%rax)
-   140018ec3:	add    %al,(%rax)
+   140018e9c:	fs sub $0x5c77656e,%eax
+   140018ea2:	pop    %rdi
+   140018ea3:	ja     0x140018f14
+   140018ea5:	jb     0x140018f12
+   140018ea7:	pop    %rsp
+   140018ea8:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   140018eaf:	insl   (%dx),%es:(%rdi)
+   140018eb0:	pop    %rsp
+   140018eb1:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   140018eb8:	insl   (%dx),%es:(%rdi)
+   140018eb9:	pop    %rsp
+   140018eba:	jae    0x140018f2e
+   140018ebc:	movsxd 0x67(%rdi,%riz,2),%ebx
+   140018ec0:	insl   (%dx),%es:(%rdi)
+   140018ec1:	insb   (%dx),%es:(%rdi)
+   140018ec2:	cs movsxd (%rax),%eax
    140018ec5:	add    %al,(%rax)
    140018ec7:	add    %al,0x47(%rdi)
    140018eca:	rex.WRB
    140018ecb:	rex.WR pop %rdi
    140018ecd:	push   %r11
    140018ecf:	push   %rbx
    140018ed0:	rex.RB push %r10
@@ -32234,17 +32232,17 @@
    140019225:	add    %al,(%rax)
    140019227:	add    %al,(%rax)
    140019229:	push   %rbp
    14001922a:	add    %eax,0x1(%rax)
    14001922d:	add    %al,(%rax)
    14001922f:	add    %al,(%rax)
    140019231:	add    %al,(%rax)
-   140019233:	add    %bl,0x6650ac(%rip)        # 0x14067e2e5
-   140019239:	add    %al,(%rax)
-   14001923b:	add    %cl,0x20000000(%rip)        # 0x160019241
+   140019233:	add    %dl,0x6651(%rbp,%rdi,8)
+   14001923a:	add    %al,(%rax)
+   14001923c:	or     $0x20000000,%eax
    140019241:	add    (%rax),%eax
    140019243:	add    %dh,%al
    140019245:	movabs 0x18ff00001,%eax
 	...
    14001927e:	add    %al,(%rax)
    140019280:	add    %eax,(%rax)
 	...
```

## ipex_llm/libs/quantize-bloom_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140013b28
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Fri May 24 15:03:59 2024
+Time/Date		Sat May 25 15:02:34 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000013c00
 SizeOfInitializedData	00000000000ad000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000013b28
@@ -32374,19 +32374,17 @@
    140019205:	add    %al,(%rax)
    140019207:	add    %al,(%rax)
    140019209:	push   %rbp
    14001920a:	add    %eax,0x1(%rax)
    14001920d:	add    %al,(%rax)
    14001920f:	add    %al,(%rax)
    140019211:	add    %al,(%rax)
-   140019213:	add    %bl,-0x54(%rdi)
-   140019216:	push   %rax
-   140019217:	data16 add %al,(%rax)
-   14001921a:	add    %al,(%rax)
-   14001921c:	or     $0x20000000,%eax
+   140019213:	add    %cl,0x6651fd(%rdx)
+   140019219:	add    %al,(%rax)
+   14001921b:	add    %cl,0x20000000(%rip)        # 0x160019221
    140019221:	add    (%rax),%eax
    140019223:	add    %dh,%al
    140019225:	movabs 0x191f00001,%eax
 	...
    14001927e:	add    %al,(%rax)
    140019280:	add    %eax,(%rax)
 	...
```

## ipex_llm/libs/quantize-gptneox.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140010988
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Fri May 24 15:02:52 2024
+Time/Date		Sat May 25 15:02:43 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000010a00
 SizeOfInitializedData	00000000000aa600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000010988
@@ -13303,15 +13303,15 @@
    14000aab0:	xor    %rsp,%rax
    14000aab3:	mov    %rax,0x50(%rsp)
    14000aab8:	mov    %r9,%rbp
    14000aabb:	mov    %r8,%rsi
    14000aabe:	mov    %rdx,%rbx
    14000aac1:	mov    %rcx,%rdi
    14000aac4:	mov    %rcx,0x28(%rsp)
-   14000aac9:	lea    0xaf10(%rip),%r8        # 0x1400159e0
+   14000aac9:	lea    0xaf14(%rip),%r8        # 0x1400159e4
    14000aad0:	call   0x14000a930
    14000aad5:	nop
    14000aad6:	movl   $0xc470,0x14(%rdi)
    14000aadd:	movl   $0x1000,0x18(%rdi)
    14000aae4:	movl   $0x1400,0x1c(%rdi)
    14000aaeb:	movl   $0x28,0x20(%rdi)
    14000aaf2:	movl   $0x24,0x24(%rdi)
@@ -26105,32 +26105,30 @@
    140015409:	jae    0x140015438
    14001540b:	jb     0x140015482
    14001540d:	outsb  %ds:(%rsi),(%dx)
    14001540e:	outsb  %ds:(%rsi),(%dx)
    14001540f:	gs jb  0x14001546e
    140015412:	(bad)
    140015417:	sub    $0x6c697562,%eax
-   14001541c:	fs pop %rsp
-   14001541e:	pop    %rdi
-   14001541f:	ja     0x140015490
-   140015421:	jb     0x14001548e
-   140015423:	pop    %rsp
-   140015424:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   14001542b:	insl   (%dx),%es:(%rdi)
-   14001542c:	pop    %rsp
-   14001542d:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   140015434:	insl   (%dx),%es:(%rdi)
-   140015435:	pop    %rsp
-   140015436:	jae    0x1400154aa
-   140015438:	movsxd 0x67(%rdi,%riz,2),%ebx
-   14001543c:	insl   (%dx),%es:(%rdi)
-   14001543d:	insb   (%dx),%es:(%rdi)
-   14001543e:	cs movsxd (%rax),%eax
-   140015441:	add    %al,(%rax)
-   140015443:	add    %al,(%rax)
+   14001541c:	fs sub $0x5c77656e,%eax
+   140015422:	pop    %rdi
+   140015423:	ja     0x140015494
+   140015425:	jb     0x140015492
+   140015427:	pop    %rsp
+   140015428:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   14001542f:	insl   (%dx),%es:(%rdi)
+   140015430:	pop    %rsp
+   140015431:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   140015438:	insl   (%dx),%es:(%rdi)
+   140015439:	pop    %rsp
+   14001543a:	jae    0x1400154ae
+   14001543c:	movsxd 0x67(%rdi,%riz,2),%ebx
+   140015440:	insl   (%dx),%es:(%rdi)
+   140015441:	insb   (%dx),%es:(%rdi)
+   140015442:	cs movsxd (%rax),%eax
    140015445:	add    %al,(%rax)
    140015447:	add    %al,0x47(%rdi)
    14001544a:	rex.WRB
    14001544b:	rex.WR pop %rdi
    14001544d:	push   %r11
    14001544f:	push   %rbx
    140015450:	rex.RB push %r10
@@ -26392,38 +26390,36 @@
    1400156d9:	jae    0x140015708
    1400156db:	jb     0x140015752
    1400156dd:	outsb  %ds:(%rsi),(%dx)
    1400156de:	outsb  %ds:(%rsi),(%dx)
    1400156df:	gs jb  0x14001573e
    1400156e2:	(bad)
    1400156e7:	sub    $0x6c697562,%eax
-   1400156ec:	fs pop %rsp
-   1400156ee:	pop    %rdi
-   1400156ef:	ja     0x140015760
-   1400156f1:	jb     0x14001575e
-   1400156f3:	pop    %rsp
-   1400156f4:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   1400156fb:	insl   (%dx),%es:(%rdi)
-   1400156fc:	pop    %rsp
-   1400156fd:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   140015704:	insl   (%dx),%es:(%rdi)
-   140015705:	pop    %rsp
-   140015706:	jae    0x14001577a
-   140015708:	movsxd 0x70(%rdi,%riz,2),%ebx
-   14001570c:	je     0x14001577c
-   14001570e:	outsl  %gs:(%rsi),(%dx)
-   140015710:	js     0x14001576e
-   140015712:	addr32 jo 0x140015789
-   140015715:	outsb  %ds:(%rsi),(%dx)
-   140015716:	outsl  %gs:(%rsi),(%dx)
-   140015718:	js     0x140015747
-   14001571a:	jne    0x140015790
-   14001571c:	imul   $0x0,0x68(%rsi,%rbp,1),%ebp
-   140015724:	add    %al,(%rax)
-   140015726:	add    %al,(%rax)
+   1400156ec:	fs sub $0x5c77656e,%eax
+   1400156f2:	pop    %rdi
+   1400156f3:	ja     0x140015764
+   1400156f5:	jb     0x140015762
+   1400156f7:	pop    %rsp
+   1400156f8:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   1400156ff:	insl   (%dx),%es:(%rdi)
+   140015700:	pop    %rsp
+   140015701:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   140015708:	insl   (%dx),%es:(%rdi)
+   140015709:	pop    %rsp
+   14001570a:	jae    0x14001577e
+   14001570c:	movsxd 0x70(%rdi,%riz,2),%ebx
+   140015710:	je     0x140015780
+   140015712:	outsl  %gs:(%rsi),(%dx)
+   140015714:	js     0x140015772
+   140015716:	addr32 jo 0x14001578d
+   140015719:	outsb  %ds:(%rsi),(%dx)
+   14001571a:	outsl  %gs:(%rsi),(%dx)
+   14001571c:	js     0x14001574b
+   14001571e:	jne    0x140015794
+   140015720:	imul   $0x0,0x68(%rsi,%rbp,1),%ebp
    140015728:	rex.RXB push %r8
    14001572a:	push   %rsp
    14001572b:	rex.WRX
    14001572c:	rex.RB
    14001572d:	rex.WRXB pop %r8
    14001572f:	pop    %rdi
    140015730:	push   %r11
@@ -26652,39 +26648,37 @@
    140015999:	jae    0x1400159c8
    14001599b:	jb     0x140015a12
    14001599d:	outsb  %ds:(%rsi),(%dx)
    14001599e:	outsb  %ds:(%rsi),(%dx)
    14001599f:	gs jb  0x1400159fe
    1400159a2:	(bad)
    1400159a7:	sub    $0x6c697562,%eax
-   1400159ac:	fs pop %rsp
-   1400159ae:	pop    %rdi
-   1400159af:	ja     0x140015a20
-   1400159b1:	jb     0x140015a1e
-   1400159b3:	pop    %rsp
-   1400159b4:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   1400159bb:	insl   (%dx),%es:(%rdi)
-   1400159bc:	pop    %rsp
-   1400159bd:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   1400159c4:	insl   (%dx),%es:(%rdi)
-   1400159c5:	pop    %rsp
-   1400159c6:	jae    0x140015a3a
-   1400159c8:	movsxd 0x70(%rdi,%riz,2),%ebx
-   1400159cc:	je     0x140015a3c
-   1400159ce:	outsl  %gs:(%rsi),(%dx)
-   1400159d0:	js     0x140015a2e
-   1400159d2:	addr32 jo 0x140015a49
-   1400159d5:	outsb  %ds:(%rsi),(%dx)
-   1400159d6:	outsl  %gs:(%rsi),(%dx)
-   1400159d8:	js     0x140015a08
-   1400159da:	movsxd 0x70(%rax),%esi
-   1400159dd:	add    %al,(%rax)
-   1400159df:	add    %dh,0x62(%rdx)
-   1400159e2:	add    %al,(%rax)
-   1400159e4:	add    %al,(%rax)
+   1400159ac:	fs sub $0x5c77656e,%eax
+   1400159b2:	pop    %rdi
+   1400159b3:	ja     0x140015a24
+   1400159b5:	jb     0x140015a22
+   1400159b7:	pop    %rsp
+   1400159b8:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   1400159bf:	insl   (%dx),%es:(%rdi)
+   1400159c0:	pop    %rsp
+   1400159c1:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   1400159c8:	insl   (%dx),%es:(%rdi)
+   1400159c9:	pop    %rsp
+   1400159ca:	jae    0x140015a3e
+   1400159cc:	movsxd 0x70(%rdi,%riz,2),%ebx
+   1400159d0:	je     0x140015a40
+   1400159d2:	outsl  %gs:(%rsi),(%dx)
+   1400159d4:	js     0x140015a32
+   1400159d6:	addr32 jo 0x140015a4d
+   1400159d9:	outsb  %ds:(%rsi),(%dx)
+   1400159da:	outsl  %gs:(%rsi),(%dx)
+   1400159dc:	js     0x140015a0c
+   1400159de:	movsxd 0x70(%rax),%esi
+   1400159e1:	add    %al,(%rax)
+   1400159e3:	add    %dh,0x62(%rdx)
    1400159e6:	add    %al,(%rax)
    1400159e8:	(bad)
    1400159ed:	sub    $0x3a6d6c6c,%eax
    1400159f2:	and    %ch,0x61(%rdi,%rbp,2)
    1400159f6:	imul   $0x646f6d20,%fs:0x67(%rsi),%ebp
    1400159fe:	gs insb (%dx),%es:(%rdi)
    140015a00:	and    %ah,0x72(%rsi)
@@ -27181,19 +27175,17 @@
    140016020:	push   $0x1400123
    140016025:	add    %al,(%rax)
    140016027:	add    %dh,0x23(%rax)
    14001602a:	add    %eax,0x1(%rax)
    14001602d:	add    %al,(%rax)
    14001602f:	add    %al,(%rax)
    140016031:	add    %al,(%rax)
-   140016033:	add    %bl,(%rsp,%rbp,4)
-   140016036:	push   %rax
-   140016037:	data16 add %al,(%rax)
-   14001603a:	add    %al,(%rax)
-   14001603c:	or     $0x90000000,%eax
+   140016033:	add    %dl,0x6651fd(%rbx)
+   140016039:	add    %al,(%rax)
+   14001603b:	add    %cl,-0x70000000(%rip)        # 0xd0016041
    140016041:	add    (%rax),%eax
    140016043:	add    %ch,%al
    140016045:	add    %eax,%gs:(%rax)
    140016048:	call   0x1400161a0
 	...
    14001607d:	add    %al,(%rax)
    14001607f:	add    %bl,0x1400169(%rax)
```

## ipex_llm/libs/quantize-gptneox_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140010b98
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Fri May 24 15:03:58 2024
+Time/Date		Sat May 25 15:02:34 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000010c00
 SizeOfInitializedData	00000000000aa600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000010b98
@@ -27317,19 +27317,17 @@
    140016000:	push   $0x1400123
    140016005:	add    %al,(%rax)
    140016007:	add    %dh,0x23(%rax)
    14001600a:	add    %eax,0x1(%rax)
    14001600d:	add    %al,(%rax)
    14001600f:	add    %al,(%rax)
    140016011:	add    %al,(%rax)
-   140016013:	add    %bl,-0x54(%rsi)
-   140016016:	push   %rax
-   140016017:	data16 add %al,(%rax)
-   14001601a:	add    %al,(%rax)
-   14001601c:	or     $0x90000000,%eax
+   140016013:	add    %cl,0x6651fd(%rdx)
+   140016019:	add    %al,(%rax)
+   14001601b:	add    %cl,-0x70000000(%rip)        # 0xd0016021
    140016021:	add    (%rax),%eax
    140016023:	add    %ch,%al
    140016025:	add    %eax,%gs:(%rax)
    140016028:	call   0x140016182
 	...
    14001607d:	add    %al,(%rax)
    14001607f:	add    %bl,0x1400169(%rax)
```

## ipex_llm/libs/quantize-llama.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x00000001400118e8
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Fri May 24 15:02:52 2024
+Time/Date		Sat May 25 15:02:43 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000011800
 SizeOfInitializedData	00000000000aac00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000118e8
@@ -2917,27 +2917,27 @@
 	reloc   26 offset  f90 [15f90] DIR64
 	reloc   27 offset  f98 [15f98] DIR64
 
 Virtual Address: 00016000 Chunk size 48 (0x30) Number of fixups 20
 	reloc    0 offset  788 [16788] DIR64
 	reloc    1 offset  790 [16790] DIR64
 	reloc    2 offset  798 [16798] DIR64
-	reloc    3 offset  900 [16900] DIR64
-	reloc    4 offset  908 [16908] DIR64
-	reloc    5 offset  910 [16910] DIR64
-	reloc    6 offset  918 [16918] DIR64
-	reloc    7 offset  920 [16920] DIR64
-	reloc    8 offset  928 [16928] DIR64
-	reloc    9 offset  930 [16930] DIR64
-	reloc   10 offset  938 [16938] DIR64
-	reloc   11 offset  940 [16940] DIR64
-	reloc   12 offset  948 [16948] DIR64
-	reloc   13 offset  950 [16950] DIR64
-	reloc   14 offset  958 [16958] DIR64
-	reloc   15 offset  960 [16960] DIR64
+	reloc    3 offset  908 [16908] DIR64
+	reloc    4 offset  910 [16910] DIR64
+	reloc    5 offset  918 [16918] DIR64
+	reloc    6 offset  920 [16920] DIR64
+	reloc    7 offset  928 [16928] DIR64
+	reloc    8 offset  930 [16930] DIR64
+	reloc    9 offset  938 [16938] DIR64
+	reloc   10 offset  940 [16940] DIR64
+	reloc   11 offset  948 [16948] DIR64
+	reloc   12 offset  950 [16950] DIR64
+	reloc   13 offset  958 [16958] DIR64
+	reloc   14 offset  960 [16960] DIR64
+	reloc   15 offset  968 [16968] DIR64
 	reloc   16 offset  f90 [16f90] DIR64
 	reloc   17 offset  f98 [16f98] DIR64
 	reloc   18 offset  fa0 [16fa0] DIR64
 	reloc   19 offset  fa8 [16fa8] DIR64
 
 Virtual Address: 00017000 Chunk size 36 (0x24) Number of fixups 14
 	reloc    0 offset   18 [17018] DIR64
@@ -14100,15 +14100,15 @@
    14000b5f4:	mov    %rax,(%rcx)
    14000b5f7:	lea    0x8(%rcx),%rdx
    14000b5fb:	mov    %rcx,%rdi
    14000b5fe:	vpxor  %xmm0,%xmm0,%xmm0
    14000b602:	lea    0x8(%rbx),%rcx
    14000b606:	vmovups %xmm0,(%rdx)
    14000b60a:	call   0x140011eb0
-   14000b60f:	lea    0xb2f2(%rip),%rax        # 0x140016908
+   14000b60f:	lea    0xb2fa(%rip),%rax        # 0x140016910
    14000b616:	mov    %rax,(%rdi)
    14000b619:	mov    %rdi,%rax
    14000b61c:	vmovups 0x18(%rbx),%xmm0
    14000b621:	mov    0x30(%rsp),%rbx
    14000b626:	vmovups %xmm0,0x18(%rdi)
    14000b62b:	add    $0x20,%rsp
    14000b62f:	pop    %rdi
@@ -14147,52 +14147,52 @@
    14000b67d:	mov    %rax,%rcx
    14000b680:	call   *0x7cb2(%rip)        # 0x140013338
    14000b686:	test   %eax,%eax
    14000b688:	je     0x14000b6c4
    14000b68a:	mov    $0x2,%ecx
    14000b68f:	call   *0x7c9b(%rip)        # 0x140013330
    14000b695:	mov    %rax,%rcx
-   14000b698:	lea    0xb1c9(%rip),%rax        # 0x140016868
+   14000b698:	lea    0xb1d1(%rip),%rax        # 0x140016870
    14000b69f:	mov    %rax,0x20(%rsp)
    14000b6a4:	mov    $0x65,%r9d
    14000b6aa:	lea    0xb10f(%rip),%r8        # 0x1400167c0
-   14000b6b1:	lea    0xb158(%rip),%rdx        # 0x140016810
+   14000b6b1:	lea    0xb160(%rip),%rdx        # 0x140016818
    14000b6b8:	call   0x140002470
    14000b6bd:	call   *0x7bf5(%rip)        # 0x1400132b8
    14000b6c3:	int3
    14000b6c4:	mov    (%rbx),%rcx
    14000b6c7:	call   *0x7c5b(%rip)        # 0x140013328
    14000b6cd:	cmp    $0xffffffffffffffff,%rax
    14000b6d1:	jne    0x14000b70b
    14000b6d3:	lea    0x3(%rax),%ecx
    14000b6d6:	call   *0x7c54(%rip)        # 0x140013330
    14000b6dc:	mov    %rax,%rcx
-   14000b6df:	lea    0xb172(%rip),%rax        # 0x140016858
+   14000b6df:	lea    0xb17a(%rip),%rax        # 0x140016860
    14000b6e6:	mov    %rax,0x20(%rsp)
    14000b6eb:	mov    $0x5b,%r9d
    14000b6f1:	lea    0xb0c8(%rip),%r8        # 0x1400167c0
-   14000b6f8:	lea    0xb111(%rip),%rdx        # 0x140016810
+   14000b6f8:	lea    0xb119(%rip),%rdx        # 0x140016818
    14000b6ff:	call   0x140002470
    14000b704:	call   *0x7bae(%rip)        # 0x1400132b8
    14000b70a:	int3
    14000b70b:	mov    %rax,0x8(%rbx)
    14000b70f:	xor    %r8d,%r8d
    14000b712:	xor    %edx,%edx
    14000b714:	mov    (%rbx),%rcx
    14000b717:	call   *0x7c1b(%rip)        # 0x140013338
    14000b71d:	test   %eax,%eax
    14000b71f:	je     0x14000b75b
    14000b721:	mov    $0x2,%ecx
    14000b726:	call   *0x7c04(%rip)        # 0x140013330
    14000b72c:	mov    %rax,%rcx
-   14000b72f:	lea    0xb132(%rip),%rax        # 0x140016868
+   14000b72f:	lea    0xb13a(%rip),%rax        # 0x140016870
    14000b736:	mov    %rax,0x20(%rsp)
    14000b73b:	mov    $0x65,%r9d
    14000b741:	lea    0xb078(%rip),%r8        # 0x1400167c0
-   14000b748:	lea    0xb0c1(%rip),%rdx        # 0x140016810
+   14000b748:	lea    0xb0c9(%rip),%rdx        # 0x140016818
    14000b74f:	call   0x140002470
    14000b754:	call   *0x7b5e(%rip)        # 0x1400132b8
    14000b75a:	int3
    14000b75b:	mov    %rbx,%rax
    14000b75e:	mov    0x68(%rsp),%rcx
    14000b763:	xor    %rsp,%rcx
    14000b766:	call   0x1400113d0
@@ -14201,15 +14201,15 @@
    14000b777:	pop    %rdi
    14000b778:	ret
    14000b779:	call   *0x7ac1(%rip)        # 0x140013240
    14000b77f:	mov    (%rax),%ecx
    14000b781:	call   *0x7b01(%rip)        # 0x140013288
    14000b787:	mov    %rax,%r9
    14000b78a:	mov    %rdi,%r8
-   14000b78d:	lea    0xb0ac(%rip),%rdx        # 0x140016840
+   14000b78d:	lea    0xb0b4(%rip),%rdx        # 0x140016848
    14000b794:	lea    0x48(%rsp),%rcx
    14000b799:	call   0x14000dc10
    14000b79e:	nop
    14000b79f:	mov    %rax,%rdx
    14000b7a2:	lea    0x30(%rsp),%rcx
    14000b7a7:	call   0x14000c1c0
    14000b7ac:	lea    0xdb5d(%rip),%rdx        # 0x140019310
@@ -14227,15 +14227,15 @@
    14000b7d0:	xor    %rsp,%rax
    14000b7d3:	mov    %rax,0x50(%rsp)
    14000b7d8:	mov    %r9,%rbp
    14000b7db:	mov    %r8,%rsi
    14000b7de:	mov    %rdx,%rbx
    14000b7e1:	mov    %rcx,%rdi
    14000b7e4:	mov    %rcx,0x28(%rsp)
-   14000b7e9:	lea    0xb2bc(%rip),%r8        # 0x140016aac
+   14000b7e9:	lea    0xb2c0(%rip),%r8        # 0x140016ab0
    14000b7f0:	call   0x14000b640
    14000b7f5:	nop
    14000b7f6:	movl   $0x7d00,0x14(%rdi)
    14000b7fd:	movl   $0x200,0x18(%rdi)
    14000b804:	movl   $0x1000,0x1c(%rdi)
    14000b80b:	movl   $0x100,0x20(%rdi)
    14000b812:	movl   $0x20,0x24(%rdi)
@@ -14246,15 +14246,15 @@
    14000b835:	lea    0x38(%rdi),%rcx
    14000b839:	call   0x14000c0f0
    14000b83e:	nop
    14000b83f:	mov    $0x2,%ecx
    14000b844:	call   *0x7ae6(%rip)        # 0x140013330
    14000b84a:	mov    %rax,%rcx
    14000b84d:	mov    %rbx,%r8
-   14000b850:	lea    0xb259(%rip),%rdx        # 0x140016ab0
+   14000b850:	lea    0xb261(%rip),%rdx        # 0x140016ab8
    14000b857:	call   0x140002470
    14000b85c:	mov    $0x4,%r8d
    14000b862:	lea    0x20(%rsp),%rdx
    14000b867:	mov    %rdi,%rcx
    14000b86a:	call   0x14000fa20
    14000b86f:	mov    0x20(%rsp),%ebx
    14000b873:	cmp    $0x67676d6c,%ebx
@@ -14739,27 +14739,27 @@
    14000bfc0:	sub    (%r10),%rax
    14000bfc3:	sar    $0x2,%rax
    14000bfc7:	cmp    $0x1,%rax
    14000bfcb:	je     0x14000c02c
    14000bfcd:	cmp    $0x1,%rdx
    14000bfd1:	je     0x14000c02c
    14000bfd3:	xor    %r8d,%r8d
-   14000bfd6:	lea    0xa9cb(%rip),%rdx        # 0x1400169a8
+   14000bfd6:	lea    0xa9d3(%rip),%rdx        # 0x1400169b0
    14000bfdd:	mov    %rbx,%rcx
    14000bfe0:	call   0x14000db10
    14000bfe5:	test   %rax,%rax
    14000bfe8:	je     0x14000c023
    14000bfea:	xor    %r8d,%r8d
-   14000bfed:	lea    0xa9c4(%rip),%rdx        # 0x1400169b8
+   14000bfed:	lea    0xa9cc(%rip),%rdx        # 0x1400169c0
    14000bff4:	mov    %rbx,%rcx
    14000bff7:	call   0x14000db10
    14000bffc:	cmp    $0xffffffffffffffff,%rax
    14000c000:	jne    0x14000c023
    14000c002:	xor    %r8d,%r8d
-   14000c005:	lea    0xa9c4(%rip),%rdx        # 0x1400169d0
+   14000c005:	lea    0xa9cc(%rip),%rdx        # 0x1400169d8
    14000c00c:	mov    %rbx,%rcx
    14000c00f:	call   0x14000db10
    14000c014:	cmp    $0xffffffffffffffff,%rax
    14000c018:	jne    0x14000c023
    14000c01a:	movl   $0x2,0x24(%rbx)
    14000c021:	jmp    0x14000c033
    14000c023:	movl   $0x1,0x24(%rbx)
@@ -14788,15 +14788,15 @@
    14000c082:	pop    %rdi
    14000c083:	pop    %rsi
    14000c084:	pop    %rbp
    14000c085:	ret
    14000c086:	lea    0x18(%rdi),%rcx
    14000c08a:	call   0x14000d690
    14000c08f:	mov    %rax,%r8
-   14000c092:	lea    0xa8e7(%rip),%rdx        # 0x140016980
+   14000c092:	lea    0xa8ef(%rip),%rdx        # 0x140016988
    14000c099:	lea    -0x21(%rbp),%rcx
    14000c09d:	call   0x14000dc10
    14000c0a2:	lea    0xd337(%rip),%rdx        # 0x1400193e0
    14000c0a9:	lea    -0x21(%rbp),%rcx
    14000c0ad:	call   0x140011ebc
    14000c0b2:	int3
    14000c0b3:	call   0x14000d590
@@ -14928,17 +14928,17 @@
    14000c234:	mov    %rax,(%rcx)
    14000c237:	lea    0x8(%rcx),%rdx
    14000c23b:	mov    %rcx,%rdi
    14000c23e:	vpxor  %xmm0,%xmm0,%xmm0
    14000c242:	lea    0x8(%rbx),%rcx
    14000c246:	vmovups %xmm0,(%rdx)
    14000c24a:	call   0x140011eb0
-   14000c24f:	lea    0xa6b2(%rip),%rax        # 0x140016908
+   14000c24f:	lea    0xa6ba(%rip),%rax        # 0x140016910
    14000c256:	mov    %rax,(%rdi)
-   14000c259:	lea    0xa6c0(%rip),%rax        # 0x140016920
+   14000c259:	lea    0xa6c8(%rip),%rax        # 0x140016928
    14000c260:	vmovups 0x18(%rbx),%xmm0
    14000c265:	mov    0x30(%rsp),%rbx
    14000c26a:	mov    %rax,(%rdi)
    14000c26d:	mov    %rdi,%rax
    14000c270:	vmovups %xmm0,0x18(%rdi)
    14000c275:	add    $0x20,%rsp
    14000c279:	pop    %rdi
@@ -14990,15 +14990,15 @@
    14000c325:	add    $0xfffffffffffffff8,%rax
    14000c329:	cmp    $0x1f,%rax
    14000c32d:	jbe    0x14000c336
    14000c32f:	call   *0x6f03(%rip)        # 0x140013238
    14000c335:	int3
    14000c336:	call   0x1400110e4
    14000c33b:	vmovups (%rdi),%xmm0
-   14000c33f:	lea    0xa5da(%rip),%rax        # 0x140016920
+   14000c33f:	lea    0xa5e2(%rip),%rax        # 0x140016928
    14000c346:	mov    %rax,(%rbx)
    14000c349:	mov    %rbx,%rax
    14000c34c:	vmovups %xmm0,0x18(%rbx)
    14000c351:	mov    0x50(%rsp),%rcx
    14000c356:	xor    %rsp,%rcx
    14000c359:	call   0x1400113d0
    14000c35e:	mov    0x80(%rsp),%rbx
@@ -15891,15 +15891,15 @@
    14000cdc7:	cmpq   $0x10,0x18(%rax)
    14000cdcc:	jb     0x14000cdd1
    14000cdce:	mov    (%rax),%rbx
    14000cdd1:	mov    $0x2,%ecx
    14000cdd6:	call   *0x6554(%rip)        # 0x140013330
    14000cddc:	mov    %rax,%rcx
    14000cddf:	mov    %rbx,%r8
-   14000cde2:	lea    0x9aef(%rip),%rdx        # 0x1400168d8
+   14000cde2:	lea    0x9af7(%rip),%rdx        # 0x1400168e0
    14000cde9:	call   0x140002470
    14000cdee:	mov    0x38(%rsp),%rdx
    14000cdf3:	cmp    $0x10,%rdx
    14000cdf7:	jb     0x14000ce2f
    14000cdf9:	inc    %rdx
    14000cdfc:	mov    0x20(%rsp),%rcx
    14000ce01:	mov    %rcx,%rax
@@ -16639,15 +16639,15 @@
    14000d786:	mov    $0x2,%ecx
    14000d78b:	call   *0x5b9f(%rip)        # 0x140013330
    14000d791:	mov    %rax,%rcx
    14000d794:	lea    0x929d(%rip),%rax        # 0x140016a38
    14000d79b:	mov    %rax,0x20(%rsp)
    14000d7a0:	mov    $0x187,%r9d
    14000d7a6:	lea    0x92b3(%rip),%r8        # 0x140016a60
-   14000d7ad:	lea    0x905c(%rip),%rdx        # 0x140016810
+   14000d7ad:	lea    0x9064(%rip),%rdx        # 0x140016818
    14000d7b4:	call   0x140002470
    14000d7b9:	call   *0x5af9(%rip)        # 0x1400132b8
    14000d7bf:	int3
    14000d7c0:	mov    0x3c(%r14),%ecx
    14000d7c4:	test   %ecx,%ecx
    14000d7c6:	je     0x14000d825
    14000d7c8:	sub    $0x1,%ecx
@@ -17102,19 +17102,19 @@
    14000dd24:	mov    %r14,%rcx
    14000dd27:	call   0x140010f20
    14000dd2c:	cmp    %r15d,%eax
    14000dd2f:	je     0x14000dd6b
    14000dd31:	mov    $0x2,%ecx
    14000dd36:	call   *0x55f4(%rip)        # 0x140013330
    14000dd3c:	mov    %rax,%rcx
-   14000dd3f:	lea    0x8aea(%rip),%rax        # 0x140016830
+   14000dd3f:	lea    0x8af2(%rip),%rax        # 0x140016838
    14000dd46:	mov    %rax,0x20(%rsp)
    14000dd4b:	mov    $0x40,%r9d
    14000dd51:	lea    0x8a68(%rip),%r8        # 0x1400167c0
-   14000dd58:	lea    0x8ab1(%rip),%rdx        # 0x140016810
+   14000dd58:	lea    0x8ab9(%rip),%rdx        # 0x140016818
    14000dd5f:	call   0x140002470
    14000dd64:	call   *0x554e(%rip)        # 0x1400132b8
    14000dd6a:	int3
    14000dd6b:	vpxor  %xmm0,%xmm0,%xmm0
    14000dd6f:	vmovups %xmm0,0x0(%rbp)
    14000dd74:	mov    %r12,0x10(%rbp)
    14000dd78:	mov    %r12,0x18(%rbp)
@@ -17154,15 +17154,15 @@
    14000ddda:	mov    $0x2,%ecx
    14000dddf:	call   *0x554b(%rip)        # 0x140013330
    14000dde5:	mov    %rax,%rcx
    14000dde8:	lea    0x89b1(%rip),%rax        # 0x1400167a0
    14000ddef:	mov    %rax,0x20(%rsp)
    14000ddf4:	mov    $0x3d,%r9d
    14000ddfa:	lea    0x89bf(%rip),%r8        # 0x1400167c0
-   14000de01:	lea    0x8a08(%rip),%rdx        # 0x140016810
+   14000de01:	lea    0x8a10(%rip),%rdx        # 0x140016818
    14000de08:	call   0x140002470
    14000de0d:	call   *0x54a5(%rip)        # 0x1400132b8
    14000de13:	int3
    14000de14:	call   0x140001f20
    14000de19:	int3
    14000de1a:	call   0x14000d570
    14000de1f:	int3
@@ -17377,15 +17377,15 @@
    14000e12c:	mov    %rcx,%rsi
    14000e12f:	sub    %r9,%rax
    14000e132:	mov    %rcx,0x28(%rsp)
    14000e137:	sar    $0x2,%rax
    14000e13b:	test   %rax,%rax
    14000e13e:	je     0x14000e240
    14000e144:	mov    (%r9),%r9d
-   14000e147:	lea    0x8822(%rip),%r8        # 0x140016970
+   14000e147:	lea    0x882a(%rip),%r8        # 0x140016978
    14000e14e:	mov    $0x100,%edx
    14000e153:	lea    0x30(%rsp),%rcx
    14000e158:	call   0x1400099b0
    14000e15d:	mov    0x8(%r14),%rcx
    14000e161:	mov    $0x1,%edi
    14000e166:	mov    (%r14),%r8
    14000e169:	mov    %rcx,%rax
@@ -17404,15 +17404,15 @@
    14000e198:	nopl   0x0(%rax,%rax,1)
    14000e1a0:	inc    %rax
    14000e1a3:	cmpb   $0x0,(%rcx,%rax,1)
    14000e1a7:	jne    0x14000e1a0
    14000e1a9:	mov    (%r8,%rdi,4),%r9d
    14000e1ad:	lea    0x30(%rsp),%rcx
    14000e1b2:	mov    $0x100,%edx
-   14000e1b7:	lea    0x87b6(%rip),%r8        # 0x140016974
+   14000e1b7:	lea    0x87be(%rip),%r8        # 0x14001697c
    14000e1be:	sub    %rax,%rdx
    14000e1c1:	add    %rax,%rcx
    14000e1c4:	call   0x1400099b0
    14000e1c9:	mov    0x8(%r14),%rcx
    14000e1cd:	inc    %rdi
    14000e1d0:	mov    (%r14),%r8
    14000e1d3:	mov    %rcx,%rax
@@ -17482,19 +17482,19 @@
    14000e2b1:	mov    %rdi,0x10(%rbx)
    14000e2b5:	mov    %rbx,%rcx
    14000e2b8:	movq   $0xf,0x18(%rbx)
    14000e2c0:	call   0x140001f80
    14000e2c5:	mov    %rax,(%rbx)
    14000e2c8:	movq   $0x15,0x10(%rbx)
    14000e2d0:	movq   $0x1f,0x18(%rbx)
-   14000e2d8:	vmovups 0x85e0(%rip),%xmm0        # 0x1400168c0
+   14000e2d8:	vmovups 0x85e8(%rip),%xmm0        # 0x1400168c8
    14000e2e0:	vmovups %xmm0,(%rax)
-   14000e2e4:	mov    0x85e6(%rip),%ecx        # 0x1400168d0
+   14000e2e4:	mov    0x85ee(%rip),%ecx        # 0x1400168d8
    14000e2ea:	mov    %ecx,0x10(%rax)
-   14000e2ed:	movzbl 0x85e0(%rip),%ecx        # 0x1400168d4
+   14000e2ed:	movzbl 0x85e8(%rip),%ecx        # 0x1400168dc
    14000e2f4:	mov    %cl,0x14(%rax)
    14000e2f7:	mov    %dil,0x15(%rax)
    14000e2fb:	jmp    0x14000e331
    14000e2fd:	mov    0x40(%rsp),%rdx
    14000e302:	lea    0x50(%rsp),%rcx
    14000e307:	vpxor  %xmm1,%xmm1,%xmm1
    14000e30b:	vmovdqu %xmm1,0x60(%rsp)
@@ -18275,48 +18275,48 @@
    14000ef32:	mov    $0x2,%ecx
    14000ef37:	call   *0x43f3(%rip)        # 0x140013330
    14000ef3d:	mov    %rax,%rcx
    14000ef40:	lea    0x7cc9(%rip),%rax        # 0x140016c10
    14000ef47:	mov    %rax,0x20(%rsp)
    14000ef4c:	mov    $0x25d,%r9d
    14000ef52:	lea    0x7b07(%rip),%r8        # 0x140016a60
-   14000ef59:	lea    0x78b0(%rip),%rdx        # 0x140016810
+   14000ef59:	lea    0x78b8(%rip),%rdx        # 0x140016818
    14000ef60:	call   0x140002470
    14000ef65:	call   *0x434d(%rip)        # 0x1400132b8
    14000ef6b:	int3
    14000ef6c:	mov    $0x2,%ecx
    14000ef71:	call   *0x43b9(%rip)        # 0x140013330
    14000ef77:	mov    %rax,%rcx
-   14000ef7a:	lea    0x78e7(%rip),%rax        # 0x140016868
+   14000ef7a:	lea    0x78ef(%rip),%rax        # 0x140016870
    14000ef81:	mov    %rax,0x20(%rsp)
    14000ef86:	mov    $0x65,%r9d
    14000ef8c:	lea    0x782d(%rip),%r8        # 0x1400167c0
-   14000ef93:	lea    0x7876(%rip),%rdx        # 0x140016810
+   14000ef93:	lea    0x787e(%rip),%rdx        # 0x140016818
    14000ef9a:	call   0x140002470
    14000ef9f:	call   *0x4313(%rip)        # 0x1400132b8
    14000efa5:	int3
    14000efa6:	mov    $0x2,%ecx
    14000efab:	call   *0x437f(%rip)        # 0x140013330
    14000efb1:	mov    %rax,%rcx
-   14000efb4:	lea    0x789d(%rip),%rax        # 0x140016858
+   14000efb4:	lea    0x78a5(%rip),%rax        # 0x140016860
    14000efbb:	mov    %rax,0x20(%rsp)
    14000efc0:	mov    $0x5b,%r9d
    14000efc6:	lea    0x77f3(%rip),%r8        # 0x1400167c0
-   14000efcd:	lea    0x783c(%rip),%rdx        # 0x140016810
+   14000efcd:	lea    0x7844(%rip),%rdx        # 0x140016818
    14000efd4:	call   0x140002470
    14000efd9:	call   *0x42d9(%rip)        # 0x1400132b8
    14000efdf:	int3
    14000efe0:	mov    $0x2,%ecx
    14000efe5:	call   *0x4345(%rip)        # 0x140013330
    14000efeb:	mov    %rax,%rcx
    14000efee:	lea    0x7597(%rip),%rax        # 0x14001658c
    14000eff5:	mov    %rax,0x20(%rsp)
    14000effa:	mov    $0x255,%r9d
    14000f000:	lea    0x7a59(%rip),%r8        # 0x140016a60
-   14000f007:	lea    0x7802(%rip),%rdx        # 0x140016810
+   14000f007:	lea    0x780a(%rip),%rdx        # 0x140016818
    14000f00e:	call   0x140002470
    14000f013:	call   *0x429f(%rip)        # 0x1400132b8
    14000f019:	nop
    14000f01a:	mov    -0x50(%rbp),%rsi
    14000f01e:	jmp    0x14000f039
    14000f020:	mov    0x100(%rbp),%rdi
    14000f027:	mov    0x40(%rsp),%rsi
@@ -18552,15 +18552,15 @@
    14000f378:	mov    $0x2,%ecx
    14000f37d:	call   *0x3fad(%rip)        # 0x140013330
    14000f383:	mov    %rax,%rcx
    14000f386:	lea    0x798b(%rip),%rax        # 0x140016d18
    14000f38d:	mov    %rax,0x20(%rsp)
    14000f392:	mov    $0x2ee,%r9d
    14000f398:	lea    0x76c1(%rip),%r8        # 0x140016a60
-   14000f39f:	lea    0x746a(%rip),%rdx        # 0x140016810
+   14000f39f:	lea    0x7472(%rip),%rdx        # 0x140016818
    14000f3a6:	call   0x140002470
    14000f3ab:	call   *0x3f07(%rip)        # 0x1400132b8
    14000f3b1:	int3
    14000f3b2:	movabs $0x4924924924924925,%rax
    14000f3bc:	imul   %rcx
    14000f3bf:	sar    $0x4,%rdx
    14000f3c3:	mov    %rdx,%rax
@@ -18598,19 +18598,19 @@
    14000f446:	mov    (%rbx),%rcx
    14000f449:	call   *0x3ee9(%rip)        # 0x140013338
    14000f44f:	test   %eax,%eax
    14000f451:	je     0x14000f48d
    14000f453:	mov    $0x2,%ecx
    14000f458:	call   *0x3ed2(%rip)        # 0x140013330
    14000f45e:	mov    %rax,%rcx
-   14000f461:	lea    0x7400(%rip),%rax        # 0x140016868
+   14000f461:	lea    0x7408(%rip),%rax        # 0x140016870
    14000f468:	mov    %rax,0x20(%rsp)
    14000f46d:	mov    $0x65,%r9d
    14000f473:	lea    0x7346(%rip),%r8        # 0x1400167c0
-   14000f47a:	lea    0x738f(%rip),%rdx        # 0x140016810
+   14000f47a:	lea    0x7397(%rip),%rdx        # 0x140016818
    14000f481:	call   0x140002470
    14000f486:	call   *0x3e2c(%rip)        # 0x1400132b8
    14000f48c:	int3
    14000f48d:	mov    0x58(%r14),%r8
    14000f491:	mov    0x68(%r14),%rdx
    14000f495:	mov    %rbx,%rcx
    14000f498:	call   0x14000fa20
@@ -18651,26 +18651,26 @@
    14000f51d:	mov    $0x2,%ecx
    14000f522:	call   *0x3e08(%rip)        # 0x140013330
    14000f528:	mov    %rax,%rcx
    14000f52b:	lea    0x77fe(%rip),%rax        # 0x140016d30
    14000f532:	mov    %rax,0x20(%rsp)
    14000f537:	mov    $0x2fc,%r9d
    14000f53d:	lea    0x751c(%rip),%r8        # 0x140016a60
-   14000f544:	lea    0x72c5(%rip),%rdx        # 0x140016810
+   14000f544:	lea    0x72cd(%rip),%rdx        # 0x140016818
    14000f54b:	call   0x140002470
    14000f550:	call   *0x3d62(%rip)        # 0x1400132b8
    14000f556:	int3
    14000f557:	mov    $0x2,%ecx
    14000f55c:	call   *0x3dce(%rip)        # 0x140013330
    14000f562:	mov    %rax,%rcx
-   14000f565:	lea    0x72fc(%rip),%rax        # 0x140016868
+   14000f565:	lea    0x7304(%rip),%rax        # 0x140016870
    14000f56c:	mov    %rax,0x20(%rsp)
    14000f571:	mov    $0x65,%r9d
    14000f577:	lea    0x7242(%rip),%r8        # 0x1400167c0
-   14000f57e:	lea    0x728b(%rip),%rdx        # 0x140016810
+   14000f57e:	lea    0x7293(%rip),%rdx        # 0x140016818
    14000f585:	call   0x140002470
    14000f58a:	call   *0x3d28(%rip)        # 0x1400132b8
    14000f590:	int3
    14000f591:	cmp    $0x1,%eax
    14000f594:	jne    0x14000f94c
    14000f59a:	mov    0x8(%rdx),%rcx
    14000f59e:	sub    (%rdx),%rcx
@@ -18860,26 +18860,26 @@
    14000f87a:	mov    $0x2,%ecx
    14000f87f:	call   *0x3aab(%rip)        # 0x140013330
    14000f885:	mov    %rax,%rcx
    14000f888:	lea    0x74b9(%rip),%rax        # 0x140016d48
    14000f88f:	mov    %rax,0x20(%rsp)
    14000f894:	mov    $0x313,%r9d
    14000f89a:	lea    0x71bf(%rip),%r8        # 0x140016a60
-   14000f8a1:	lea    0x6f68(%rip),%rdx        # 0x140016810
+   14000f8a1:	lea    0x6f70(%rip),%rdx        # 0x140016818
    14000f8a8:	call   0x140002470
    14000f8ad:	call   *0x3a05(%rip)        # 0x1400132b8
    14000f8b3:	int3
    14000f8b4:	mov    $0x2,%ecx
    14000f8b9:	call   *0x3a71(%rip)        # 0x140013330
    14000f8bf:	mov    %rax,%rcx
-   14000f8c2:	lea    0x6f9f(%rip),%rax        # 0x140016868
+   14000f8c2:	lea    0x6fa7(%rip),%rax        # 0x140016870
    14000f8c9:	mov    %rax,0x20(%rsp)
    14000f8ce:	mov    $0x65,%r9d
    14000f8d4:	lea    0x6ee5(%rip),%r8        # 0x1400167c0
-   14000f8db:	lea    0x6f2e(%rip),%rdx        # 0x140016810
+   14000f8db:	lea    0x6f36(%rip),%rdx        # 0x140016818
    14000f8e2:	call   0x140002470
    14000f8e7:	call   *0x39cb(%rip)        # 0x1400132b8
    14000f8ed:	nop
    14000f8ee:	test   %r12,%r12
    14000f8f1:	je     0x14000f94c
    14000f8f3:	mov    %r12,%rbx
    14000f8f6:	cmp    %rsi,%r12
@@ -18982,15 +18982,15 @@
    14000fa00:	call   0x140001420
    14000fa05:	mov    %rbx,%rax
    14000fa08:	add    $0x30,%rsp
    14000fa0c:	pop    %rbx
    14000fa0d:	ret
    14000fa0e:	int3
    14000fa0f:	int3
-   14000fa10:	lea    0x6f51(%rip),%rax        # 0x140016968
+   14000fa10:	lea    0x6f59(%rip),%rax        # 0x140016970
    14000fa17:	ret
    14000fa18:	int3
    14000fa19:	int3
    14000fa1a:	int3
    14000fa1b:	int3
    14000fa1c:	int3
    14000fa1d:	int3
@@ -19026,30 +19026,30 @@
    14000fa80:	xor    %rsp,%rcx
    14000fa83:	call   0x1400113d0
    14000fa88:	add    $0x60,%rsp
    14000fa8c:	pop    %rdi
    14000fa8d:	pop    %rsi
    14000fa8e:	pop    %rbx
    14000fa8f:	ret
-   14000fa90:	lea    0x6df1(%rip),%rdx        # 0x140016888
+   14000fa90:	lea    0x6df9(%rip),%rdx        # 0x140016890
    14000fa97:	lea    0x38(%rsp),%rcx
    14000fa9c:	call   0x14000b3f0
    14000faa1:	nop
    14000faa2:	mov    %rax,%rdx
    14000faa5:	lea    0x20(%rsp),%rcx
    14000faaa:	call   0x14000c1c0
    14000faaf:	lea    0x985a(%rip),%rdx        # 0x140019310
    14000fab6:	lea    0x20(%rsp),%rcx
    14000fabb:	call   0x140011ebc
    14000fac0:	nop
    14000fac1:	call   *0x3779(%rip)        # 0x140013240
    14000fac7:	mov    (%rax),%ecx
    14000fac9:	call   *0x37b9(%rip)        # 0x140013288
    14000facf:	mov    %rax,%r8
-   14000fad2:	lea    0x6d9f(%rip),%rdx        # 0x140016878
+   14000fad2:	lea    0x6da7(%rip),%rdx        # 0x140016880
    14000fad9:	lea    0x38(%rsp),%rcx
    14000fade:	call   0x14000dc10
    14000fae3:	nop
    14000fae4:	mov    %rax,%rdx
    14000fae7:	lea    0x20(%rsp),%rcx
    14000faec:	call   0x14000c1c0
    14000faf1:	lea    0x9818(%rip),%rdx        # 0x140019310
@@ -19657,69 +19657,69 @@
    140010442:	call   0x1400110e4
    140010447:	mov    -0x48(%rbp),%r12
    14001044b:	mov    (%r12),%rcx
    14001044f:	jmp    0x14000fb50
    140010454:	mov    $0x2,%ecx
    140010459:	call   *0x2ed1(%rip)        # 0x140013330
    14001045f:	mov    %rax,%rcx
-   140010462:	lea    0x63ff(%rip),%rax        # 0x140016868
+   140010462:	lea    0x6407(%rip),%rax        # 0x140016870
    140010469:	mov    %rax,0x20(%rsp)
    14001046e:	mov    $0x65,%r9d
    140010474:	lea    0x6345(%rip),%r8        # 0x1400167c0
-   14001047b:	lea    0x638e(%rip),%rdx        # 0x140016810
+   14001047b:	lea    0x6396(%rip),%rdx        # 0x140016818
    140010482:	call   0x140002470
    140010487:	call   *0x2e2b(%rip)        # 0x1400132b8
    14001048d:	int3
    14001048e:	mov    $0x2,%ecx
    140010493:	call   *0x2e97(%rip)        # 0x140013330
    140010499:	mov    %rax,%rcx
-   14001049c:	lea    0x63b5(%rip),%rax        # 0x140016858
+   14001049c:	lea    0x63bd(%rip),%rax        # 0x140016860
    1400104a3:	mov    %rax,0x20(%rsp)
    1400104a8:	mov    $0x5b,%r9d
    1400104ae:	lea    0x630b(%rip),%r8        # 0x1400167c0
-   1400104b5:	lea    0x6354(%rip),%rdx        # 0x140016810
+   1400104b5:	lea    0x635c(%rip),%rdx        # 0x140016818
    1400104bc:	call   0x140002470
    1400104c1:	call   *0x2df1(%rip)        # 0x1400132b8
    1400104c7:	nop
    1400104c8:	call   *0x2d6a(%rip)        # 0x140013238
    1400104ce:	nop
    1400104cf:	call   *0x2d63(%rip)        # 0x140013238
    1400104d5:	nop
    1400104d6:	call   *0x2d5c(%rip)        # 0x140013238
    1400104dc:	nop
    1400104dd:	mov    $0x2,%ecx
    1400104e2:	call   *0x2e48(%rip)        # 0x140013330
    1400104e8:	mov    %rax,%rcx
-   1400104eb:	lea    0x6376(%rip),%rax        # 0x140016868
+   1400104eb:	lea    0x637e(%rip),%rax        # 0x140016870
    1400104f2:	mov    %rax,0x20(%rsp)
    1400104f7:	mov    $0x65,%r9d
    1400104fd:	lea    0x62bc(%rip),%r8        # 0x1400167c0
-   140010504:	lea    0x6305(%rip),%rdx        # 0x140016810
+   140010504:	lea    0x630d(%rip),%rdx        # 0x140016818
    14001050b:	call   0x140002470
    140010510:	call   *0x2da2(%rip)        # 0x1400132b8
    140010516:	int3
    140010517:	mov    $0x2,%ecx
    14001051c:	call   *0x2e0e(%rip)        # 0x140013330
    140010522:	mov    %rax,%rcx
-   140010525:	lea    0x632c(%rip),%rax        # 0x140016858
+   140010525:	lea    0x6334(%rip),%rax        # 0x140016860
    14001052c:	mov    %rax,0x20(%rsp)
    140010531:	mov    $0x5b,%r9d
    140010537:	lea    0x6282(%rip),%r8        # 0x1400167c0
-   14001053e:	lea    0x62cb(%rip),%rdx        # 0x140016810
+   14001053e:	lea    0x62d3(%rip),%rdx        # 0x140016818
    140010545:	call   0x140002470
    14001054a:	call   *0x2d68(%rip)        # 0x1400132b8
    140010550:	nop
    140010551:	mov    $0x2,%ecx
    140010556:	call   *0x2dd4(%rip)        # 0x140013330
    14001055c:	mov    %rax,%rcx
-   14001055f:	lea    0x62f2(%rip),%rax        # 0x140016858
+   14001055f:	lea    0x62fa(%rip),%rax        # 0x140016860
    140010566:	mov    %rax,0x20(%rsp)
    14001056b:	mov    $0x5b,%r9d
    140010571:	lea    0x6248(%rip),%r8        # 0x1400167c0
-   140010578:	lea    0x6291(%rip),%rdx        # 0x140016810
+   140010578:	lea    0x6299(%rip),%rdx        # 0x140016818
    14001057f:	call   0x140002470
    140010584:	call   *0x2d2e(%rip)        # 0x1400132b8
    14001058a:	int3
    14001058b:	mov    0x30(%rbp),%rcx
    14001058f:	xor    %rsp,%rcx
    140010592:	call   0x1400113d0
    140010597:	mov    0x198(%rsp),%rbx
@@ -19739,30 +19739,30 @@
    1400105c1:	lea    0x6568(%rip),%rdx        # 0x140016b30
    1400105c8:	lea    -0x10(%rbp),%rcx
    1400105cc:	call   0x14000dc10
    1400105d1:	lea    0x8e08(%rip),%rdx        # 0x1400193e0
    1400105d8:	lea    -0x10(%rbp),%rcx
    1400105dc:	call   0x140011ebc
    1400105e1:	nop
-   1400105e2:	lea    0x629f(%rip),%rdx        # 0x140016888
+   1400105e2:	lea    0x62a7(%rip),%rdx        # 0x140016890
    1400105e9:	lea    0x10(%rbp),%rcx
    1400105ed:	call   0x14000b3f0
    1400105f2:	nop
    1400105f3:	mov    %rax,%rdx
    1400105f6:	lea    -0x10(%rbp),%rcx
    1400105fa:	call   0x14000c1c0
    1400105ff:	lea    0x8d0a(%rip),%rdx        # 0x140019310
    140010606:	lea    -0x10(%rbp),%rcx
    14001060a:	call   0x140011ebc
    14001060f:	nop
    140010610:	call   *0x2c2a(%rip)        # 0x140013240
    140010616:	mov    (%rax),%ecx
    140010618:	call   *0x2c6a(%rip)        # 0x140013288
    14001061e:	mov    %rax,%r8
-   140010621:	lea    0x6250(%rip),%rdx        # 0x140016878
+   140010621:	lea    0x6258(%rip),%rdx        # 0x140016880
    140010628:	lea    0x10(%rbp),%rcx
    14001062c:	call   0x14000dc10
    140010631:	nop
    140010632:	mov    %rax,%rdx
    140010635:	lea    -0x10(%rbp),%rcx
    140010639:	call   0x14000c1c0
    14001063e:	lea    0x8ccb(%rip),%rdx        # 0x140019310
@@ -20049,26 +20049,26 @@
    140010a36:	vzeroupper
    140010a39:	call   *0x27f9(%rip)        # 0x140013238
    140010a3f:	nop
    140010a40:	call   *0x27fa(%rip)        # 0x140013240
    140010a46:	mov    (%rax),%ecx
    140010a48:	call   *0x283a(%rip)        # 0x140013288
    140010a4e:	mov    %rax,%r8
-   140010a51:	lea    0x5e20(%rip),%rdx        # 0x140016878
+   140010a51:	lea    0x5e28(%rip),%rdx        # 0x140016880
    140010a58:	lea    -0x1(%rbp),%rcx
    140010a5c:	call   0x14000dc10
    140010a61:	nop
    140010a62:	mov    %rax,%rdx
    140010a65:	lea    -0x39(%rbp),%rcx
    140010a69:	call   0x14000c1c0
    140010a6e:	lea    0x889b(%rip),%rdx        # 0x140019310
    140010a75:	lea    -0x39(%rbp),%rcx
    140010a79:	call   0x140011ebc
    140010a7e:	nop
-   140010a7f:	lea    0x5e02(%rip),%rdx        # 0x140016888
+   140010a7f:	lea    0x5e0a(%rip),%rdx        # 0x140016890
    140010a86:	lea    -0x1(%rbp),%rcx
    140010a8a:	call   0x14000b3f0
    140010a8f:	nop
    140010a90:	mov    %rax,%rdx
    140010a93:	lea    -0x39(%rbp),%rcx
    140010a97:	call   0x14000c1c0
    140010a9c:	lea    0x886d(%rip),%rdx        # 0x140019310
@@ -20119,15 +20119,15 @@
    140010b1d:	pop    %rsi
    140010b1e:	pop    %rbx
    140010b1f:	ret
    140010b20:	call   *0x271a(%rip)        # 0x140013240
    140010b26:	mov    (%rax),%ecx
    140010b28:	call   *0x275a(%rip)        # 0x140013288
    140010b2e:	mov    %rax,%r8
-   140010b31:	lea    0x5d78(%rip),%rdx        # 0x1400168b0
+   140010b31:	lea    0x5d80(%rip),%rdx        # 0x1400168b8
    140010b38:	lea    0x38(%rsp),%rcx
    140010b3d:	call   0x14000dc10
    140010b42:	nop
    140010b43:	mov    %rax,%rdx
    140010b46:	lea    0x20(%rsp),%rcx
    140010b4b:	call   0x14000c1c0
    140010b50:	lea    0x87b9(%rip),%rdx        # 0x140019310
@@ -20239,15 +20239,15 @@
    140010cd0:	pop    %r12
    140010cd2:	pop    %rdi
    140010cd3:	ret
    140010cd4:	call   *0x2566(%rip)        # 0x140013240
    140010cda:	mov    (%rax),%ecx
    140010cdc:	call   *0x25a6(%rip)        # 0x140013288
    140010ce2:	mov    %rax,%r8
-   140010ce5:	lea    0x5bc4(%rip),%rdx        # 0x1400168b0
+   140010ce5:	lea    0x5bcc(%rip),%rdx        # 0x1400168b8
    140010cec:	lea    0x40(%rsp),%rcx
    140010cf1:	call   0x14000dc10
    140010cf6:	nop
    140010cf7:	mov    %rax,%rdx
    140010cfa:	lea    0x28(%rsp),%rcx
    140010cff:	call   0x14000c1c0
    140010d04:	lea    0x8605(%rip),%rdx        # 0x140019310
@@ -20256,15 +20256,15 @@
    140010d15:	nop
    140010d16:	call   0x14000d590
    140010d1b:	int3
    140010d1c:	call   *0x251e(%rip)        # 0x140013240
    140010d22:	mov    (%rax),%ecx
    140010d24:	call   *0x255e(%rip)        # 0x140013288
    140010d2a:	mov    %rax,%r8
-   140010d2d:	lea    0x5b7c(%rip),%rdx        # 0x1400168b0
+   140010d2d:	lea    0x5b84(%rip),%rdx        # 0x1400168b8
    140010d34:	lea    0x40(%rsp),%rcx
    140010d39:	call   0x14000dc10
    140010d3e:	nop
    140010d3f:	mov    %rax,%rdx
    140010d42:	lea    0x28(%rsp),%rcx
    140010d47:	call   0x14000c1c0
    140010d4c:	lea    0x85bd(%rip),%rdx        # 0x140019310
@@ -27347,32 +27347,30 @@
    1400164e9:	jae    0x140016518
    1400164eb:	jb     0x140016562
    1400164ed:	outsb  %ds:(%rsi),(%dx)
    1400164ee:	outsb  %ds:(%rsi),(%dx)
    1400164ef:	gs jb  0x14001654e
    1400164f2:	(bad)
    1400164f7:	sub    $0x6c697562,%eax
-   1400164fc:	fs pop %rsp
-   1400164fe:	pop    %rdi
-   1400164ff:	ja     0x140016570
-   140016501:	jb     0x14001656e
-   140016503:	pop    %rsp
-   140016504:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   14001650b:	insl   (%dx),%es:(%rdi)
-   14001650c:	pop    %rsp
-   14001650d:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   140016514:	insl   (%dx),%es:(%rdi)
-   140016515:	pop    %rsp
-   140016516:	jae    0x14001658a
-   140016518:	movsxd 0x67(%rdi,%riz,2),%ebx
-   14001651c:	insl   (%dx),%es:(%rdi)
-   14001651d:	insb   (%dx),%es:(%rdi)
-   14001651e:	cs movsxd (%rax),%eax
-   140016521:	add    %al,(%rax)
-   140016523:	add    %al,(%rax)
+   1400164fc:	fs sub $0x5c77656e,%eax
+   140016502:	pop    %rdi
+   140016503:	ja     0x140016574
+   140016505:	jb     0x140016572
+   140016507:	pop    %rsp
+   140016508:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   14001650f:	insl   (%dx),%es:(%rdi)
+   140016510:	pop    %rsp
+   140016511:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   140016518:	insl   (%dx),%es:(%rdi)
+   140016519:	pop    %rsp
+   14001651a:	jae    0x14001658e
+   14001651c:	movsxd 0x67(%rdi,%riz,2),%ebx
+   140016520:	insl   (%dx),%es:(%rdi)
+   140016521:	insb   (%dx),%es:(%rdi)
+   140016522:	cs movsxd (%rax),%eax
    140016525:	add    %al,(%rax)
    140016527:	add    %al,0x47(%rdi)
    14001652a:	rex.WRB
    14001652b:	rex.WR pop %rdi
    14001652d:	push   %r11
    14001652f:	push   %rbx
    140016530:	rex.RB push %r10
@@ -27650,218 +27648,218 @@
    1400167c9:	jae    0x1400167f8
    1400167cb:	jb     0x140016842
    1400167cd:	outsb  %ds:(%rsi),(%dx)
    1400167ce:	outsb  %ds:(%rsi),(%dx)
    1400167cf:	gs jb  0x14001682e
    1400167d2:	(bad)
    1400167d7:	sub    $0x6c697562,%eax
-   1400167dc:	fs pop %rsp
-   1400167de:	pop    %rdi
-   1400167df:	ja     0x140016850
-   1400167e1:	jb     0x14001684e
-   1400167e3:	pop    %rsp
-   1400167e4:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   1400167eb:	insl   (%dx),%es:(%rdi)
-   1400167ec:	pop    %rsp
-   1400167ed:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   1400167f4:	insl   (%dx),%es:(%rdi)
-   1400167f5:	pop    %rsp
-   1400167f6:	jae    0x14001686a
-   1400167f8:	movsxd 0x6c(%rsp,%rbp,2),%ebx
-   1400167fc:	(bad)
-   1400167fd:	insl   (%dx),%es:(%rdi)
-   1400167fe:	(bad)
-   1400167ff:	pop    %rsp
-   140016800:	insb   (%dx),%es:(%rdi)
-   140016801:	insb   (%dx),%es:(%rdi)
+   1400167dc:	fs sub $0x5c77656e,%eax
+   1400167e2:	pop    %rdi
+   1400167e3:	ja     0x140016854
+   1400167e5:	jb     0x140016852
+   1400167e7:	pop    %rsp
+   1400167e8:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   1400167ef:	insl   (%dx),%es:(%rdi)
+   1400167f0:	pop    %rsp
+   1400167f1:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   1400167f8:	insl   (%dx),%es:(%rdi)
+   1400167f9:	pop    %rsp
+   1400167fa:	jae    0x14001686e
+   1400167fc:	movsxd 0x6c(%rsp,%rbp,2),%ebx
+   140016800:	(bad)
+   140016801:	insl   (%dx),%es:(%rdi)
    140016802:	(bad)
-   140016803:	insl   (%dx),%es:(%rdi)
-   140016804:	(bad)
-   140016805:	sub    $0x6c697475,%eax
-   14001680a:	cs push $0x0
-   140016810:	rex.WR
-   140016811:	rex.WR
-   140016812:	rex.B
-   140016813:	rex.WRB
-   140016814:	pop    %r15
-   140016816:	push   %r11
-   140016818:	push   %rbx
-   140016819:	rex.RB push %r10
-   14001681b:	push   %rsp
-   14001681c:	cmp    (%rax),%ah
-   14001681e:	and    $0x64253a73,%eax
-   140016823:	cmp    (%rax),%ah
-   140016825:	and    $0xa73,%eax
-   14001682a:	add    %al,(%rax)
-   14001682c:	add    %al,(%rax)
-   14001682e:	add    %al,(%rax)
-   140016830:	jae    0x14001689b
-   140016832:	jp     0x140016899
-   140016834:	xor    (%rax),%ah
-   140016836:	cmp    $0x6973203d,%eax
-   14001683b:	jp     0x1400168a2
-   14001683d:	add    %al,(%rax)
-   14001683f:	add    %ah,0x61(%rsi)
-   140016842:	imul   $0x206f7420,0x64(%rbp,%riz,2),%ebp
-   14001684a:	outsl  %ds:(%rsi),(%dx)
-   14001684b:	jo     0x1400168b2
-   14001684d:	outsb  %ds:(%rsi),(%dx)
-   14001684e:	and    %ah,0x25203a73(%rip)        # 0x16521a2c7
-   140016854:	jae    0x140016856
-   140016856:	add    %al,(%rax)
-   140016858:	jb     0x1400168bf
-   14001685a:	je     0x14001687c
-   14001685c:	and    %edi,0x312d20(%rip)        # 0x140329582
-   140016862:	add    %al,(%rax)
-   140016864:	add    %al,(%rax)
-   140016866:	add    %al,(%rax)
-   140016868:	jb     0x1400168cf
-   14001686a:	je     0x14001688c
-   14001686c:	cmp    $0x30203d,%eax
-   140016871:	add    %al,(%rax)
-   140016873:	add    %al,(%rax)
-   140016875:	add    %al,(%rax)
-   140016877:	add    %dh,0x65(%rdx)
-   14001687a:	(bad)
-   14001687b:	and    %ah,%fs:0x72(%rbp)
-   14001687f:	jb     0x1400168f0
-   140016881:	jb     0x1400168bd
-   140016883:	and    %ah,0x75000073(%rip)        # 0x1b50168fc
-   140016889:	outsb  %ds:(%rsi),(%dx)
-   14001688a:	gs js  0x1400168fd
-   14001688d:	movsxd %gs:0x64(%rbp,%riz,2),%esi
-   140016892:	insb   (%dx),%es:(%rdi)
-   140016893:	jns    0x1400168b5
-   140016895:	jb     0x1400168fc
-   140016897:	(bad)
-   140016898:	movsxd 0x65(%rax),%ebp
-   14001689b:	and    %ah,%fs:0x6e(%rbp)
-   14001689f:	and    %ch,%fs:0x66(%rdi)
-   1400168a3:	and    %ah,0x69(%rsi)
-   1400168a6:	insb   (%dx),%es:(%rdi)
-   1400168a7:	add    %al,%gs:(%rax)
-   1400168aa:	add    %al,(%rax)
-   1400168ac:	add    %al,(%rax)
-   1400168ae:	add    %al,(%rax)
-   1400168b0:	ja     0x140016924
-   1400168b2:	imul   $0x6f727265,0x20(%rbp,%riz,2),%esi
-   1400168ba:	jb     0x1400168f6
-   1400168bc:	and    %ah,0x6f460073(%rip)        # 0x1af476935
-   1400168c2:	jb     0x140016931
-   1400168c4:	(bad)
-   1400168c5:	je     0x140016914
-   1400168c7:	gs jae 0x14001693d
-   1400168ca:	(bad)
-   1400168cb:	and    %spl,%gs:0x61(%r14d)
-   1400168d1:	imul   $0x77000000,0x64(%rbp,%riz,2),%ebp
-   1400168d9:	(bad)
-   1400168da:	jb     0x14001694a
-   1400168dc:	imul   $0x6e55203a,0x67(%rsi),%ebp
-   1400168e3:	insl   (%dx),%es:(%rdi)
-   1400168e4:	(bad)
-   1400168e5:	jo     0x14001693d
-   1400168e7:	imul   $0x6946664f,0x77(%rbp),%esp
-   1400168ee:	insb   (%dx),%es:(%rdi)
-   1400168ef:	and    %ah,%gs:0x61(%rsi)
-   1400168f3:	imul   $0x7325203a,0x64(%rbp,%riz,2),%ebp
-   1400168fb:	or     (%rax),%al
-   1400168fd:	add    %al,(%rax)
-   1400168ff:	add    %al,(%rax)
-   140016901:	je     0x140016904
-   140016903:	rex add %eax,(%rax)
-   140016906:	add    %al,(%rax)
-   140016908:	nop
-   140016909:	(bad)
-   14001690a:	add    %al,0x1(%rax)
-   14001690d:	add    %al,(%rax)
-   14001690f:	add    %al,0x24(%rax)
+   140016803:	pop    %rsp
+   140016804:	insb   (%dx),%es:(%rdi)
+   140016805:	insb   (%dx),%es:(%rdi)
+   140016806:	(bad)
+   140016807:	insl   (%dx),%es:(%rdi)
+   140016808:	(bad)
+   140016809:	sub    $0x6c697475,%eax
+   14001680e:	cs push $0x0
+   140016814:	add    %al,(%rax)
+   140016816:	add    %al,(%rax)
+   140016818:	rex.WR
+   140016819:	rex.WR
+   14001681a:	rex.B
+   14001681b:	rex.WRB
+   14001681c:	pop    %r15
+   14001681e:	push   %r11
+   140016820:	push   %rbx
+   140016821:	rex.RB push %r10
+   140016823:	push   %rsp
+   140016824:	cmp    (%rax),%ah
+   140016826:	and    $0x64253a73,%eax
+   14001682b:	cmp    (%rax),%ah
+   14001682d:	and    $0xa73,%eax
+   140016832:	add    %al,(%rax)
+   140016834:	add    %al,(%rax)
+   140016836:	add    %al,(%rax)
+   140016838:	jae    0x1400168a3
+   14001683a:	jp     0x1400168a1
+   14001683c:	xor    (%rax),%ah
+   14001683e:	cmp    $0x6973203d,%eax
+   140016843:	jp     0x1400168aa
+   140016845:	add    %al,(%rax)
+   140016847:	add    %ah,0x61(%rsi)
+   14001684a:	imul   $0x206f7420,0x64(%rbp,%riz,2),%ebp
+   140016852:	outsl  %ds:(%rsi),(%dx)
+   140016853:	jo     0x1400168ba
+   140016855:	outsb  %ds:(%rsi),(%dx)
+   140016856:	and    %ah,0x25203a73(%rip)        # 0x16521a2cf
+   14001685c:	jae    0x14001685e
+   14001685e:	add    %al,(%rax)
+   140016860:	jb     0x1400168c7
+   140016862:	je     0x140016884
+   140016864:	and    %edi,0x312d20(%rip)        # 0x14032958a
+   14001686a:	add    %al,(%rax)
+   14001686c:	add    %al,(%rax)
+   14001686e:	add    %al,(%rax)
+   140016870:	jb     0x1400168d7
+   140016872:	je     0x140016894
+   140016874:	cmp    $0x30203d,%eax
+   140016879:	add    %al,(%rax)
+   14001687b:	add    %al,(%rax)
+   14001687d:	add    %al,(%rax)
+   14001687f:	add    %dh,0x65(%rdx)
+   140016882:	(bad)
+   140016883:	and    %ah,%fs:0x72(%rbp)
+   140016887:	jb     0x1400168f8
+   140016889:	jb     0x1400168c5
+   14001688b:	and    %ah,0x75000073(%rip)        # 0x1b5016904
+   140016891:	outsb  %ds:(%rsi),(%dx)
+   140016892:	gs js  0x140016905
+   140016895:	movsxd %gs:0x64(%rbp,%riz,2),%esi
+   14001689a:	insb   (%dx),%es:(%rdi)
+   14001689b:	jns    0x1400168bd
+   14001689d:	jb     0x140016904
+   14001689f:	(bad)
+   1400168a0:	movsxd 0x65(%rax),%ebp
+   1400168a3:	and    %ah,%fs:0x6e(%rbp)
+   1400168a7:	and    %ch,%fs:0x66(%rdi)
+   1400168ab:	and    %ah,0x69(%rsi)
+   1400168ae:	insb   (%dx),%es:(%rdi)
+   1400168af:	add    %al,%gs:(%rax)
+   1400168b2:	add    %al,(%rax)
+   1400168b4:	add    %al,(%rax)
+   1400168b6:	add    %al,(%rax)
+   1400168b8:	ja     0x14001692c
+   1400168ba:	imul   $0x6f727265,0x20(%rbp,%riz,2),%esi
+   1400168c2:	jb     0x1400168fe
+   1400168c4:	and    %ah,0x6f460073(%rip)        # 0x1af47693d
+   1400168ca:	jb     0x140016939
+   1400168cc:	(bad)
+   1400168cd:	je     0x14001691c
+   1400168cf:	gs jae 0x140016945
+   1400168d2:	(bad)
+   1400168d3:	and    %spl,%gs:0x61(%r14d)
+   1400168d9:	imul   $0x77000000,0x64(%rbp,%riz,2),%ebp
+   1400168e1:	(bad)
+   1400168e2:	jb     0x140016952
+   1400168e4:	imul   $0x6e55203a,0x67(%rsi),%ebp
+   1400168eb:	insl   (%dx),%es:(%rdi)
+   1400168ec:	(bad)
+   1400168ed:	jo     0x140016945
+   1400168ef:	imul   $0x6946664f,0x77(%rbp),%esp
+   1400168f6:	insb   (%dx),%es:(%rdi)
+   1400168f7:	and    %ah,%gs:0x61(%rsi)
+   1400168fb:	imul   $0x7325203a,0x64(%rbp,%riz,2),%ebp
+   140016903:	or     (%rax),%al
+   140016905:	add    %al,(%rax)
+   140016907:	add    %al,(%rax)
+   140016909:	je     0x14001690c
+   14001690b:	rex add %eax,(%rax)
+   14001690e:	add    %al,(%rax)
+   140016910:	nop
+   140016911:	(bad)
    140016912:	add    %al,0x1(%rax)
    140016915:	add    %al,(%rax)
-   140016917:	add    %cl,0x1400174(%rax)
+   140016917:	add    %al,0x24(%rax)
+   14001691a:	add    %al,0x1(%rax)
    14001691d:	add    %al,(%rax)
-   14001691f:	add    %dl,0x14000ce(%rax)
+   14001691f:	add    %cl,0x1400174(%rax)
    140016925:	add    %al,(%rax)
-   140016927:	add    %al,0x24(%rax)
-   14001692a:	add    %al,0x1(%rax)
+   140016927:	add    %dl,0x14000ce(%rax)
    14001692d:	add    %al,(%rax)
-   14001692f:	add    %bl,(%rax)
-   140016931:	jne    0x140016934
-   140016933:	rex add %eax,(%rax)
-   140016936:	add    %al,(%rax)
-   140016938:	(bad)
-   140016939:	(bad)
-   14001693a:	add    %al,0x1(%rax)
-   14001693d:	add    %al,(%rax)
-   14001693f:	add    %dl,(%rax)
-   140016941:	cli
+   14001692f:	add    %al,0x24(%rax)
+   140016932:	add    %al,0x1(%rax)
+   140016935:	add    %al,(%rax)
+   140016937:	add    %bl,(%rax)
+   140016939:	jne    0x14001693c
+   14001693b:	rex add %eax,(%rax)
+   14001693e:	add    %al,(%rax)
+   140016940:	(bad)
+   140016941:	(bad)
    140016942:	add    %al,0x1(%rax)
    140016945:	add    %al,(%rax)
-   140016947:	add    %al,%al
-   140016949:	stc
+   140016947:	add    %dl,(%rax)
+   140016949:	cli
    14001694a:	add    %al,0x1(%rax)
    14001694d:	add    %al,(%rax)
-   14001694f:	add    %ah,0x14000da(%rax)
+   14001694f:	add    %al,%al
+   140016951:	stc
+   140016952:	add    %al,0x1(%rax)
    140016955:	add    %al,(%rax)
-   140016957:	add    %dh,0x14000da(%rax)
+   140016957:	add    %ah,0x14000da(%rax)
    14001695d:	add    %al,(%rax)
-   14001695f:	add    %dl,%al
-   140016961:	fiaddl (%rax)
-   140016963:	rex add %eax,(%rax)
-   140016966:	add    %al,(%rax)
-   140016968:	outsb  %gs:(%esi),(%dx)
-   14001696b:	gs jb  0x1400169d7
-   14001696e:	movsxd (%rax),%eax
-   140016970:	and    $0x20007535,%eax
-   140016975:	js     0x140016997
-   140016977:	and    $0x7535,%eax
-   14001697c:	add    %al,(%rax)
-   14001697e:	add    %al,(%rax)
-   140016980:	imul   $0x69736e6f,0x63(%rsi),%ebp
-   140016987:	jae    0x1400169fd
-   140016989:	outsb  %gs:(%rsi),(%dx)
-   14001698b:	je     0x1400169ad
-   14001698d:	je     0x1400169f4
-   14001698f:	outsb  %ds:(%rsi),(%dx)
-   140016990:	jae    0x140016a01
-   140016992:	jb     0x1400169b4
-   140016994:	jae    0x1400169fe
-   140016996:	(bad)
-   140016997:	jb     0x1400169fd
-   140016999:	and    %dh,0x70(%rcx,%rdi,2)
-   14001699d:	and    %ch,%gs:0x6e(%rcx)
-   1400169a1:	and    %ah,(%rdi)
-   1400169a3:	and    $0x2773,%eax
-   1400169a8:	je     0x140016a19
-   1400169aa:	imul   $0x6d,0x65(%rdi),%ebx
-   1400169ae:	(bad)
-   1400169b3:	outsb  %ds:(%rsi),(%dx)
-   1400169b4:	addr32 jae 0x1400169e5
-   1400169b7:	add    %ch,(%rsi)
-   1400169b9:	(bad)
-   1400169ba:	je     0x140016a30
-   1400169bc:	outsb  %gs:(%rsi),(%dx)
-   1400169be:	je     0x140016a29
-   1400169c0:	outsl  %ds:(%rsi),(%dx)
-   1400169c1:	outsb  %ds:(%rsi),(%dx)
-   1400169c2:	ja,pn  0x140016a34
-   1400169c5:	ja,pn  0x140016a2d
-   1400169c8:	imul   $0x74,0x68(%rdi),%esp
-   1400169cf:	add    %ch,(%rsi)
-   1400169d1:	gs gs fs pop %di
-   1400169d6:	outsw  %ds:(%rsi),(%dx)
-   1400169d8:	jb     0x140016a51
-   1400169da:	(bad)
-   1400169db:	jb     0x140016a41
-   1400169dd:	ja,pn  0x140016a12
-   1400169e0:	ja,pn  0x140016a48
-   1400169e3:	imul   $0x74,0x68(%rdi),%esp
-   1400169ea:	add    %al,(%rax)
-   1400169ec:	add    %al,(%rax)
-   1400169ee:	add    %al,(%rax)
-   1400169f0:	imul   $0x69736e6f,0x63(%rsi),%ebp
+   14001695f:	add    %dh,0x14000da(%rax)
+   140016965:	add    %al,(%rax)
+   140016967:	add    %dl,%al
+   140016969:	fiaddl (%rax)
+   14001696b:	rex add %eax,(%rax)
+   14001696e:	add    %al,(%rax)
+   140016970:	outsb  %gs:(%esi),(%dx)
+   140016973:	gs jb  0x1400169df
+   140016976:	movsxd (%rax),%eax
+   140016978:	and    $0x20007535,%eax
+   14001697d:	js     0x14001699f
+   14001697f:	and    $0x7535,%eax
+   140016984:	add    %al,(%rax)
+   140016986:	add    %al,(%rax)
+   140016988:	imul   $0x69736e6f,0x63(%rsi),%ebp
+   14001698f:	jae    0x140016a05
+   140016991:	outsb  %gs:(%rsi),(%dx)
+   140016993:	je     0x1400169b5
+   140016995:	je     0x1400169fc
+   140016997:	outsb  %ds:(%rsi),(%dx)
+   140016998:	jae    0x140016a09
+   14001699a:	jb     0x1400169bc
+   14001699c:	jae    0x140016a06
+   14001699e:	(bad)
+   14001699f:	jb     0x140016a05
+   1400169a1:	and    %dh,0x70(%rcx,%rdi,2)
+   1400169a5:	and    %ch,%gs:0x6e(%rcx)
+   1400169a9:	and    %ah,(%rdi)
+   1400169ab:	and    $0x2773,%eax
+   1400169b0:	je     0x140016a21
+   1400169b2:	imul   $0x6d,0x65(%rdi),%ebx
+   1400169b6:	(bad)
+   1400169bb:	outsb  %ds:(%rsi),(%dx)
+   1400169bc:	addr32 jae 0x1400169ed
+   1400169bf:	add    %ch,(%rsi)
+   1400169c1:	(bad)
+   1400169c2:	je     0x140016a38
+   1400169c4:	outsb  %gs:(%rsi),(%dx)
+   1400169c6:	je     0x140016a31
+   1400169c8:	outsl  %ds:(%rsi),(%dx)
+   1400169c9:	outsb  %ds:(%rsi),(%dx)
+   1400169ca:	ja,pn  0x140016a3c
+   1400169cd:	ja,pn  0x140016a35
+   1400169d0:	imul   $0x74,0x68(%rdi),%esp
+   1400169d7:	add    %ch,(%rsi)
+   1400169d9:	gs gs fs pop %di
+   1400169de:	outsw  %ds:(%rsi),(%dx)
+   1400169e0:	jb     0x140016a59
+   1400169e2:	(bad)
+   1400169e3:	jb     0x140016a49
+   1400169e5:	ja,pn  0x140016a1a
+   1400169e8:	ja,pn  0x140016a50
+   1400169eb:	imul   $0x6e690074,0x68(%rdi),%esp
+   1400169f2:	movsxd 0x6e(%rdi),%ebp
+   1400169f5:	jae    0x140016a60
    1400169f7:	jae    0x140016a6d
    1400169f9:	outsb  %gs:(%rsi),(%dx)
    1400169fb:	je     0x140016a1d
    1400169fd:	je     0x140016a64
    1400169ff:	outsb  %ds:(%rsi),(%dx)
    140016a00:	jae    0x140016a71
    140016a02:	jb     0x140016a24
@@ -27905,50 +27903,53 @@
    140016a69:	jae    0x140016a98
    140016a6b:	jb     0x140016ae2
    140016a6d:	outsb  %ds:(%rsi),(%dx)
    140016a6e:	outsb  %ds:(%rsi),(%dx)
    140016a6f:	gs jb  0x140016ace
    140016a72:	(bad)
    140016a77:	sub    $0x6c697562,%eax
-   140016a7c:	fs pop %rsp
-   140016a7e:	pop    %rdi
-   140016a7f:	ja     0x140016af0
-   140016a81:	jb     0x140016aee
-   140016a83:	pop    %rsp
-   140016a84:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   140016a8b:	insl   (%dx),%es:(%rdi)
-   140016a8c:	pop    %rsp
-   140016a8d:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   140016a94:	insl   (%dx),%es:(%rdi)
-   140016a95:	pop    %rsp
-   140016a96:	jae    0x140016b0a
-   140016a98:	movsxd 0x6c(%rsp,%rbp,2),%ebx
-   140016a9c:	(bad)
-   140016a9d:	insl   (%dx),%es:(%rdi)
-   140016a9e:	(bad)
-   140016a9f:	pop    %rsp
-   140016aa0:	insb   (%dx),%es:(%rdi)
-   140016aa1:	insb   (%dx),%es:(%rdi)
+   140016a7c:	fs sub $0x5c77656e,%eax
+   140016a82:	pop    %rdi
+   140016a83:	ja     0x140016af4
+   140016a85:	jb     0x140016af2
+   140016a87:	pop    %rsp
+   140016a88:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   140016a8f:	insl   (%dx),%es:(%rdi)
+   140016a90:	pop    %rsp
+   140016a91:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   140016a98:	insl   (%dx),%es:(%rdi)
+   140016a99:	pop    %rsp
+   140016a9a:	jae    0x140016b0e
+   140016a9c:	movsxd 0x6c(%rsp,%rbp,2),%ebx
+   140016aa0:	(bad)
+   140016aa1:	insl   (%dx),%es:(%rdi)
    140016aa2:	(bad)
-   140016aa3:	insl   (%dx),%es:(%rdi)
-   140016aa4:	(bad)
-   140016aa5:	cs movsxd 0x70(%rax),%esi
-   140016aa9:	add    %al,(%rax)
-   140016aab:	add    %dh,0x62(%rdx)
-   140016aae:	add    %al,(%rax)
-   140016ab0:	(bad)
-   140016ab5:	sub    $0x3a6d6c6c,%eax
-   140016aba:	and    %ch,0x61(%rdi,%rbp,2)
-   140016abe:	imul   $0x646f6d20,%fs:0x67(%rsi),%ebp
-   140016ac6:	gs insb (%dx),%es:(%rdi)
-   140016ac8:	and    %ah,0x72(%rsi)
-   140016acb:	outsl  %ds:(%rsi),(%dx)
-   140016acc:	insl   (%dx),%es:(%rdi)
-   140016acd:	and    %ah,0xa73(%rip)        # 0x140017546
-	...
+   140016aa3:	pop    %rsp
+   140016aa4:	insb   (%dx),%es:(%rdi)
+   140016aa5:	insb   (%dx),%es:(%rdi)
+   140016aa6:	(bad)
+   140016aa7:	insl   (%dx),%es:(%rdi)
+   140016aa8:	(bad)
+   140016aa9:	cs movsxd 0x70(%rax),%esi
+   140016aad:	add    %al,(%rax)
+   140016aaf:	add    %dh,0x62(%rdx)
+   140016ab2:	add    %al,(%rax)
+   140016ab4:	add    %al,(%rax)
+   140016ab6:	add    %al,(%rax)
+   140016ab8:	(bad)
+   140016abd:	sub    $0x3a6d6c6c,%eax
+   140016ac2:	and    %ch,0x61(%rdi,%rbp,2)
+   140016ac6:	imul   $0x646f6d20,%fs:0x67(%rsi),%ebp
+   140016ace:	gs insb (%dx),%es:(%rdi)
+   140016ad0:	and    %ah,0x72(%rsi)
+   140016ad3:	outsl  %ds:(%rsi),(%dx)
+   140016ad4:	insl   (%dx),%es:(%rdi)
+   140016ad5:	and    %ah,0xa73(%rip)        # 0x14001754e
+   140016adb:	add    %al,(%rax)
+   140016add:	add    %al,(%rax)
    140016adf:	add    %dh,0x6e(%rbp)
    140016ae2:	imul   $0x77,0x6f(%rsi),%ebp
    140016ae6:	outsb  %ds:(%rsi),(%dx)
    140016ae7:	and    %ch,(%rax)
    140016ae9:	insl   (%dx),%es:(%rdi)
    140016aea:	(bad)
    140016aeb:	imul   $0x72657620,0x2c(%ebx),%esp
@@ -28460,19 +28461,17 @@
    1400170ed:	add    %al,(%rax)
    1400170ef:	add    %cl,0x1400133(%rax)
    1400170f5:	add    %al,(%rax)
    1400170f7:	add    %dl,0x1400133(%rax)
    1400170fd:	add    %al,(%rax)
    1400170ff:	add    %al,(%rax)
    140017101:	add    %al,(%rax)
-   140017103:	add    %bl,(%rsp,%rbp,4)
-   140017106:	push   %rax
-   140017107:	data16 add %al,(%rax)
-   14001710a:	add    %al,(%rax)
-   14001710c:	or     $0x90000000,%eax
+   140017103:	add    %dl,0x6651fd(%rbx)
+   140017109:	add    %al,(%rax)
+   14001710b:	add    %cl,-0x70000000(%rip)        # 0xd0017111
    140017111:	add    (%rax),%eax
    140017113:	add    %ch,%ah
    140017115:	jbe    0x140017118
    140017117:	add    %ch,%ah
    140017119:	(bad)
 	...
    14001717e:	add    %al,(%rax)
@@ -33619,22 +33618,20 @@
    14001b439:	cmp    (%rcx),%eax
    14001b43b:	rex add %eax,(%rax)
    14001b43e:	add    %al,(%rax)
    14001b440:	pop    %rsp
    14001b441:	cmp    (%rcx),%eax
    14001b443:	rex add %eax,(%rax)
    14001b446:	add    %al,(%rax)
-   14001b448:	cmp    %ch,0x1(%rcx)
-   14001b44b:	rex add %eax,(%rax)
-   14001b44e:	add    %al,(%rax)
-   14001b450:	add    (%rax),%eax
-   14001b452:	add    %al,(%rax)
-   14001b454:	add    %al,(%rax)
-   14001b456:	add    %al,(%rax)
-   14001b458:	(bad)
+   14001b448:	rex imul $0x140,(%rcx),%eax
+   14001b44f:	add    %al,(%rbx)
+   14001b451:	add    %al,(%rax)
+   14001b453:	add    %al,(%rax)
+   14001b455:	add    %al,(%rax)
+   14001b457:	add    %bh,%bh
    14001b459:	(bad)
    14001b45a:	(bad)
    14001b45b:	incl   (%rax)
    14001b45d:	add    %al,(%rax)
    14001b45f:	add    %cl,%ch
    14001b461:	pop    %rbp
    14001b462:	and    %dl,%dl
@@ -35570,20 +35567,21 @@
    1400c006e:	cwtl
    1400c006f:	scas   %es:(%rdi),%eax
    1400c0070:	add    %ah,0x1(%rax)
    1400c0073:	add    %dh,(%rax)
    1400c0075:	add    %al,(%rax)
    1400c0077:	add    %cl,-0x67586f59(%rax)
    1400c007d:	cmpsl  %es:(%rdi),%ds:(%rsi)
-   1400c007e:	add    %ch,-0x56ef56f8(%rcx)
-   1400c0084:	sbb    %ch,-0x56d756e0(%rcx)
-   1400c008a:	xor    %ch,-0x56bf56c8(%rcx)
-   1400c0090:	test   $0xffffffffa958a950,%rax
-   1400c0096:	(bad)
-   1400c0097:	test   $0xaf98af90,%eax
+   1400c007e:	or     %ch,-0x56e756f0(%rcx)
+   1400c0084:	and    %ch,-0x56cf56d8(%rcx)
+   1400c008a:	cmp    %ch,-0x56b756c0(%rcx)
+   1400c0090:	push   %rax
+   1400c0091:	test   $0xa960a958,%eax
+   1400c0096:	push   $0xffffffff98af90a9
+   1400c009b:	scas   %es:(%rdi),%eax
    1400c009c:	movabs 0x2400017000afa8af,%al
    1400c00a5:	add    %al,(%rax)
    1400c00a7:	add    %bl,(%rax)
    1400c00a9:	movabs 0xa0d8a0c0a038a030,%al
    1400c00b2:	loopne 0x1400c0054
    1400c00b4:	call   0x138acf159
    1400c00b9:	movabs 0xa198a190a188a180,%al
```

## ipex_llm/libs/quantize-llama_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140011af8
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Fri May 24 15:03:58 2024
+Time/Date		Sat May 25 15:02:34 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000011c00
 SizeOfInitializedData	00000000000aac00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000011af8
@@ -28608,19 +28608,17 @@
    1400170cd:	add    %al,(%rax)
    1400170cf:	add    %cl,0x1400133(%rax)
    1400170d5:	add    %al,(%rax)
    1400170d7:	add    %dl,0x1400133(%rax)
    1400170dd:	add    %al,(%rax)
    1400170df:	add    %al,(%rax)
    1400170e1:	add    %al,(%rax)
-   1400170e3:	add    %bl,-0x54(%rsi)
-   1400170e6:	push   %rax
-   1400170e7:	data16 add %al,(%rax)
-   1400170ea:	add    %al,(%rax)
-   1400170ec:	or     $0x90000000,%eax
+   1400170e3:	add    %cl,0x6651fd(%rdx)
+   1400170e9:	add    %al,(%rax)
+   1400170eb:	add    %cl,-0x70000000(%rip)        # 0xd00170f1
    1400170f1:	add    (%rax),%eax
    1400170f3:	add    %ch,0x1(%rsi,%rsi,2)
    1400170f7:	add    %ch,0x1(%rsi,%riz,2)
    1400170fb:	add    %al,(%rax)
    1400170fd:	add    %al,(%rax)
    1400170ff:	add    %ah,(%rax)
    140017101:	jp     0x140017104
```

## ipex_llm/libs/quantize-starcoder.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140013c70
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Fri May 24 15:02:53 2024
+Time/Date		Sat May 25 15:02:44 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000013c00
 SizeOfInitializedData	00000000000ace00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000013c70
@@ -32291,32 +32291,30 @@
    140018f99:	jae    0x140018fc8
    140018f9b:	jb     0x140019012
    140018f9d:	outsb  %ds:(%rsi),(%dx)
    140018f9e:	outsb  %ds:(%rsi),(%dx)
    140018f9f:	gs jb  0x140018ffe
    140018fa2:	(bad)
    140018fa7:	sub    $0x6c697562,%eax
-   140018fac:	fs pop %rsp
-   140018fae:	pop    %rdi
-   140018faf:	ja     0x140019020
-   140018fb1:	jb     0x14001901e
-   140018fb3:	pop    %rsp
-   140018fb4:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   140018fbb:	insl   (%dx),%es:(%rdi)
-   140018fbc:	pop    %rsp
-   140018fbd:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   140018fc4:	insl   (%dx),%es:(%rdi)
-   140018fc5:	pop    %rsp
-   140018fc6:	jae    0x14001903a
-   140018fc8:	movsxd 0x67(%rdi,%riz,2),%ebx
-   140018fcc:	insl   (%dx),%es:(%rdi)
-   140018fcd:	insb   (%dx),%es:(%rdi)
-   140018fce:	cs movsxd (%rax),%eax
-   140018fd1:	add    %al,(%rax)
-   140018fd3:	add    %al,(%rax)
+   140018fac:	fs sub $0x5c77656e,%eax
+   140018fb2:	pop    %rdi
+   140018fb3:	ja     0x140019024
+   140018fb5:	jb     0x140019022
+   140018fb7:	pop    %rsp
+   140018fb8:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   140018fbf:	insl   (%dx),%es:(%rdi)
+   140018fc0:	pop    %rsp
+   140018fc1:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   140018fc8:	insl   (%dx),%es:(%rdi)
+   140018fc9:	pop    %rsp
+   140018fca:	jae    0x14001903e
+   140018fcc:	movsxd 0x67(%rdi,%riz,2),%ebx
+   140018fd0:	insl   (%dx),%es:(%rdi)
+   140018fd1:	insb   (%dx),%es:(%rdi)
+   140018fd2:	cs movsxd (%rax),%eax
    140018fd5:	add    %al,(%rax)
    140018fd7:	add    %al,0x47(%rdi)
    140018fda:	rex.WRB
    140018fdb:	rex.WR pop %rdi
    140018fdd:	push   %r11
    140018fdf:	push   %rbx
    140018fe0:	rex.RB push %r10
@@ -32579,17 +32577,17 @@
    140019325:	add    %al,(%rax)
    140019327:	add    %al,(%rax)
    140019329:	push   %rbp
    14001932a:	add    %eax,0x1(%rax)
    14001932d:	add    %al,(%rax)
    14001932f:	add    %al,(%rax)
    140019331:	add    %al,(%rax)
-   140019333:	add    %bl,0x6650ac(%rip)        # 0x14067e3e5
-   140019339:	add    %al,(%rax)
-   14001933b:	add    %cl,0x20000000(%rip)        # 0x160019341
+   140019333:	add    %dl,0x6651(%rbp,%rdi,8)
+   14001933a:	add    %al,(%rax)
+   14001933c:	or     $0x20000000,%eax
    140019341:	add    (%rax),%eax
    140019343:	add    %bh,%ah
    140019345:	movabs %al,0x192fc0001
 	...
    14001937e:	add    %al,(%rax)
    140019380:	add    %eax,(%rax)
 	...
```

## ipex_llm/libs/quantize-starcoder_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140013e80
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Fri May 24 15:03:59 2024
+Time/Date		Sat May 25 15:02:34 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000013e00
 SizeOfInitializedData	00000000000ad200
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000013e80
@@ -32704,19 +32704,17 @@
    140019305:	add    %al,(%rax)
    140019307:	add    %al,(%rax)
    140019309:	push   %rbp
    14001930a:	add    %eax,0x1(%rax)
    14001930d:	add    %al,(%rax)
    14001930f:	add    %al,(%rax)
    140019311:	add    %al,(%rax)
-   140019313:	add    %bl,-0x54(%rdi)
-   140019316:	push   %rax
-   140019317:	data16 add %al,(%rax)
-   14001931a:	add    %al,(%rax)
-   14001931c:	or     $0x20000000,%eax
+   140019313:	add    %cl,0x6651fd(%rdx)
+   140019319:	add    %al,(%rax)
+   14001931b:	add    %cl,0x20000000(%rip)        # 0x160019321
    140019321:	add    (%rax),%eax
    140019323:	add    %bh,%ah
    140019325:	movabs %al,0x194fc0001
 	...
    14001937e:	add    %al,(%rax)
    140019380:	add    %eax,(%rax)
 	...
```

## ipex_llm/libs/starcoder-api.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018000277c
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Fri May 24 15:02:53 2024
+Time/Date		Sat May 25 15:02:43 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000002200
 SizeOfInitializedData	0000000000003400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000000277c
@@ -4028,17 +4028,20 @@
    1800045f0:	cmp    %al,0x0(%rdx)
    1800045f3:	addb   $0x0,(%rcx)
    1800045f6:	add    %al,(%rax)
    1800045f8:	rex
    1800045f9:	rex.X add %al,0x1(%rax)
    180004600:	add    %al,(%rax)
    180004602:	add    %al,(%rax)
-   180004604:	sbb    $0x6650ac,%eax
-   180004609:	add    %al,(%rax)
-   18000460b:	add    %cl,-0x20000000(%rip)        # 0x160004611
+   180004604:	xchg   %eax,%ebx
+   180004605:	std
+   180004606:	push   %rcx
+   180004607:	data16 add %al,(%rax)
+   18000460a:	add    %al,(%rax)
+   18000460c:	or     $0xe0000000,%eax
    180004611:	add    (%rax),%al
    180004613:	add    %ah,%ah
    180004615:	rex.W add %al,(%rax)
    180004618:	in     $0x2e,%al
 	...
    18000467e:	add    %al,(%rax)
    180004680:	add    %eax,(%rax)
```

## ipex_llm/libs/starcoder.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180063368
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Fri May 24 15:02:53 2024
+Time/Date		Sat May 25 15:02:44 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000063a00
 SizeOfInitializedData	00000000000c8000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000063368
@@ -126947,32 +126947,30 @@
    180068e49:	jae    0x180068e78
    180068e4b:	jb     0x180068ec2
    180068e4d:	outsb  %ds:(%rsi),(%dx)
    180068e4e:	outsb  %ds:(%rsi),(%dx)
    180068e4f:	gs jb  0x180068eae
    180068e52:	(bad)
    180068e57:	sub    $0x6c697562,%eax
-   180068e5c:	fs pop %rsp
-   180068e5e:	pop    %rdi
-   180068e5f:	ja     0x180068ed0
-   180068e61:	jb     0x180068ece
-   180068e63:	pop    %rsp
-   180068e64:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   180068e6b:	insl   (%dx),%es:(%rdi)
-   180068e6c:	pop    %rsp
-   180068e6d:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   180068e74:	insl   (%dx),%es:(%rdi)
-   180068e75:	pop    %rsp
-   180068e76:	jae    0x180068eea
-   180068e78:	movsxd 0x67(%rdi,%riz,2),%ebx
-   180068e7c:	insl   (%dx),%es:(%rdi)
-   180068e7d:	insb   (%dx),%es:(%rdi)
-   180068e7e:	cs movsxd (%rax),%eax
-   180068e81:	add    %al,(%rax)
-   180068e83:	add    %al,(%rax)
+   180068e5c:	fs sub $0x5c77656e,%eax
+   180068e62:	pop    %rdi
+   180068e63:	ja     0x180068ed4
+   180068e65:	jb     0x180068ed2
+   180068e67:	pop    %rsp
+   180068e68:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   180068e6f:	insl   (%dx),%es:(%rdi)
+   180068e70:	pop    %rsp
+   180068e71:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   180068e78:	insl   (%dx),%es:(%rdi)
+   180068e79:	pop    %rsp
+   180068e7a:	jae    0x180068eee
+   180068e7c:	movsxd 0x67(%rdi,%riz,2),%ebx
+   180068e80:	insl   (%dx),%es:(%rdi)
+   180068e81:	insb   (%dx),%es:(%rdi)
+   180068e82:	cs movsxd (%rax),%eax
    180068e85:	add    %al,(%rax)
    180068e87:	add    %al,0x47(%rdi)
    180068e8a:	rex.WRB
    180068e8b:	rex.WR pop %rdi
    180068e8d:	push   %r11
    180068e8f:	push   %rbx
    180068e90:	rex.RB push %r10
@@ -133086,17 +133084,20 @@
    18006cd77:	add    %al,%al
    18006cd79:	push   %rsi
    18006cd7a:	(bad)
    18006cd7b:	addb   $0x0,(%rcx)
    18006cd7e:	add    %al,(%rax)
    18006cd80:	add    %al,(%rax)
    18006cd82:	add    %al,(%rax)
-   18006cd84:	sbb    $0x6650ac,%eax
-   18006cd89:	add    %al,(%rax)
-   18006cd8b:	add    %cl,0x50000000(%rip)        # 0x1d006cd91
+   18006cd84:	xchg   %eax,%esp
+   18006cd85:	std
+   18006cd86:	push   %rcx
+   18006cd87:	data16 add %al,(%rax)
+   18006cd8a:	add    %al,(%rax)
+   18006cd8c:	or     $0x50000000,%eax
    18006cd91:	add    (%rax),%eax
    18006cd93:	add    %dl,-0x21(%rax)
    18006cd96:	(bad)
    18006cd97:	add    %dl,-0x33(%rax)
    18006cd9a:	(bad)
 	...
    18006cdff:	add    %al,%al
```

## Comparing `ipex_llm-2.1.0b20240524.data/scripts/ipex-llm-init.bat` & `ipex_llm-2.1.0b20240525.data/scripts/ipex-llm-init.bat`

 * *Files identical despite different names*

## Comparing `ipex_llm-2.1.0b20240524.data/scripts/llm-chat.ps1` & `ipex_llm-2.1.0b20240525.data/scripts/llm-chat.ps1`

 * *Files identical despite different names*

## Comparing `ipex_llm-2.1.0b20240524.data/scripts/llm-cli.ps1` & `ipex_llm-2.1.0b20240525.data/scripts/llm-cli.ps1`

 * *Files identical despite different names*

## Comparing `ipex_llm-2.1.0b20240524.dist-info/METADATA` & `ipex_llm-2.1.0b20240525.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipex-llm
-Version: 2.1.0b20240524
+Version: 2.1.0b20240525
 Summary: Large Language Model Develop Toolkit
 Home-page: https://github.com/intel-analytics/ipex-llm
 Author: BigDL Authors
 Author-email: bigdl-user-group@googlegroups.com
 License: Apache License, Version 2.0
 Platform: windows
 Classifier: License :: OSI Approved :: Apache Software License
@@ -22,15 +22,15 @@
 Requires-Dist: tokenizers (==0.15.2) ; extra == 'all'
 Requires-Dist: accelerate (==0.21.0) ; extra == 'all'
 Requires-Dist: tabulate ; extra == 'all'
 Requires-Dist: intel-openmp ; (platform_machine == "x86_64" or platform_machine == "AMD64") and extra == 'all'
 Requires-Dist: torch (==2.1.2+cpu) ; (platform_system == "Linux") and extra == 'all'
 Requires-Dist: torch (==2.1.2) ; (platform_system == "Windows") and extra == 'all'
 Provides-Extra: cpp
-Requires-Dist: bigdl-core-cpp (==2.5.0b20240524) ; extra == 'cpp'
+Requires-Dist: bigdl-core-cpp (==2.5.0b20240525) ; extra == 'cpp'
 Requires-Dist: dpcpp-cpp-rt (==2024.0.2) ; (platform_system == "Windows") and extra == 'cpp'
 Requires-Dist: mkl-dpcpp (==2024.0.0) ; (platform_system == "Windows") and extra == 'cpp'
 Requires-Dist: onednn (==2024.0.0) ; (platform_system == "Windows") and extra == 'cpp'
 Provides-Extra: llama-index
 Requires-Dist: py-cpuinfo ; extra == 'llama-index'
 Requires-Dist: protobuf ; extra == 'llama-index'
 Requires-Dist: mpmath (==1.3.0) ; extra == 'llama-index'
@@ -58,32 +58,32 @@
 Requires-Dist: tokenizers (==0.15.2) ; extra == 'xpu'
 Requires-Dist: accelerate (==0.21.0) ; extra == 'xpu'
 Requires-Dist: tabulate ; extra == 'xpu'
 Requires-Dist: setuptools (<70.0.0) ; extra == 'xpu'
 Requires-Dist: torch (==2.1.0a0) ; extra == 'xpu'
 Requires-Dist: torchvision (==0.16.0a0) ; extra == 'xpu'
 Requires-Dist: intel-extension-for-pytorch (==2.1.10+xpu) ; extra == 'xpu'
-Requires-Dist: bigdl-core-xe-21 (==2.5.0b20240524) ; extra == 'xpu'
-Requires-Dist: bigdl-core-xe-esimd-21 (==2.5.0b20240524) ; extra == 'xpu'
+Requires-Dist: bigdl-core-xe-21 (==2.5.0b20240525) ; extra == 'xpu'
+Requires-Dist: bigdl-core-xe-esimd-21 (==2.5.0b20240525) ; extra == 'xpu'
 Provides-Extra: xpu-2-1
 Requires-Dist: py-cpuinfo ; extra == 'xpu-2-1'
 Requires-Dist: protobuf ; extra == 'xpu-2-1'
 Requires-Dist: mpmath (==1.3.0) ; extra == 'xpu-2-1'
 Requires-Dist: numpy (==1.26.4) ; extra == 'xpu-2-1'
 Requires-Dist: transformers (==4.36.2) ; extra == 'xpu-2-1'
 Requires-Dist: sentencepiece ; extra == 'xpu-2-1'
 Requires-Dist: tokenizers (==0.15.2) ; extra == 'xpu-2-1'
 Requires-Dist: accelerate (==0.21.0) ; extra == 'xpu-2-1'
 Requires-Dist: tabulate ; extra == 'xpu-2-1'
 Requires-Dist: setuptools (<70.0.0) ; extra == 'xpu-2-1'
 Requires-Dist: torch (==2.1.0a0) ; extra == 'xpu-2-1'
 Requires-Dist: torchvision (==0.16.0a0) ; extra == 'xpu-2-1'
 Requires-Dist: intel-extension-for-pytorch (==2.1.10+xpu) ; extra == 'xpu-2-1'
-Requires-Dist: bigdl-core-xe-21 (==2.5.0b20240524) ; extra == 'xpu-2-1'
-Requires-Dist: bigdl-core-xe-esimd-21 (==2.5.0b20240524) ; extra == 'xpu-2-1'
+Requires-Dist: bigdl-core-xe-21 (==2.5.0b20240525) ; extra == 'xpu-2-1'
+Requires-Dist: bigdl-core-xe-esimd-21 (==2.5.0b20240525) ; extra == 'xpu-2-1'
 Requires-Dist: intel-openmp ; (platform_machine == "x86_64" or platform_machine == "AMD64") and extra == 'xpu-2-1'
 Requires-Dist: dpcpp-cpp-rt (==2024.0.2) ; (platform_system == "Windows") and extra == 'xpu-2-1'
 Requires-Dist: mkl-dpcpp (==2024.0.0) ; (platform_system == "Windows") and extra == 'xpu-2-1'
 Requires-Dist: onednn (==2024.0.0) ; (platform_system == "Windows") and extra == 'xpu-2-1'
 Requires-Dist: intel-openmp ; (platform_machine == "x86_64" or platform_machine == "AMD64") and extra == 'xpu'
 Requires-Dist: dpcpp-cpp-rt (==2024.0.2) ; (platform_system == "Windows") and extra == 'xpu'
 Requires-Dist: mkl-dpcpp (==2024.0.0) ; (platform_system == "Windows") and extra == 'xpu'
```

## Comparing `ipex_llm-2.1.0b20240524.dist-info/RECORD` & `ipex_llm-2.1.0b20240525.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -40,46 +40,46 @@
 ipex_llm/langchain/llms/__init__.py,sha256=vBCl9JF45vnk9CWBG1k8lp8J6F8OCR9UY2E-idkkm5Y,1636
 ipex_llm/langchain/llms/bigdlllm.py,sha256=FAZG6cAIJhRgbxm16gMq-cyBwLe-u165zE7yyxD7r9E,24438
 ipex_llm/langchain/llms/transformersllm.py,sha256=7eaIkJi1CbTCSgNxBCoZTe-o_5FYjD1GTYPWpn0Ccr4,10576
 ipex_llm/langchain/llms/transformerspipelinellm.py,sha256=vm522YPPwWxxAPVvQBtxRfBinC4hIbXdKW6VjHDaFXY,7379
 ipex_llm/langchain/vllm/__init__.py,sha256=T-EbRT6GJ_8RCu-iLmSzcftOimXSPQf2d5X72AUAy2Y,874
 ipex_llm/langchain/vllm/vllm.py,sha256=6dxc-ZISZQrJilEa_HA827l75Dv9rcHpY_G6FdJ8BVs,7793
 ipex_llm/libs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-ipex_llm/libs/bloom-api.dll,sha256=bRm91sf0JDYmDYW_qZdmB3dpOptgYY86TJsi5Kc_UVo,36352
-ipex_llm/libs/bloom.dll,sha256=bImhyKNYrDasl25lsqUXXCxZjGuG3idQIv8xMZAVBmo,473088
-ipex_llm/libs/chatglm_C.cp310-win_amd64.pyd,sha256=CtTZX_eoQqZOXw23LxvtSu1Wfv-a9gv32sQzsrWSuw0,854016
-ipex_llm/libs/chatglm_C.cp311-win_amd64.pyd,sha256=CIBpgFhCb6K19l0JmsKeO8P42-Uir5Vric_4_TN5hQY,856576
-ipex_llm/libs/chatglm_C.cp39-win_amd64.pyd,sha256=gIZKLFlzuxrN-9o4LUSeTbXVVxLdl_nE-4FIJh_bxtc,844288
-ipex_llm/libs/gptneox-api.dll,sha256=s6ZN-H2asqTUwB-htblOv1YnnR4EpCsQWNbtfGH7z_E,24576
-ipex_llm/libs/gptneox.dll,sha256=Vfg5OZif_zV72CX0yx-h8ikGJAXCVHkm7q4UzZ6WW-w,532992
-ipex_llm/libs/libbloom_avx.dll,sha256=xGVP9aEbIOCFX_LddvggLBnxjutXJuwFsOk5y6CguS8,499712
-ipex_llm/libs/libbloom_vnni.dll,sha256=TF0khSsYmrsU_FS4Ler23c-UaGFKZaMv5rBE9wEW-Hg,473600
-ipex_llm/libs/libgptneox_avx.dll,sha256=1hgfocXTEUgh1uYTHVCZ81CAshUuLQDuDeolWzAnc5c,559104
-ipex_llm/libs/libgptneox_vnni.dll,sha256=-cmfnXkFIjugHHYT_8hjy3Z4ScYd2XetEOseXuUWteM,533504
-ipex_llm/libs/libllama_avx.dll,sha256=U0H98zTpXJ8tLI25o6zKBSF79Cx5_ftqNdnz6eXVlRw,553472
-ipex_llm/libs/libllama_vnni.dll,sha256=FLANCH9HnHm8A8B2qETA6y-lXdEt0gt3mLuUJNLuT1I,527872
-ipex_llm/libs/libstarcoder_avx.dll,sha256=auX7iOlvkR6AumRhmlezM9yQuODRCOFM5ITAzEpcd_E,590848
-ipex_llm/libs/libstarcoder_vnni.dll,sha256=PeALaPTD0OgLSy_FbZaqN4M7XEjGNMOz9y_rVSllqcc,564736
-ipex_llm/libs/llama-api.dll,sha256=EsrS6ESutgDttE9JYN80sXApkgqC9Vr9onA5nOIPBUQ,25088
-ipex_llm/libs/llama.dll,sha256=ce14h2siogFgiFzpod0k9wZzFWgOKj1P56-sB3w9Y7Y,526848
-ipex_llm/libs/main-bloom.exe,sha256=RqrmVTLvM9rLTCnBlEMeaeWJ_Gi5MGbNSpWxuxwqU5o,103424
-ipex_llm/libs/main-chatglm_vnni.exe,sha256=7vGXZNINtBwV9z2yZoRaKnyLXOOSHOgexxcoZr8xwBk,726016
-ipex_llm/libs/main-gptneox.exe,sha256=XP-2Gv-UH-X4F0bj_OSS7AyvP2Ntl1gs3T8AxJBZOXo,98816
-ipex_llm/libs/main-llama.exe,sha256=p0sOtkUUgtzRW-bK_hgU98eouC-WVmBF4E0Tufn5vv8,99840
-ipex_llm/libs/main-starcoder.exe,sha256=hei-iz8QZVgJu6iQYC2cwYEZhKN7J4DNEhcbtNG-VCs,157696
-ipex_llm/libs/quantize-bloom.exe,sha256=xFiJPk7HIKzAyTS0mxtHCWkpWKKOe4c1hCB2SiZj2GA,126464
-ipex_llm/libs/quantize-bloom_vnni.exe,sha256=hmpffqZnT7Fe-2GoOrZC2uf7Kd2I93n9ITrveyaSw9k,127488
-ipex_llm/libs/quantize-gptneox.exe,sha256=CJ8uPX0VZCe5Pwfmy_csG6PtLscE3iNGUlaCHVH7SeQ,103936
-ipex_llm/libs/quantize-gptneox_vnni.exe,sha256=f4cR1URKNrB-yL_Jp7BXve-HMoLINCOJiSWoqBKEDRg,104448
-ipex_llm/libs/quantize-llama.exe,sha256=ALVGiI8OlZlgNprDvprB88BsAGcAF4nfUPWC05mhmxo,109056
-ipex_llm/libs/quantize-llama_vnni.exe,sha256=ObP-2k0Eqys9wlK-2MXId9NdujuqiBl1fgzg7-NooVc,110080
-ipex_llm/libs/quantize-starcoder.exe,sha256=Q3JDKisUjJZL79FExbL91sxJJ_dghxBo5qmjNif0vnY,126976
-ipex_llm/libs/quantize-starcoder_vnni.exe,sha256=r8HA0d2ArxStEXa3vTC-wCDbzgGyRGECFgDOznDbwG8,128512
-ipex_llm/libs/starcoder-api.dll,sha256=bqBsQQ9Kqjtaa_ztUEJl2OiseQPHD_c0ltfmHP_oyYM,21504
-ipex_llm/libs/starcoder.dll,sha256=CRypdFgeQrtX4H6wamQLcTzTDqUeLBB8R2ZTi326KOQ,564224
+ipex_llm/libs/bloom-api.dll,sha256=CXxhrBr0tAIopxickm_zi5UuSasxGXWShucCF_UJlGI,36352
+ipex_llm/libs/bloom.dll,sha256=4lRjVDSPH5u9L-p5pebTD39-shRfbyiXrNtjLTJhnf0,473088
+ipex_llm/libs/chatglm_C.cp310-win_amd64.pyd,sha256=nru9LGroOjJshrX5XzdmJduKAY1j9BPZvZgXRFnYDBY,854016
+ipex_llm/libs/chatglm_C.cp311-win_amd64.pyd,sha256=7nqggfU_xpljK-CbEhYKjzQkHvZjBUNTgKgQ4qcK_vQ,856576
+ipex_llm/libs/chatglm_C.cp39-win_amd64.pyd,sha256=jeFauFKRaf9horwbX1jPuGRjQuGHtBeB1xzGM9nFa2g,844288
+ipex_llm/libs/gptneox-api.dll,sha256=irzKrhYHXQQA4Snpjfc8oHLATBCwOQLvMR-hVTvn5Oo,24576
+ipex_llm/libs/gptneox.dll,sha256=c3xnbz2wDGCw2HJICbmwUYi-IzMq1pVEi9_Tin6jODM,532992
+ipex_llm/libs/libbloom_avx.dll,sha256=3FomBDPIbpjvvJIoM6-dujtZep0WX2BTIU4VU5Ty0fg,499712
+ipex_llm/libs/libbloom_vnni.dll,sha256=ssnJZQoPUAOjOdVp4m_bF5xCzt6pNR034VKrNVSzrhg,473600
+ipex_llm/libs/libgptneox_avx.dll,sha256=MoF5vvEmbsuNaC98DdcM_FlLA4hDVHpab6v1sSv1Llc,559104
+ipex_llm/libs/libgptneox_vnni.dll,sha256=HBQa5D27sR-bexnj-LVmb2ggmqFbD2t3eJpJaP7EsCE,533504
+ipex_llm/libs/libllama_avx.dll,sha256=t4S8DLDoJ2M9YXX_eRk7SZvvK1NhvezCVvnR83Es0ow,553472
+ipex_llm/libs/libllama_vnni.dll,sha256=1HVgE7IDqardiyxQSrRi1FZThrQUbx7Yz9oRb_igYQg,527872
+ipex_llm/libs/libstarcoder_avx.dll,sha256=O8CsVEMWKwsrUMCuWnVBJbyKaqIphfLwDDb-XaRqojg,590848
+ipex_llm/libs/libstarcoder_vnni.dll,sha256=O0FyXo4TpBExgMFyTF-IBKJmmbaNyAJqV2uqWU895L0,564736
+ipex_llm/libs/llama-api.dll,sha256=mkB6J93ZqJ1hbaKLWFL1Tlo-3xycNum_EA30are6RbQ,25088
+ipex_llm/libs/llama.dll,sha256=-WWsxorKALhXpRhzplWolSe-y2L-zGR_Auo0Cu9XdKg,526848
+ipex_llm/libs/main-bloom.exe,sha256=c2gsUgPtjYIa3KhibdT5yTfcfj7cVIdKjhP4vP0doio,103424
+ipex_llm/libs/main-chatglm_vnni.exe,sha256=iHbLG-10tWiPbJQ3aJ4AjsnADCAAMqaV2Xrr_T1GEJA,726016
+ipex_llm/libs/main-gptneox.exe,sha256=Ma0xgJxFoB2B4L1jDNtMvHDh-T84aAjytCfOGOh8hww,98816
+ipex_llm/libs/main-llama.exe,sha256=O-Kbt174ZzDjGcgyiSFqrAs353XLdwPOYo2VnqZ8XVA,99840
+ipex_llm/libs/main-starcoder.exe,sha256=1MzNeu3MlKXPWPKwECpuewJpyv2eYrqvF8iogLrmQ3E,157696
+ipex_llm/libs/quantize-bloom.exe,sha256=_ENIP36RKgeQaBeKdboB7G3emjJITpsLse2q-_aN-f8,126464
+ipex_llm/libs/quantize-bloom_vnni.exe,sha256=JedZZnqPl0retqOvszvERry4aPNtWDCob_hUSQQBtVM,127488
+ipex_llm/libs/quantize-gptneox.exe,sha256=xIsJMFQFmEHVTJ0nK6I8vc2RuOuMbjtKLoYQFQ-cMTw,103936
+ipex_llm/libs/quantize-gptneox_vnni.exe,sha256=uf45ZSvMfvlioG-Gt02lBrg8kQJszkHnqCpngDf3ZkA,104448
+ipex_llm/libs/quantize-llama.exe,sha256=DyRha9V-iC89ZWFr14tJk-6xDbum2ft79o9mF5GdvOE,109056
+ipex_llm/libs/quantize-llama_vnni.exe,sha256=ZeSIwGtCMtRMOogAyfvuyN5EuQ-lFNw9rBJrywCgJ5c,110080
+ipex_llm/libs/quantize-starcoder.exe,sha256=1g6TlU8PZEiMLDl5oDAElZqe3QDVdwiPb_qFk8RMyRw,126976
+ipex_llm/libs/quantize-starcoder_vnni.exe,sha256=2ydMhhp1JJbYZQR3113O01LxsaflajdvpfBmaW7L6bw,128512
+ipex_llm/libs/starcoder-api.dll,sha256=EQxOfUltoRoPByZHBpotWQ-TjGTNabSTPwU2ZQAC8Jk,21504
+ipex_llm/libs/starcoder.dll,sha256=zHh4RfBJimHfiCZHMsbY3OWcmsctGl8Fblr7NxqnJ_4,564224
 ipex_llm/llamaindex/__init__.py,sha256=T-EbRT6GJ_8RCu-iLmSzcftOimXSPQf2d5X72AUAy2Y,874
 ipex_llm/llamaindex/llms/__init__.py,sha256=KP1lEdGqDuxPoxL1ZSH25Pm2kKMPJBWUTLR0ckSLMIU,1139
 ipex_llm/llamaindex/llms/bigdlllm.py,sha256=FQBzq1KOjfc6uofTXAha3O7TqpJkNfOFepXQmOVlbnI,26314
 ipex_llm/serving/__init__.py,sha256=b2IXvVqQ5cItki021h8s3ymW12RPu8QNPprq4Mn3bDM,586
 ipex_llm/serving/fastchat/__init__.py,sha256=b2IXvVqQ5cItki021h8s3ymW12RPu8QNPprq4Mn3bDM,586
 ipex_llm/serving/fastchat/bigdl_llm_model.py,sha256=NXEN_3EPmcP3dDnvug4MokEXXE2zVUnENgBYxfubqic,10084
 ipex_llm/serving/fastchat/ipex_llm_worker.py,sha256=-nDeJIrGneosxjidzcQBMMkByLsRAM8kV70F5v8Kl10,19605
@@ -188,15 +188,15 @@
 ipex_llm/vllm/cpu/entrypoints/openai/api_server.py,sha256=NIeHHB8IcqmyA83sZEdKPhVM3vpJBupFuTFOuW2nj-Q,6944
 ipex_llm/vllm/xpu/__init__.py,sha256=zBSG6nzrVF5QnpR6_f7kPhBFeowTE9gaZ7D5m98E7_w,585
 ipex_llm/vllm/xpu/ipex_llm_gpu_executor.py,sha256=3lfClSuMWg6tfDmi_kCAI9zmc9_N5DINL-ZS6UHs0N0,18506
 ipex_llm/vllm/xpu/model_convert.py,sha256=lriPO5Ife5lMU6q5US4N6l9Y-iQmZa1fNGFPLXoVTuM,7172
 ipex_llm/vllm/xpu/engine/__init__.py,sha256=mzPVAyZdbvfzBQi-wxZh1sbme_NElPMmtrJ9C2zh8Us,747
 ipex_llm/vllm/xpu/engine/engine.py,sha256=6cRzT1UUoqbcaeLh-PigsRv881QavHIWUvHlB5miy3A,5953
 ipex_llm/vllm/xpu/entrypoints/openai/api_server.py,sha256=uIujXmuoKAcOcx5dz8DhnXpqpIlCgPz-4k-SfYKSvS0,10568
-ipex_llm-2.1.0b20240524.data/scripts/ipex-llm-init.bat,sha256=HPtCYuDYwEatq7dAwOvdfVcHYCpAVdbj75K1qh0vQek,2578
-ipex_llm-2.1.0b20240524.data/scripts/llm-chat.ps1,sha256=6qrs-hGVAV8IKh7Jx8nq_XrnZcjd7qGU5wndArM7Yag,2769
-ipex_llm-2.1.0b20240524.data/scripts/llm-cli.ps1,sha256=3qBtTLs_EjYDnM8YyCpJhzLnGCKTEGssu9UNqfkjVXs,3009
-ipex_llm-2.1.0b20240524.dist-info/METADATA,sha256=TWGGlY23SyP87rA9Xwofb0uYc9xw6QPKGt0avt4TYK0,5341
-ipex_llm-2.1.0b20240524.dist-info/WHEEL,sha256=bC8mYJUOJCh5KnyEeT6W_BCQYi3v39D3z64Vy_sFvVg,98
-ipex_llm-2.1.0b20240524.dist-info/entry_points.txt,sha256=TiUyBB2MRmfF3ko-pyAEzqeBCRnyhu27bNOAsWPp3e8,61
-ipex_llm-2.1.0b20240524.dist-info/top_level.txt,sha256=CGCMHM-SyqUabU4h8RqJ2KTYckQUO3LvIWwmUQ6Qbzw,9
-ipex_llm-2.1.0b20240524.dist-info/RECORD,,
+ipex_llm-2.1.0b20240525.data/scripts/ipex-llm-init.bat,sha256=HPtCYuDYwEatq7dAwOvdfVcHYCpAVdbj75K1qh0vQek,2578
+ipex_llm-2.1.0b20240525.data/scripts/llm-chat.ps1,sha256=6qrs-hGVAV8IKh7Jx8nq_XrnZcjd7qGU5wndArM7Yag,2769
+ipex_llm-2.1.0b20240525.data/scripts/llm-cli.ps1,sha256=3qBtTLs_EjYDnM8YyCpJhzLnGCKTEGssu9UNqfkjVXs,3009
+ipex_llm-2.1.0b20240525.dist-info/METADATA,sha256=Mr1vqhyz5CwYy9w5Ww3OtdEWRX9uiuZ5_2mYKZXHsK8,5341
+ipex_llm-2.1.0b20240525.dist-info/WHEEL,sha256=bC8mYJUOJCh5KnyEeT6W_BCQYi3v39D3z64Vy_sFvVg,98
+ipex_llm-2.1.0b20240525.dist-info/entry_points.txt,sha256=TiUyBB2MRmfF3ko-pyAEzqeBCRnyhu27bNOAsWPp3e8,61
+ipex_llm-2.1.0b20240525.dist-info/top_level.txt,sha256=CGCMHM-SyqUabU4h8RqJ2KTYckQUO3LvIWwmUQ6Qbzw,9
+ipex_llm-2.1.0b20240525.dist-info/RECORD,,
```

