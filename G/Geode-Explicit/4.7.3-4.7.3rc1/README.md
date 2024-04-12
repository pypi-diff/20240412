# Comparing `tmp/Geode_Explicit-4.7.3-cp39-cp39-win_amd64.whl.zip` & `tmp/Geode_Explicit-4.7.3rc1-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 3139273 bytes, number of entries: 12
--rw-rw-rw-  2.0 fat      194 b- defN 24-Apr-12 00:38 geode_explicit/__init__.py
--rw-rw-rw-  2.0 fat      271 b- defN 24-Apr-12 00:38 geode_explicit/brep.py
--rw-rw-rw-  2.0 fat      249 b- defN 24-Apr-12 00:38 geode_explicit/section.py
--rw-rw-rw-  2.0 fat  4022784 b- defN 24-Apr-12 00:39 geode_explicit/bin/Geode-Explicit_brep.dll
--rw-rw-rw-  2.0 fat    33792 b- defN 24-Apr-12 00:39 geode_explicit/bin/Geode-Explicit_common.dll
--rw-rw-rw-  2.0 fat  3715072 b- defN 24-Apr-12 00:39 geode_explicit/bin/Geode-Explicit_section.dll
--rw-rw-rw-  2.0 fat   147456 b- defN 24-Apr-12 00:39 geode_explicit/bin/geode_explicit_py_brep.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat   135680 b- defN 24-Apr-12 00:39 geode_explicit/bin/geode_explicit_py_section.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     2205 b- defN 24-Apr-12 00:39 Geode_Explicit-4.7.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 24-Apr-12 00:39 Geode_Explicit-4.7.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 24-Apr-12 00:39 Geode_Explicit-4.7.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1118 b- defN 24-Apr-12 00:39 Geode_Explicit-4.7.3.dist-info/RECORD
-12 files, 8058936 bytes uncompressed, 3137373 bytes compressed:  61.1%
+Zip file size: 3139283 bytes, number of entries: 12
+-rw-rw-rw-  2.0 fat      194 b- defN 24-Apr-11 17:33 geode_explicit/__init__.py
+-rw-rw-rw-  2.0 fat      271 b- defN 24-Apr-11 17:33 geode_explicit/brep.py
+-rw-rw-rw-  2.0 fat      249 b- defN 24-Apr-11 17:33 geode_explicit/section.py
+-rw-rw-rw-  2.0 fat  4022784 b- defN 24-Apr-11 17:34 geode_explicit/bin/Geode-Explicit_brep.dll
+-rw-rw-rw-  2.0 fat    33792 b- defN 24-Apr-11 17:34 geode_explicit/bin/Geode-Explicit_common.dll
+-rw-rw-rw-  2.0 fat  3715072 b- defN 24-Apr-11 17:34 geode_explicit/bin/Geode-Explicit_section.dll
+-rw-rw-rw-  2.0 fat   147456 b- defN 24-Apr-11 17:34 geode_explicit/bin/geode_explicit_py_brep.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   135680 b- defN 24-Apr-11 17:34 geode_explicit/bin/geode_explicit_py_section.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     2211 b- defN 24-Apr-11 17:34 Geode_Explicit-4.7.3rc1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 24-Apr-11 17:34 Geode_Explicit-4.7.3rc1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       15 b- defN 24-Apr-11 17:34 Geode_Explicit-4.7.3rc1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1130 b- defN 24-Apr-11 17:34 Geode_Explicit-4.7.3rc1.dist-info/RECORD
+12 files, 8058954 bytes uncompressed, 3137359 bytes compressed:  61.1%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: geode_explicit/bin/geode_explicit_py_brep.cp39-win_amd64.pyd
 Comment: 
 
 Filename: geode_explicit/bin/geode_explicit_py_section.cp39-win_amd64.pyd
 Comment: 
 
-Filename: Geode_Explicit-4.7.3.dist-info/METADATA
+Filename: Geode_Explicit-4.7.3rc1.dist-info/METADATA
 Comment: 
 
-Filename: Geode_Explicit-4.7.3.dist-info/WHEEL
+Filename: Geode_Explicit-4.7.3rc1.dist-info/WHEEL
 Comment: 
 
-Filename: Geode_Explicit-4.7.3.dist-info/top_level.txt
+Filename: Geode_Explicit-4.7.3rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: Geode_Explicit-4.7.3.dist-info/RECORD
+Filename: Geode_Explicit-4.7.3rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## geode_explicit/bin/Geode-Explicit_brep.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001802e2424
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Fri Apr 12 00:39:18 2024
+Time/Date		Thu Apr 11 17:34:20 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		00000000002e6600
 SizeOfInitializedData	00000000000f2000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000002e2424
