---
aliases:
  - Chapter II
---
### Operational specification 
- **table implementation**
	this implementation is not practical because the insert and the remove of elements in the list. because we'll always need to declare the total amount of elements of the table.
- **chained list implementation**
	- **simple list chained**
		- **Def**
			- Maillon notion : each element have a data zone and a pointer to the next cell.
			- the next maillon : if there's no next cell the pointer is NULL.
			- list notion : the list is made using a sequence of those cells.
		- **implementation**
			we suppose that we had already declared the type `Telement`.
			```C
			typedef int Telement;
			struct cells {
					Telemnt info;
					struct cells *suiv;
			};
			typedef struct cells liste;
			// init
			liste * listeVide(){
				return NULL;
			} // there's more stuffs to do in here but ive got lazy to write them down sorry. 
			```
	- **double list chained**
		it have a pointer to the next element and the previous one.
	- **Circulated list**
		the last element have a pointer to the very first one 







