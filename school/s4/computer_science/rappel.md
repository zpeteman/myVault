---
aliases:
  - Chap_I
---
# Pointers and dynamic variables
- **static variables** are characterized by 4 properties :
	- name
	- address 
	- type
	- value
- **Pointer** is a special variable that can contain the address of another variable or a memory zone in general.
	- if $p$ have the address $a$ of the variable $v$ we say that **$p$ points to $v$**.
	`````C
			int *p;
			p=&v;
	`````
	- a pointer $p$ that points to the variable $v$ with address $a$ is of type $T$ 
		- the type `T*` 
	- we declare it like this : `T* p;`.
	- and initialise it : 
		``` C
		p = &v;
		p=NULL;
		```
 - **Dynamic Variables** is anonymous (address, type and value). we access to it with the help of a pointer.
	 - creation `T*p = (T*) malloc (sizeof(T) );` the function `malloc()` of the library `stdlib.h` returns `NULL` is the allocation failed.
	 - affectation of pointers, 
		```C
		p = NULL;
		p = q // earlier we have created q just like how we created p the exact same prompt. there are equivalent cuz they are in the same memory spot.
		```
	- affectation of the pointers spot. `*p = *q`
	- freeing the allocated dynamic spot. `free(p);`

# Pointers and tables
we Declare a type `T`:
- **Definition**
	a table **Tab** is a data structure which let's us stock a number of elements **Tab[i]** with index **i**. tables verify general proprieties :
	- all elements have the same type of base.
	- the number of elements is fixed.
	- the modifications of elements happens in a constant time $O(1)$, independent of the number of elements in the table.
- **Declaration**
	`T tab[TAILLE];`
- **maximum size Problem**
	if we wanna add an element to a full table will not be able to cuz of the max size of the table.
	-  Error
	- Recompilation of the table.
- **Dynamic Declaration**
	```C
	T* p;
	...
	p = (T*)malloc(n*sizeof(T));
	```
	with **n is a variable** given
	the address `P[i]` is **p+i** and its value is `*(p+i)`.

# Record
- **Declaration of the type of the structure**
	```C
	struct nom_de_struct {
	type_du_champ_1 nom_du_champ_1;
	type_du_champ_2 nom_du_champ_2;
	}
	```
- **Declaration of the record**
	`struct nom_de_struct v;`
- **access to the champs**
	`v.nom_du_champ_1;`
- **init**
	`struct Personne P1={"A12345", "Hamid", 21};`
- **Operations**
	the only operation is : 
	```C
	struct Personne P2;
	P2 = P1;
	``` 
- **Definition of the type**
	```C
	typedef struct nom_de_struct nom_type;
	nom_type v;
	```
- **Definition and declaration of the type of the structure**
	```C
	typedef struct nom_de_struct{
	type_du_champ_1 nom_du_champ_1;
	type_du_champ_2 nom_du_champ_2;
	}nom_type;
	```

# record and pointers
we consider this structure :
```C
typedef struct Personnne{
		char CIN[8];
		char nom[10];
		int age;
}Personne;
Personne *P1, P2 = {"B123", "Farid", 26};
//dynamic allocation of *P1:
P1 = (Personne*)malloc(sizeof(personne));
strcpy (P1 ->nom, "Hamid");
strcpy (P1 ->CIN, "A123");
P -> age = 21;
```

`P1 -> age ` is the same as `(*P1).age`.

# Structure of Structures
example: 
```C
typedef struct date{
		int jour, mois, annee;
}date;
typedef struct Personne {
		char CIN[8];
		char nom[10];
		int age;
		date dn;
}Personne;
Personne P1;
strcpy (P1.CIN, "B123");
strcpy (P1.nom, "Hamid");
P1.age = 21;
P1.dn.jour = 15;
P1.dn.mois = 11;
p1.dn.annee = 1998;
```

example 2 (for the case where the table is connected to the persons above it):
```C
typedef struct Personne {
		char CIN[8];
		char nom[10];
		int age;
		struct Personne *pere;
}Personne;
Personne P2, P1= {"A123", "Karim", 56, NULL};
strcpy (P2.CIN, "B123");
strcpy (P2.nom, "Hamid");
P2.age = 21;
P2.pere = &P1; // init with &P1
P1.dn.jour = 15;
P1.dn.mois = 11;
p1.dn.annee = 1998;
```

# record tables
```C
typedef struct Personne {
		char CIN[8];
		char nom[10];
		int age;
}Personne;
Personne P[TAILLE];
// the acces of the table is done is done with i.
P[i].CIN
P[i].nom
P[i].age
```