@@ -86953,30 +86953,30 @@
 	reloc   62 offset  bc0 [384bc0] DIR64
 	reloc   63 offset  bc8 [384bc8] DIR64
 	reloc   64 offset  bd0 [384bd0] DIR64
 	reloc   65 offset  bd8 [384bd8] DIR64
 	reloc   66 offset  be0 [384be0] DIR64
 	reloc   67 offset  be8 [384be8] DIR64
 	reloc   68 offset  bf0 [384bf0] DIR64
-	reloc   69 offset  c10 [384c10] DIR64
-	reloc   70 offset  c18 [384c18] DIR64
-	reloc   71 offset  c20 [384c20] DIR64
-	reloc   72 offset  c28 [384c28] DIR64
-	reloc   73 offset  c30 [384c30] DIR64
-	reloc   74 offset  c38 [384c38] DIR64
-	reloc   75 offset  c40 [384c40] DIR64
-	reloc   76 offset  c48 [384c48] DIR64
-	reloc   77 offset  c50 [384c50] DIR64
-	reloc   78 offset  c58 [384c58] DIR64
-	reloc   79 offset  c60 [384c60] DIR64
-	reloc   80 offset  c68 [384c68] DIR64
-	reloc   81 offset  c70 [384c70] DIR64
-	reloc   82 offset  c78 [384c78] DIR64
-	reloc   83 offset  c80 [384c80] DIR64
-	reloc   84 offset  c88 [384c88] DIR64
+	reloc   69 offset  bf8 [384bf8] DIR64
+	reloc   70 offset  c00 [384c00] DIR64
+	reloc   71 offset  c08 [384c08] DIR64
+	reloc   72 offset  c10 [384c10] DIR64
+	reloc   73 offset  c18 [384c18] DIR64
+	reloc   74 offset  c20 [384c20] DIR64
+	reloc   75 offset  c28 [384c28] DIR64
+	reloc   76 offset  c30 [384c30] DIR64
+	reloc   77 offset  c38 [384c38] DIR64
+	reloc   78 offset  c40 [384c40] DIR64
+	reloc   79 offset  c48 [384c48] DIR64
+	reloc   80 offset  c50 [384c50] DIR64
+	reloc   81 offset  c58 [384c58] DIR64
+	reloc   82 offset  c60 [384c60] DIR64
+	reloc   83 offset  c68 [384c68] DIR64
+	reloc   84 offset  c70 [384c70] DIR64
 	reloc   85 offset  c90 [384c90] DIR64
 	reloc   86 offset  c98 [384c98] DIR64
 	reloc   87 offset  ca0 [384ca0] DIR64
 	reloc   88 offset  ca8 [384ca8] DIR64
 	reloc   89 offset  cb0 [384cb0] DIR64
 	reloc   90 offset  cd0 [384cd0] DIR64
 	reloc   91 offset  cd8 [384cd8] DIR64
@@ -359472,15 +359472,15 @@
    180132b7f:	test   %rax,%rax
    180132b82:	je     0x180132bad
    180132b84:	movq   $0x1,(%rax)
    180132b8b:	mov    %r15b,0x8(%rax)
    180132b8f:	xor    %eax,%eax
    180132b91:	mov    %rax,0x10(%rbx)
    180132b95:	mov    %r15,0x10(%rbx)
-   180132b99:	lea    0x252010(%rip),%rax        # 0x180384bb0
+   180132b99:	lea    0x252050(%rip),%rax        # 0x180384bf0
    180132ba0:	mov    %rax,0x18(%rbx)
    180132ba4:	mov    %rsi,0x100(%rbx)
    180132bab:	jmp    0x180132bb0
    180132bad:	mov    %r15,%rbx
    180132bb0:	mov    %rbx,-0x60(%rbp)
    180132bb4:	mov    %r15,-0x30(%rbp)
    180132bb8:	mov    (%rbx),%rax
@@ -359531,15 +359531,15 @@
    180132c67:	test   %rax,%rax
    180132c6a:	je     0x180132c95
    180132c6c:	movq   $0x1,(%rax)
    180132c73:	movb   $0x0,0x8(%rax)
    180132c77:	xor    %eax,%eax
    180132c79:	mov    %rax,0x10(%rbx)
    180132c7d:	mov    %r15,0x10(%rbx)
-   180132c81:	lea    0x251f88(%rip),%rax        # 0x180384c10
+   180132c81:	lea    0x252008(%rip),%rax        # 0x180384c90
    180132c88:	mov    %rax,0x18(%rbx)
    180132c8c:	mov    %rsi,0x100(%rbx)
    180132c93:	jmp    0x180132c98
    180132c95:	mov    %r15,%rbx
    180132c98:	mov    %rbx,-0x50(%rbp)
    180132c9c:	mov    %r15,-0x28(%rbp)
    180132ca0:	mov    (%rbx),%rax
