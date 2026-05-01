---
aliases:
  - Chapter 3
---
# Definition
- Stacks and queue are types of list used to stock and manipulate data in a dynamic set.
- them particular usage is in the way they operate in the insertion and the removal of the elements :
	- stacks delete the last inserted element.
	- queues delete the first inserted one.
- in both of them we can only access to one element.
- the way the stacks operate called **LIFO** (**last in, First out**).
- there's two ways to use a stack either by using a pointer or a table.
# Stacks
### operations
there's only five operations that can be done for a stack :
- test if the stack is empty.
- adding an element.
- deleting an element.
- recuperation of an element.
- empty the stack.

```C
//Declaration :
typedef int element;
struct cellulePile {
	elemnt value;
	struct celluePille * precedent;
};
typedef struct cellulePile cellulePile, * Pile;
```
### using a pointer
```C
//Creation and initialization :
//init
Pille pileVide(){
	return NULL;
}
//test 
int testerPileVide(Pile p){
	return p==NULL;
}

//Adding an element :
Pile empiler(elemnt val, Pile p){
	Pile pn;
	pn = malloc(sizeof(celluePile));
	pn -> value = val;
	if(p==NULL){
	pn -> precedent = NULL;
	return pn;
	} else {
	pn -> precedent =p;
	p =pn;
	return p
	}
}

// Deletion of an element:
Pile depiler(Pile p){
	Pile pPile;
	if(p==NULL)
		return NULL;
	else{
	pPile = p->precedent;
	free(p);
	return pPile;
	}
}

//Recuperation of an element:
Pile valeurSommet(Pile p, elemnt *vdep){
	Pile pPile;
	if(p=NULL)
		return NULL;
	else {
		*vdep = p->value;
		pPile=p -> precedent;
		free(p);
		return pPile;
	}
}
element sommetPile(Pile p){
	return p->value;
}

//empty the stack:
Pile viderPile(Pile p){
	while(p!=NULL)
		p=depiler(p);
	return p;
}
```

### using a table
```C
//creation : 
void pileVide(pileTab *p){
	p-> sommet=0;
}
//test
int testerPileVide(pileTab p){
	return p.sommet==0;
}

//adding an element:
pileTab empiler(element val, pileTab p){
	p.value[p.sommet]=val;
	(p.sommet)++;
	return p;
}

//deletion of an element:
pileTab depiler(pileTab p){
	p.sommet=p.sommet-1;
	return p;
}

//recupertaion:
int valeurSommet(pileTab *p){
	int vdep;
	vdep = p -> valeur[p-> sommet -1];
	p->sommet = p -> sommet -1;
	return vdep;
}
element sommetPile(pileTab p){
	return p.valeur[p.sommet -1];
}

//deletion: 
pileTab viderPile(pileTab p){
	while(p.sommet!=0)
		p=depiler(p);
	return p;
}
```

# Queues
- The way that queues work is call **FIFO** (**First in, First out**)
- generally we can implement it : pointers, tables and chained lists.
### operations
there's only five operations that can be done for a stack :
- test if the queue is empty.
- adding an element.
- deleting an element.
- recuperation of an element.
- empty the queue.

```C
//Declaration :
typedef int element;
struct celluleFile {
	elemnt value;
	struct cellueFille * suivant;
};
typedef struct celluleFile celluleFile, * File;
```

### Using pointers
```C
// init
File fileVide() {
    File f;
    f.tete = f.queue = NULL;
    return f;
}

// test empty
int testerFileVide(File f) {
    return f.tete == NULL;
}

// enqueue
File enfiler(element val, File f) {
    cellule* nv = malloc(sizeof(cellule));
    nv->valeur = val;
    nv->suivant = NULL;

    if (f.queue == NULL) {
        f.tete = f.queue = nv;
    } else {
        f.queue->suivant = nv;
        f.queue = nv;
    }
    return f;
}

// dequeue
File defiler(File f) {
    if (f.tete == NULL) return f;

    cellule* tmp = f.tete;
    f.tete = f.tete->suivant;

    if (f.tete == NULL) f.queue = NULL;

    free(tmp);
    return f;
}

// retrieve + delete
File valeurFile(File f, element* v) {
    if (f.tete == NULL) return f;

    *v = f.tete->valeur;
    return defiler(f);
}

// peek
element teteFile(File f) {
    return f.tete->valeur;
}

// empty queue
File viderFile(File f) {
    while (f.tete != NULL)
        f = defiler(f);
    return f;
}
```

### using circular buffer
```C
// init
FileTab fileVideTab() {
    FileTab f;
    f.debut = 0;
    f.fin = -1;
    f.taille = 0;
    return f;
}

// test empty
int testerFileVideTab(FileTab f) {
    return f.taille == 0;
}

// enqueue
FileTab enfilerTab(element val, FileTab f) {
    if (f.taille == MAX) return f; // full

    f.fin = (f.fin + 1) % MAX;
    f.tab[f.fin] = val;
    f.taille++;
    return f;
}

// dequeue
FileTab defilerTab(FileTab f) {
    if (f.taille == 0) return f;

    f.debut = (f.debut + 1) % MAX;
    f.taille--;
    return f;
}

// retrieve + delete
FileTab valeurFileTab(FileTab f, element* v) {
    if (f.taille == 0) return f;

    *v = f.tab[f.debut];
    return defilerTab(f);
}

// peek
element teteFileTab(FileTab f) {
    return f.tab[f.debut];
}

// empty queue
FileTab viderFileTab(FileTab f) {
    f.debut = 0;
    f.fin = -1;
    f.taille = 0;
    return f;
}
```

### Using chained lists
```C
// init
Queue initQueue() {
    Queue q;
    q.head = q.tail = NULL;
    return q;
}

// empty test
int isEmpty(Queue q) {
    return q.head == NULL;
}

// enqueue
Queue enqueue(element val, Queue q) {
    node* n = malloc(sizeof(node));
    n->val = val;
    n->next = NULL;

    if (q.tail == NULL) {
        q.head = q.tail = n;
    } else {
        q.tail->next = n;
        q.tail = n;
    }
    return q;
}

// dequeue
Queue dequeue(Queue q) {
    if (q.head == NULL) return q;

    node* tmp = q.head;
    q.head = q.head->next;

    if (q.head == NULL) q.tail = NULL;

    free(tmp);
    return q;
}

// retrieve + delete
Queue frontValue(Queue q, element* v) {
    if (q.head == NULL) return q;

    *v = q.head->val;
    return dequeue(q);
}

// peek
element front(Queue q) {
    return q.head->val;
}

// empty queue
Queue clearQueue(Queue q) {
    while (q.head != NULL)
        q = dequeue(q);
    return q;
}
```