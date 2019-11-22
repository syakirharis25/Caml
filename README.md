# Categorical Abstract Machine Language (Caml) 
My works related to Categorical Abstract Machine Language (Caml) programming language.
<br /> <br />

## Table of Contents
1. [Introduction.](#introduction)
2. [Official references websites.](#references)
3. [OCaml compiler.](#compiler)
4. [GitHub notes.](#github)

<a name="introduction"></a>
## Introduction
<img src="Caml-1.gif" height="50"> 

Caml is a general-purpose programming language, designed with program safety and reliability in mind. It is very expressive, yet easy to learn and use. Caml supports functional, imperative, and object-oriented programming styles. It has been developed and distributed by INRIA, a French research institute in computer science and applied mathematics, since 1985. Caml comes from ML and CAM which is the categorical abstract machine: a virtual machine inspired by Cartesian closed categories.
<br /> <br />

<img src="OCaml-wiki.svg.png" height="50">

OCaml also known as Objective Caml is the main implementation of the Caml programming language, created in 1996 by Xavier Leroy, Jérôme Vouillon, Damien Doligez, Didier Rémy, Ascánder Suárez, and others. It extends Caml with object-oriented features, and is a member of the ML family. OCaml is a general purpose programming language with an emphasis on expressiveness and safety. Developed for more than 20 years at Inria by a group of leading researchers, it has an advanced type system that helps catch your mistakes without getting in your way. It's used in environments where a single mistake can cost millions and speed matters, is supported by an active community, and has a rich set of libraries and development tools.
<br /> <br />

<img src="inria.svg" height="100">
Institut national de recherche en informatique et en automatique (Inria), in English, The National Institute for Research in Computer Science and Automation, is a French national research institution focusing on computer science and applied mathematics. It was created under the name Institut de recherche en informatique et en automatique (IRIA) in 1967 at Rocquencourt near Paris, part of Plan Calcul,  French governmental program to promote a national or European computer industry and associated research and education activities. Its first site was the historical premises of SHAPE (central command of NATO military forces). In 1979 IRIA became INRIA. Since 2011, it has been styled Inria. Inria is a Public Scientific and Technical Research Establishment (EPST) under the double supervision of the French Ministry of National Education, Advanced Instruction and Research and the Ministry of Economy, Finance and Industry.

<a name="references"></a>
## Official references websites
Official Caml website : https://caml.inria.fr <br />
Official OCaml website : https://ocaml.org <br />
Official Inria website : https://www.inria.fr

Official OCaml download website : https://ocaml.org/docs/install.html <br />
Official OCaml download website for Microsoft Windows operating system : https://www.typerex.org/ocpwin.html

OCaml tutorials : https://ocaml.org/learn/tutorials <br />
Online OCaml playground : https://try.ocamlpro.com

Caml and OCaml was created by Xavier Leroy : https://github.com/xavierleroy, https://xavierleroy.org

<a name=compiler></compiler>
## OCaml compiler
**ocamlc** is the bytecode compiler, and **ocamlopt** is the native code compiler. If you don't know which one to use, use ocamlopt since it provides standalone executables that are normally faster than bytecode. The **-o** command specify the name of the output file produced by the linker. The default output name is **_a.out_** under Unix and **_camlprog.exe_** under Windows. **_.cmi_** files are intermediate (interface) files which are compiled forms of the **_.ml_** file. **_.cmo_** is the	object file (bytecode). **_.cmx_** is produced by ocamlopt (the native-code compiler). Main output files of ocamlopt is **_.o_** but ocamlopt also produce it.

**ocamlc** (bytecode compiler) implementation command.
```
$ ocamlc -o filename filename.ml
$ ocamlrun filename
```
**ocamlc** command will create filename.cmi and filename.cmo files.

**ocamlopt** (native code compiler) implementation command.
```
$ ocamlopt -o filename filname.ml
$ ./filename
```
In Microsoft Windows system, OCaml commands can be found inside **C:\Users\username\AppData\Roaming\OCamlPro\OCPWin\4.01.0+ocp1-full-mingw64-20160113\bin** folder.

Reference : https://caml.inria.fr/pub/docs/manual-ocaml/native.html, 

<a name="github"></a>
## GitHub notes
Clone the current GitHub remote repository contents into local machine.
```
$ git clone https://github.com/syakirharis25/Caml.git
$ git remote -v
$ git status
```

If the **_refusing to merge unrelated histories_** shown due to the changing name of the working directory on the local machine, then execute this commands.
```
$ git pull origin master --allow-unrelated-histories
```

If there is any changes in the GitHub (remote) repository, first we need to pull the changes into our local machine, before adding the new contents into GitHub.
```
$ git status
$ git remote -v
$ git pull origin master
$ git add <file>
$ git commit -m "message or remarks about the action done"
$ git push origin
$ git status
```

Adding new line, non-breaking space in GitHub README.md
```
a <br />
b <br />
c
```

Refer to https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet for GitHub markdown formatting.