@@ -359591,15 +359591,15 @@
    180132d54:	test   %rax,%rax
    180132d57:	je     0x180132d82
    180132d59:	movq   $0x1,(%rax)
    180132d60:	movb   $0x0,0x8(%rax)
    180132d64:	xor    %eax,%eax
    180132d66:	mov    %rax,0x10(%rbx)
    180132d6a:	mov    %r15,0x10(%rbx)
-   180132d6e:	lea    0x251ebb(%rip),%rax        # 0x180384c30
+   180132d6e:	lea    0x251f5b(%rip),%rax        # 0x180384cd0
    180132d75:	mov    %rax,0x18(%rbx)
    180132d79:	mov    %rsi,0x100(%rbx)
    180132d80:	jmp    0x180132d85
    180132d82:	mov    %r15,%rbx
    180132d85:	mov    %rbx,-0x40(%rbp)
    180132d89:	mov    %r15,-0x20(%rbp)
    180132d8d:	mov    (%rbx),%rax
@@ -359651,15 +359651,15 @@
    180132e41:	test   %rax,%rax
    180132e44:	je     0x180132e6f
    180132e46:	movq   $0x1,(%rax)
    180132e4d:	movb   $0x0,0x8(%rax)
    180132e51:	xor    %eax,%eax
    180132e53:	mov    %rax,0x10(%rbx)
    180132e57:	mov    %r15,0x10(%rbx)
-   180132e5b:	lea    0x251e6e(%rip),%rax        # 0x180384cd0
+   180132e5b:	lea    0x251d4e(%rip),%rax        # 0x180384bb0
    180132e62:	mov    %rax,0x18(%rbx)
    180132e66:	mov    %rsi,0x100(%rbx)
    180132e6d:	jmp    0x180132e72
    180132e6f:	mov    %r15,%rbx
    180132e72:	mov    %rbx,-0x18(%rbp)
    180132e76:	mov    %r15,0x58(%rsp)
    180132e7b:	mov    (%rbx),%rax
@@ -367768,15 +367768,15 @@
    18013a966:	mov    %eax,0x40(%rsp)
    18013a96a:	mov    0x70(%rsp),%rax
    18013a96f:	shr    $0x20,%rax
    18013a973:	test   %eax,%eax
    18013a975:	je     0x18013aab4
    18013a97b:	lea    0x50(%rsp),%rax
    18013a980:	mov    %rax,0x68(%rsp)
-   18013a985:	lea    0x24a2e4(%rip),%r13        # 0x180384c70
+   18013a985:	lea    0x24a244(%rip),%r13        # 0x180384bd0
    18013a98c:	mov    0x38(%rsp),%edx
    18013a990:	mov    %r15,-0x60(%rbp)
    18013a994:	mov    %edx,-0x58(%rbp)
    18013a997:	lea    0xe8(%rbp),%rax
    18013a99e:	mov    %rax,-0x50(%rbp)
    18013a9a2:	mov    %r14,-0x48(%rbp)
    18013a9a6:	call   *0x1ae99c(%rip)        # 0x1802e9348
@@ -398397,15 +398397,15 @@
    1801555ad:	je     0x1801555d2
    1801555af:	mov    $0x1,%r14d
    1801555b5:	mov    %r14,(%rax)
    1801555b8:	mov    %bl,0x8(%rax)
    1801555bb:	xor    %eax,%eax
    1801555bd:	mov    %rax,0x10(%rdi)
    1801555c1:	mov    %rbx,0x10(%rdi)
-   1801555c5:	lea    0x22f6e4(%rip),%rcx        # 0x180384cb0
+   1801555c5:	lea    0x22f6a4(%rip),%rcx        # 0x180384c70
    1801555cc:	mov    %rcx,0x18(%rdi)
    1801555d0:	jmp    0x1801555d5
    1801555d2:	mov    %rbx,%rdi
    1801555d5:	mov    (%rsi),%rcx
    1801555d8:	test   %rcx,%rcx
    1801555db:	je     0x1801555f9
    1801555dd:	mov    $0xffffffffffffffff,%r14
@@ -398444,15 +398444,15 @@
    18015566b:	test   %rax,%rax
    18015566e:	je     0x18015568e
    180155670:	mov    %r14,(%rax)
    180155673:	movb   $0x0,0x8(%rax)
    180155677:	xor    %ecx,%ecx
    180155679:	mov    %rcx,0x10(%rax)
    18015567d:	mov    %rbx,0x10(%rax)
-   180155681:	lea    0x22f628(%rip),%rcx        # 0x180384cb0
+   180155681:	lea    0x22f5e8(%rip),%rcx        # 0x180384c70
    180155688:	mov    %rcx,0x18(%rax)
    18015568c:	jmp    0x180155691
    18015568e:	mov    %rbx,%rax
    180155691:	mov    %rax,0x0(%r13)
    180155695:	movb   $0x0,0x9(%rax)
    180155699:	mov    0xe8(%rsp),%rdx
    1801556a1:	lea    0x10(%rdx),%rcx
