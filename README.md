# Caml
My works related to Categorical Abstract Machine Language (Caml) programming language.

<img src="Caml-1.gif" height="50">

Caml is a general-purpose programming language, designed with program safety and reliability in mind. It is very expressive, yet easy to learn and use. Caml supports functional, imperative, and object-oriented programming styles. It has been developed and distributed by INRIA, a French research institute in computer science and applied mathematics, since 1985.

<img src="OCaml-wiki.svg.png" height="50">

OCaml also known as Objective Caml is the main implementation of the Caml programming language, created in 1996 by Xavier Leroy, Jérôme Vouillon, Damien Doligez, Didier Rémy, Ascánder Suárez, and others. It extends Caml with object-oriented features, and is a member of the ML family. OCaml is a general purpose programming language with an emphasis on expressiveness and safety. Developed for more than 20 years at Inria by a group of leading researchers, it has an advanced type system that helps catch your mistakes without getting in your way. It's used in environments where a single mistake can cost millions and speed matters, is supported by an active community, and has a rich set of libraries and development tools.

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

Refer to https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet for GitHub markdown formatting.
