
1) Imprime en consola `Hello World`.

(base) karmelealonsoaia@MacBook-Air-de-Karmele 1.1-lab_bash % echo "Hello world"
Hello world
 


2) Crea un directorio nuevo llamado `new_dir`.

(base) karmelealonsoaia@MacBook-Air-de-Karmele 1.1-lab_bash % mkdir "new_dir"
(base) karmelealonsoaia@MacBook-Air-de-Karmele 1.1-lab_bash % ls
README.md	lorem		new_dir		solutions.md


3) Elimina ese directorio.

(base) karmelealonsoaia@MacBook-Air-de-Karmele 1.1-lab_bash % rm -r "new_dir"
(base) karmelealonsoaia@MacBook-Air-de-Karmele 1.1-lab_bash % ls
README.md	lorem		solutions.md

4) Copia el archivo `sed.txt` dentro de la carpeta lorem a la carpeta lorem-copy. TIP: Puede ser necesario crear la carpeta lorem-copy primero. 

(base) karmelealonsoaia@MacBook-Air-de-Karmele 1.1-lab_bash % mkdir "lorem-copy"
(base) karmelealonsoaia@MacBook-Air-de-Karmele 1.1-lab_bash % cp lorem/sed.txt lorem-copy
(base) karmelealonsoaia@MacBook-Air-de-Karmele 1.1-lab_bash % cd lorem-copy
(base) karmelealonsoaia@MacBook-Air-de-Karmele lorem-copy % ls
sed.txt


5) Muestra el contenido del archivo `sed.txt` dentro de la carpeta lorem. 

(base) karmelealonsoaia@MacBook-Air-de-Karmele lorem-copy % cat sed.txt
Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, 
totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo. 
Nemo enim ipsam voluptatem quia voluptas sit aspernatur aut odit aut fugit, 
sed quia consequuntur magni dolores eos qui ratione voluptatem sequi nesciunt. 
Neque porro quisquam est, qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit, 
sed quia non numquam eius modi tempora incidunt ut labore et dolore magnam aliquam quaerat voluptatem. 
Ut enim ad minima veniam, quis nostrum exercitationem ullam corporis suscipit laboriosam, 
nisi ut aliquid ex ea commodi consequatur? Quis autem vel eum iure reprehenderit qui in ea voluptate velit esse quam nihil molestiae consequatur, 
vel illum qui dolorem eum fugiat quo voluptas nulla pariatur?%  

6) Muestra el contenido de los archivos `at.txt` y `lorem.txt` dentro de la carpeta lorem. 

(base) karmelealonsoaia@MacBook-Air-de-Karmele lorem-copy % cd ..
(base) karmelealonsoaia@MacBook-Air-de-Karmele 1.1-lab_bash % cd lorem
(base) karmelealonsoaia@MacBook-Air-de-Karmele lorem % ls
at.txt		lorem.txt	sed.txt
(base) karmelealonsoaia@MacBook-Air-de-Karmele lorem % cat at.txt
At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis praesentium voluptatum 
deleniti atque corrupti quos dolores et quas molestias excepturi sint occaecati cupiditate non 
provident, similique sunt in culpa qui officia deserunt mollitia animi, id est laborum et dolorum fuga. 
Et harum quidem rerum facilis est et expedita distinctio. 
Nam libero tempore, cum soluta nobis est eligendi optio cumque nihil impedit quo minus id quod 
maxime placeat facere possimus, omnis voluptas assumenda est, omnis dolor repellendus. 
Temporibus autem quibusdam et aut officiis debitis aut rerum necessitatibus saepe eveniet 
ut et voluptates repudiandae sint et molestiae non recusandae. 
Itaque earum rerum hic tenetur a sapiente delectus, ut aut reiciendis voluptatibus maiores 
alias consequatur aut perferendis doloribus asperiores repellat%                                                   (base) karmelealonsoaia@MacBook-Air-de-Karmele lorem % cat lorem.txt
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. 
Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. 
Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. 
Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.%    