@@ -404779,15 +404779,15 @@
    18015ac69:	test   %rax,%rax
    18015ac6c:	je     0x18015aca9
    18015ac6e:	movq   $0x1,(%rax)
    18015ac75:	mov    %r15b,0x8(%rax)
    18015ac79:	xor    %eax,%eax
    18015ac7b:	mov    %rax,0x10(%rsi)
    18015ac7f:	mov    %r15,0x10(%rsi)
-   18015ac83:	lea    0x229f46(%rip),%rax        # 0x180384bd0
+   18015ac83:	lea    0x229fc6(%rip),%rax        # 0x180384c50
    18015ac8a:	mov    %rax,0x18(%rsi)
    18015ac8e:	movups (%rbx),%xmm0
    18015ac91:	movups %xmm0,0x40(%rsi)
    18015ac95:	mov    0x80(%rsp),%rcx
    18015ac9d:	mov    (%rcx),%rax
    18015aca0:	mov    %rax,0x50(%rsi)
    18015aca4:	mov    %r15,(%rcx)
@@ -404878,15 +404878,15 @@
    18015ada9:	test   %rax,%rax
    18015adac:	je     0x18015adf3
    18015adae:	movq   $0x1,(%rax)
    18015adb5:	mov    %r15b,0x8(%rax)
    18015adb9:	xor    %eax,%eax
    18015adbb:	mov    %rax,0x10(%rsi)
    18015adbf:	mov    %r15,0x10(%rsi)
-   18015adc3:	lea    0x229e86(%rip),%rax        # 0x180384c50
+   18015adc3:	lea    0x229e66(%rip),%rax        # 0x180384c30
    18015adca:	mov    %rax,0x18(%rsi)
    18015adce:	movups (%rbx),%xmm0
    18015add1:	movups %xmm0,0x40(%rsi)
    18015add5:	movsd  0x10(%rbx),%xmm1
    18015adda:	movsd  %xmm1,0x50(%rsi)
    18015addf:	mov    0x80(%rsp),%rcx
    18015ade7:	mov    (%rcx),%rax
@@ -407569,15 +407569,15 @@
    18015d1c9:	test   %rax,%rax
    18015d1cc:	je     0x18015d215
    18015d1ce:	movq   $0x1,(%rax)
    18015d1d5:	mov    %r15b,0x8(%rax)
    18015d1d9:	xor    %eax,%eax
    18015d1db:	mov    %rax,0x10(%rsi)
    18015d1df:	mov    %r15,0x10(%rsi)
-   18015d1e3:	lea    0x227aa6(%rip),%rax        # 0x180384c90
+   18015d1e3:	lea    0x227a26(%rip),%rax        # 0x180384c10
    18015d1ea:	mov    %rax,0x18(%rsi)
    18015d1ee:	mov    (%rbx),%rax
    18015d1f1:	mov    %rax,0x40(%rsi)
    18015d1f5:	mov    0x8(%rbx),%rax
    18015d1f9:	mov    %rax,0x48(%rsi)
    18015d1fd:	mov    %r15,0x8(%rbx)
    18015d201:	mov    0x80(%rsp),%rcx
@@ -1081373,93 +1081373,92 @@
    180384ba3:	insb   (%dx),%es:(%rdi)
    180384ba4:	imul   $0x74,0x69(%rbx),%esp
    180384bab:	add    %bh,%bh
    180384bad:	(bad)
    180384bae:	(bad)
    180384baf:	call   *-0x1c(%rax)
    180384bb2:	adc    $0x180,%eax
-   180384bb7:	add    %dl,0x18015e6(%rax)
+   180384bb7:	add    %dh,0x18015e4(%rax)
    180384bbd:	add    %al,(%rax)
    180384bbf:	add    %dl,0x18015df(%rax)
    180384bc5:	add    %al,(%rax)
    180384bc7:	add    %al,-0x21(%rax)
    180384bca:	adc    $0x180,%eax
-   180384bcf:	add    %al,0x1801618(%rax)
-   180384bd5:	add    %al,(%rax)
-   180384bd7:	add    %ah,0x19(%rax)
-   180384bda:	(bad)
-   180384bdb:	addb   $0x0,(%rcx)
-   180384bde:	add    %al,(%rax)
-   180384be0:	lock sbb %dl,(%rsi)
-   180384be3:	addb   $0x0,(%rcx)
-   180384be6:	add    %al,(%rax)
-   180384be8:	rex fists 0x180(%rip)        # 0x180384d6f
-   180384bef:	add    %dh,-0x19(%rax)
+   180384bcf:	add    %ah,%al
+   180384bd1:	ficoms 0x180(%rip)        # 0x180384d57
+   180384bd7:	add    %dl,%al
+   180384bd9:	fists  0x180(%rip)        # 0x180384d5f
+   180384bdf:	add    %dl,0x18015df(%rax)
+   180384be5:	add    %al,(%rax)
+   180384be7:	add    %al,-0x21(%rax)
+   180384bea:	adc    $0x180,%eax
+   180384bef:	add    %dl,-0x1c(%rax)
    180384bf2:	adc    $0x180,%eax
-	...
-   180384c0f:	add    %dl,-0x1c(%rax)
-   180384c12:	adc    $0x180,%eax
-   180384c17:	add    %dh,0x18015e5(%rax)
-   180384c1d:	add    %al,(%rax)
-   180384c1f:	add    %dl,0x18015df(%rax)
-   180384c25:	add    %al,(%rax)
-   180384c27:	add    %al,-0x21(%rax)
-   180384c2a:	adc    $0x180,%eax
-   180384c2f:	add    %dl,-0x1c(%rax)
-   180384c32:	adc    $0x180,%eax
-   180384c37:	add    %dl,0x18015e5(%rax)
-   180384c3d:	add    %al,(%rax)
-   180384c3f:	add    %dl,0x18015df(%rax)
-   180384c45:	add    %al,(%rax)
-   180384c47:	add    %al,-0x21(%rax)
-   180384c4a:	adc    $0x180,%eax
-   180384c4f:	add    %dl,%al
-   180384c51:	(bad)
-   180384c52:	(bad)
-   180384c53:	addb   $0x0,(%rcx)
-   180384c56:	add    %al,(%rax)
-   180384c58:	mov    $0x17,%al
+   180384bf7:	add    %dl,0x18015e6(%rax)
+   180384bfd:	add    %al,(%rax)
+   180384bff:	add    %dl,0x18015df(%rax)
+   180384c05:	add    %al,(%rax)
+   180384c07:	add    %al,-0x21(%rax)
+   180384c0a:	adc    $0x180,%eax
+   180384c0f:	add    %al,%al
+   180384c11:	ss (bad)
+   180384c13:	addb   $0x0,(%rcx)
+   180384c16:	add    %al,(%rax)
+   180384c18:	loopne 0x180384c51
+   180384c1a:	(bad)
+   180384c1b:	addb   $0x0,(%rcx)
+   180384c1e:	add    %al,(%rax)
+   180384c20:	jo     0x180384c59
+   180384c22:	(bad)
+   180384c23:	addb   $0x0,(%rcx)
+   180384c26:	add    %al,(%rax)
+   180384c28:	xor    %dh,(%rdi)
+   180384c2a:	(bad)
+   180384c2b:	addb   $0x0,(%rcx)
+   180384c2e:	add    %al,(%rax)
+   180384c30:	rclb   $1,(%rsi)
+   180384c32:	(bad)
+   180384c33:	addb   $0x0,(%rcx)
+   180384c36:	add    %al,(%rax)
+   180384c38:	mov    $0x17,%al
+   180384c3a:	(bad)
+   180384c3b:	addb   $0x0,(%rcx)
+   180384c3e:	add    %al,(%rax)
+   180384c40:	rex (bad)
+   180384c42:	(bad)
+   180384c43:	addb   $0x0,(%rcx)
+   180384c46:	add    %al,(%rax)
+   180384c48:	rex fists 0x180(%rip)        # 0x180384dcf
+   180384c4f:	add    %al,0x1801618(%rax)
+   180384c55:	add    %al,(%rax)
+   180384c57:	add    %ah,0x19(%rax)
    180384c5a:	(bad)
    180384c5b:	addb   $0x0,(%rcx)
    180384c5e:	add    %al,(%rax)
-   180384c60:	rex (bad)
-   180384c62:	(bad)
+   180384c60:	lock sbb %dl,(%rsi)
    180384c63:	addb   $0x0,(%rcx)
    180384c66:	add    %al,(%rax)
    180384c68:	rex fists 0x180(%rip)        # 0x180384def