7) Visualiza las primeras 3 líneas del archivo `sed.txt` dentro de la carpeta lorem-copy 

(base) karmelealonsoaia@MacBook-Air-de-Karmele lorem-copy % head -n3 sed.txt
Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, 
totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo. 


8) Añade `Homo homini lupus.` al final de archivo `sed.txt` dentro de la carpeta lorem-copy. 

(base) karmelealonsoaia@MacBook-Air-de-Karmele lorem-copy % echo "Homo homini lupus" >> sed.txt
(base) karmelealonsoaia@MacBook-Air-de-Karmele lorem-copy % tail sed.txt
Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, 
totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo. 
Nemo enim ipsam voluptatem quia voluptas sit aspernatur aut odit aut fugit, 
sed quia consequuntur magni dolores eos qui ratione voluptatem sequi nesciunt. 
Neque porro quisquam est, qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit, 
sed quia non numquam eius modi tempora incidunt ut labore et dolore magnam aliquam quaerat voluptatem. 
Ut enim ad minima veniam, quis nostrum exercitationem ullam corporis suscipit laboriosam, 
nisi ut aliquid ex ea commodi consequatur? Quis autem vel eum iure reprehenderit qui in ea voluptate velit esse quam nihil molestiae consequatur, 
vel illum qui dolorem eum fugiat quo voluptas nulla pariatur?Homo homini lupus

9) Visualiza las últimas 3 líneas del archivo `sed.txt` dentro de la carpeta lorem-copy. Deberías ver ahora `Homo homini lupus.`. 

(base) karmelealonsoaia@MacBook-Air-de-Karmele lorem-copy % tail -n3 sed.txt
Ut enim ad minima veniam, quis nostrum exercitationem ullam corporis suscipit laboriosam, 
nisi ut aliquid ex ea commodi consequatur? Quis autem vel eum iure reprehenderit qui in ea voluptate velit esse quam nihil molestiae consequatur, 
vel illum qui dolorem eum fugiat quo voluptas nulla pariatur?Homo homini lupus

10) Encuentra al usuario activo en el sistema.

(base) karmelealonsoaia@MacBook-Air-de-Karmele lorem-copy % whoami
karmelealonsoaia

11) Encuentra dónde estás en tu sistema de ficheros.

(base) karmelealonsoaia@MacBook-Air-de-Karmele lorem-copy % pwd
/Users/karmelealonsoaia/Desktop/Ironhack apuntes/1.1-lab_bash/lorem-copy


12) Lista los archivos que terminan por `.txt` en la carpeta lorem.

(base) karmelealonsoaia@MacBook-Air-de-Karmele lorem-copy % cd ..
(base) karmelealonsoaia@MacBook-Air-de-Karmele 1.1-lab_bash % cd lorem
(base) karmelealonsoaia@MacBook-Air-de-Karmele lorem % ls *.txt
at.txt		lorem.txt	sed.txt


13) Cuenta el número de líneas que tiene el archivo `sed.txt` dentro de la carpeta lorem. 

(base) karmelealonsoaia@MacBook-Air-de-Karmele lorem % wc sed.txt
       8     129     873 sed.txt

14) Cuenta el número de **archivos** que empiezan por `lorem` que están en este directorio y en directorios internos.

(base) karmelealonsoaia@MacBook-Air-de-Karmele lorem % find . -type f -name "lorem*"
./lorem.txt

15) Cuenta el número de apariciones del string `et` en `at.txt` dentro de la carpeta lorem. 


## Ficheros bash

Cualquier comando o comandos de bash se pueden almacenar en un fichero y ejecutar cuando queramos. 
Obviamente puedes utilizar tu editor preferido. Creamos el fichero: 
```
$ Ficheros bash" 
```

E incluimos el contenido que queramos. En este caso listar ficheros:
```bash
#!/bin/bash
ls
```

Ejecutamos el script:
```

```

Y veremos por consola el siguiente output. 
```console
README.md lorem solutions.ipynb
```