-   180384c6f:	add    %ah,%al
-   180384c71:	ficoms 0x180(%rip)        # 0x180384df7
-   180384c77:	add    %dl,%al
-   180384c79:	fists  0x180(%rip)        # 0x180384dff
-   180384c7f:	add    %dl,0x18015df(%rax)
-   180384c85:	add    %al,(%rax)
-   180384c87:	add    %al,-0x21(%rax)
-   180384c8a:	adc    $0x180,%eax
-   180384c8f:	add    %al,%al
-   180384c91:	ss (bad)
-   180384c93:	addb   $0x0,(%rcx)
-   180384c96:	add    %al,(%rax)
-   180384c98:	loopne 0x180384cd1
-   180384c9a:	(bad)
-   180384c9b:	addb   $0x0,(%rcx)
-   180384c9e:	add    %al,(%rax)
-   180384ca0:	jo     0x180384cd9
-   180384ca2:	(bad)
-   180384ca3:	addb   $0x0,(%rcx)
-   180384ca6:	add    %al,(%rax)
-   180384ca8:	xor    %dh,(%rdi)
-   180384caa:	(bad)
-   180384cab:	addb   $0x0,(%rcx)
-   180384cae:	add    %al,(%rax)
-   180384cb0:	movabs 0x18015b8,%al
+   180384c6f:	add    %ah,0x18015b8(%rax)
+	...
+   180384c8d:	add    %al,(%rax)
+   180384c8f:	add    %dl,-0x1c(%rax)
+   180384c92:	adc    $0x180,%eax
+   180384c97:	add    %dh,0x18015e5(%rax)
+   180384c9d:	add    %al,(%rax)
+   180384c9f:	add    %dl,0x18015df(%rax)
+   180384ca5:	add    %al,(%rax)
+   180384ca7:	add    %al,-0x21(%rax)
+   180384caa:	adc    $0x180,%eax
+   180384caf:	add    %dh,-0x19(%rax)
+   180384cb2:	adc    $0x180,%eax
 	...
-   180384ccd:	add    %al,(%rax)
    180384ccf:	add    %dl,-0x1c(%rax)
    180384cd2:	adc    $0x180,%eax
-   180384cd7:	add    %dh,0x18015e4(%rax)
+   180384cd7:	add    %dl,0x18015e5(%rax)
    180384cdd:	add    %al,(%rax)
    180384cdf:	add    %dl,0x18015df(%rax)
    180384ce5:	add    %al,(%rax)
    180384ce7:	add    %al,-0x21(%rax)
    180384cea:	adc    $0x180,%eax
    180384cef:	add    %bh,%cl
    180384cf1:	rex.WR cmp %r8b,0x1(%rax)
@@ -1082071,15 +1082070,16 @@
    18038536a:	(bad)
    18038536b:	(bad)
    18038536c:	(bad)
    18038536d:	(bad)
    18038536e:	(bad)
    18038536f:	incl   (%rax)
    180385371:	add    %al,(%rax)
-   180385373:	add    %dh,0x661882(%rsi)
+   180385373:	add    %bl,(%rdi,%rbx,1)
+   180385376:	sbb    %ah,0x0(%rsi)
    180385379:	add    %al,(%rax)
    18038537b:	add    %cl,-0x78000000(%rip)        # 0x108385381
    180385381:	add    (%rax),%eax
    180385383:	add    %cl,0x688c0038(%rsi,%rdi,2)
    18038538a:	cmp    %al,(%rax)
    18038538c:	add    %al,(%rax)
    18038538e:	add    %al,(%rax)
@@ -1209064,27 +1209064,32 @@
    1803db1c9:	stos   %eax,%es:(%rdi)
    1803db1ca:	cwtl
    1803db1cb:	stos   %eax,%es:(%rdi)
    1803db1cc:	mov    $0xab,%al
    1803db1ce:	mov    $0xc8abc0ab,%eax
    1803db1d3:	stos   %eax,%es:(%rdi)
    1803db1d4:	shrb   $1,-0x541f5428(%rbx)
-   1803db1da:	call   0x190e9a28a
-   1803db1df:	lods   %ds:(%rsi),%al
-   1803db1e0:	sbb    %ch,0x30ac28ac(%rax,%riz,1)
+   1803db1da:	call   0x178e9a28a
+   1803db1df:	stos   %eax,%es:(%rdi)
+   1803db1e0:	add    %ch,0x18ac10ac(%rax,%rcx,1)
    1803db1e7:	lods   %ds:(%rsi),%al
-   1803db1e8:	cmp    %ch,0x50ac48ac(%rax,%rax,2)
+   1803db1e8:	and    %ch,0x38ac30ac(%rax,%rbp,1)
    1803db1ef:	lods   %ds:(%rsi),%al
-   1803db1f0:	pop    %rax
-   1803db1f1:	lods   %ds:(%rsi),%al
-   1803db1f2:	(bad)
-   1803db1f3:	lods   %ds:(%rsi),%al
-   1803db1f4:	push   $0x78ac70ac
+   1803db1f0:	rex lods %ds:(%rsi),%al
+   1803db1f2:	rex.W lods %ds:(%rsi),%al
+   1803db1f4:	push   %rax
+   1803db1f5:	lods   %ds:(%rsi),%al
+   1803db1f6:	pop    %rax
+   1803db1f7:	lods   %ds:(%rsi),%al
+   1803db1f8:	(bad)
    1803db1f9:	lods   %ds:(%rsi),%al
-   1803db1fa:	subb   $0xac,-0x67536f54(%rax,%rcx,4)
+   1803db1fa:	push   $0xffffffff90ac70ac
+   1803db1ff:	lods   %ds:(%rsi),%al
+   1803db200:	cwtl
+   1803db201:	lods   %ds:(%rsi),%al
    1803db202:	movabs 0xd8acd0acb0aca8ac,%al
    1803db20b:	lods   %ds:(%rsi),%al
    1803db20c:	loopne 0x1803db1ba
    1803db20e:	call   0x180eaa2bf
    1803db213:	lods   %ds:(%rsi),%eax
    1803db214:	or     %ch,-0x52e752f0(%rbp)
    1803db21a:	and    %ch,-0x52cf52d8(%rbp)
```

## geode_explicit/bin/Geode-Explicit_common.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180004178
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Fri Apr 12 00:38:52 2024
+Time/Date		Thu Apr 11 17:34:00 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		0000000000004000
 SizeOfInitializedData	0000000000004600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000004178
@@ -6760,17 +6760,19 @@
    180005532:	(bad)
    180005533:	(bad)
    180005534:	(bad)
    180005535:	ljmp   (bad)
    180005536:	out    %eax,(%dx)
    180005537:	jg     0x180005539
    180005539:	add    %al,(%rax)
-   18000553b:	add    %bl,0x6618(%rdx,%rax,4)
-   180005542:	add    %al,(%rax)
-   180005544:	or     $0xa4000000,%eax
+   18000553b:	add    %cl,(%rax)
+   18000553d:	(bad)
+   18000553e:	sbb    %ah,0x0(%rsi)
+   180005541:	add    %al,(%rax)
+   180005543:	add    %cl,-0x5c000000(%rip)        # 0x124005549
    180005549:	add    (%rax),%al
    18000554b:	add    %dl,0x0(%rbx,%rbx,2)
    18000554f:	add    %dl,0x0(%rdi,%rcx,2)
 	...
    18000555f:	add    %bh,(%rax)
    180005561:	add    %eax,(%rax)
 	...
```

## geode_explicit/bin/Geode-Explicit_section.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001802a9d78
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Fri Apr 12 00:38:57 2024
+Time/Date		Thu Apr 11 17:34:04 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		00000000002aba00
 SizeOfInitializedData	00000000000e1a00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000002a9d78
@@ -1001380,15 +1001380,16 @@
    18034900a:	(bad)
    18034900b:	(bad)
    18034900c:	(bad)
    18034900d:	(bad)
    18034900e:	(bad)
    18034900f:	incl   (%rax)
    180349011:	add    %al,(%rax)
-   180349013:	add    %ah,0x661882(%rcx)
+   180349013:	add    %cl,(%rdi,%rbx,1)
+   180349016:	sbb    %ah,0x0(%rsi)
    180349019:	add    %al,(%rax)
    18034901b:	add    %cl,-0x78000000(%rip)        # 0x108349021
    180349021:	add    (%rax),%eax
    180349023:	add    %cl,-0x54(%rax)
    180349026:	xor    $0x0,%al
    180349028:	rex.W (bad)
    18034902a:	xor    $0x0,%al
```

## Comparing `Geode_Explicit-4.7.3.dist-info/METADATA` & `Geode_Explicit-4.7.3rc1.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: Geode-Explicit
-Version: 4.7.3
+Version: 4.7.3rc1
 Summary: Geode-solutions OpenGeode module for building explicit models
 Home-page: https://github.com/Geode-solutions/Geode-Explicit
 Author: Geode-solutions
 Author-email: contact@geode-solutions.com
 License: Proprietary
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Requires-Dist: geode-background ==7.*,>=7.9.6
 Requires-Dist: geode-common ==31.*,>=31.0.6
 Requires-Dist: geode-conversion ==5.*,>=5.2.8
-Requires-Dist: opengeode-core ==14.*,>=14.18.3
+Requires-Dist: opengeode-core ==14.*,>=14.18.3rc1
 Requires-Dist: opengeode-inspector ==5.*,>=5.0.5
 
 <h1 align="center">Geode-Explicit<sup><i>by Geode-solutions</i></sup></h1>
 <h3 align="center">Geode-solutions OpenGeode module for building explicit models</h3>
 
 <p align="center">
   <img src="https://github.com/Geode-solutions/Geode-Explicit_private/workflows/CI/badge.svg" alt="Build Status">
```

### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: Geode-Explicit Version: 4.7.3 Summary: Geode-
+Metadata-Version: 2.1 Name: Geode-Explicit Version: 4.7.3rc1 Summary: Geode-
 solutions OpenGeode module for building explicit models Home-page: https://
 github.com/Geode-solutions/Geode-Explicit Author: Geode-solutions Author-email:
 contact@geode-solutions.com License: Proprietary Platform: UNKNOWN Description-
 Content-Type: text/markdown Requires-Dist: geode-background ==7.*,>=7.9.6
 Requires-Dist: geode-common ==31.*,>=31.0.6 Requires-Dist: geode-conversion
-==5.*,>=5.2.8 Requires-Dist: opengeode-core ==14.*,>=14.18.3 Requires-Dist:
+==5.*,>=5.2.8 Requires-Dist: opengeode-core ==14.*,>=14.18.3rc1 Requires-Dist:
 opengeode-inspector ==5.*,>=5.0.5
                 ************ GGeeooddee--EExxpplliicciittbbyy GGeeooddee--ssoolluuttiioonnss ************
     ******** GGeeooddee--ssoolluuttiioonnss OOppeennGGeeooddee mmoodduullee ffoorr bbuuiillddiinngg eexxpplliicciitt mmooddeellss ********
             [Build Status][Deploy Status][Coverage Status][Version]
               [Windows support][Ubuntu support][Red Hat support]
  [Language][License][Semantic-release]_[_S_l_a_c_k_ _i_n_v_i_t_e_]Copyright (c) 2019 - 2024,
                                 Geode-solutions
```

## Comparing `Geode_Explicit-4.7.3.dist-info/RECORD` & `Geode_Explicit-4.7.3rc1.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 geode_explicit/__init__.py,sha256=3IEZJDMtMfFSTtDJOl8tpLIg5P9Iytnx2bE1I6Gg8qo,194
 geode_explicit/brep.py,sha256=i4sDZvKY0NnpwATBxQHOq2egAGLbxDH5u4iZqCHMOlk,271
 geode_explicit/section.py,sha256=k_Q35aAqi_ZAP004Xc86lQf4FSYA2u0kU6y1_iR9Ahk,249
-geode_explicit/bin/Geode-Explicit_brep.dll,sha256=YbjJ-j5h7HgmiqGT3e0YddhsNpDYDJsFOhlju705k3Y,4022784
-geode_explicit/bin/Geode-Explicit_common.dll,sha256=O_-Gh7NAwZRSvIMyd223Hz2pEL9gsGTmxZnMU0k2uDw,33792
-geode_explicit/bin/Geode-Explicit_section.dll,sha256=bFiNkpVIpvtJrurF4tzwH36Qwo9s0dBhV-B8ig9IAq0,3715072
-geode_explicit/bin/geode_explicit_py_brep.cp39-win_amd64.pyd,sha256=kSrnKbDgebPhyS4PIB5fFLqhD66cFDh4I6xC-ToFfmc,147456
-geode_explicit/bin/geode_explicit_py_section.cp39-win_amd64.pyd,sha256=64aBN1OxE89YSlLnITsz8p6WMUPPR90xrljDa_dx3iA,135680
-Geode_Explicit-4.7.3.dist-info/METADATA,sha256=3-rKSo-FEg-v0-pdx_OKWppWjxKICtOOEP2OvXLkWqM,2205
-Geode_Explicit-4.7.3.dist-info/WHEEL,sha256=Z6c-bE0pUM47a70GvqO_SvH_XXU0lm62gEAKtoNJ08A,100
-Geode_Explicit-4.7.3.dist-info/top_level.txt,sha256=SLuJS840PQSB1EAIYibu72OEG1sORAkOdcw3z29RuQQ,15
-Geode_Explicit-4.7.3.dist-info/RECORD,,
+geode_explicit/bin/Geode-Explicit_brep.dll,sha256=0DRpRffwx7Z36qOKYKfxSIlFMeKb2r7rUQ70gv0ibWU,4022784
+geode_explicit/bin/Geode-Explicit_common.dll,sha256=Fa9-kubCY-fJwSFtjorJEGfZWcEoO1nS-Yf6hd-fDV0,33792
+geode_explicit/bin/Geode-Explicit_section.dll,sha256=U7I2MngD1l6_iqeUIjB_93aEtLlGeUUNeLJZfQOXPPU,3715072
+geode_explicit/bin/geode_explicit_py_brep.cp39-win_amd64.pyd,sha256=ZiCNs20P5vGpx_ouoMJAyOeEHbD8bpYgkGoBwLEExEA,147456
+geode_explicit/bin/geode_explicit_py_section.cp39-win_amd64.pyd,sha256=cjxL5x0wdifsusk7X-kz_JBfsCxXBDQsPUnylp4VRJw,135680
+Geode_Explicit-4.7.3rc1.dist-info/METADATA,sha256=RJ9HbJYqJjFH0TedOmHqnBZZlp54laHeH3CeKZU6f2I,2211
+Geode_Explicit-4.7.3rc1.dist-info/WHEEL,sha256=Z6c-bE0pUM47a70GvqO_SvH_XXU0lm62gEAKtoNJ08A,100
+Geode_Explicit-4.7.3rc1.dist-info/top_level.txt,sha256=SLuJS840PQSB1EAIYibu72OEG1sORAkOdcw3z29RuQQ,15
+Geode_Explicit-4.7.3rc1.dist-info/RECORD,,
```

