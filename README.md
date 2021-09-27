# tp3-LoicAstruc38
tp3-LoicAstruc38 created by GitHub Classroom


#include <stdio.h>

int exercice_1 (){
    int a = 0, b = 0;
    printf("Saisissez un entier :\n");
    scanf("%d", &a);
    printf("Saisissez un entier :\n");
    scanf("%d", &b);
    if (a>=b) {
        printf("%d est le plus grand des deux nombres \n", a);}
    else {
        printf("%d est le plus grand des deux nombres \n", b);}
}

int exercice_2 (){
    int longueur = 0, largeur = 0;
    printf("Saisissez deux entiers :\n");
    scanf("%d", &longueur);
    scanf("%d", &largeur);
    printf("Le perimetre du rectangle est %d \n\n", (largeur + longueur) * 2);
    printf("L'aire du rectangle est %d \n\n", largeur * longueur);
}

int exercice_3 (){
    int a = 0;
    printf("Saisissez un entier : \n");
    scanf("%d", &a);
    if (a%3 == 0){
        printf("Cet entier est un multiple de 3 \n");}
    if (a >= 10)
        printf("Cet entier est superieur ou egal a 10 \n");
}

int exercice_4 (){
    int age = 0;
    printf("Saisissez votre age : \n");
    scanf("%d", &age);
    if (age < 12){
        printf("Le billet coute 4 euros \n\n");}
    else if (12 <= age && age < 17){
        printf("Le billet coute 6 euros \n\n");}
    else if (age >= 65){
        printf("Le billet coute 6 euros \n\n");}
    else if (age < 27 && 17 <= age) {
        int a = 0;
        etudiant:
        printf("Si vous etes etudiant saisissez 1, sinon saisissez 0: \n");
        scanf("%d", &a);
        if (a = 1) {
            printf("Le billet coute 6 euros \n\n");}
        else if (a = 0) {
            printf("Le billet coute 9 euros \n\n");}
        else {
            printf("Saisie incorrecte");
            goto etudiant;}}
    else {
        printf("Le billet coute 9 euros \n\n");}
}

int exercice_5 (){
    int i = 0;
    printf("Saisissez le numero de la boisson choisie :\n");
    scanf("%d", &i);
    if (i == 1){
        printf("Boisson_Froide_1\n\n");}
    else if (i == 2){
        printf("Boisson_Froide_2\n\n");}
    else if (i == 3){
        printf("Boisson_Froide_3\n\n");}
    else if (i == 10){
        printf("Boisson_Chaude_1\n\n");}
    else if (i == 11){
        printf("Boisson_Chaude_2\n\n");}
    else {
        printf("Erreur de numero");}
}

int exercice_6 (){
    float note1 = 21, note2 = 21, note3 = 21;
    while(note1 < 0 || note1 > 20){
        printf("Saisisissez la premiere note sur 20 :\n");
        scanf("%f", &note1);}
    while(note2 < 0 || note2 > 20){
        printf("Saisisissez la deuxieme note sur 20 :\n");
        scanf("%f", &note2);}
    while(note3 < 0 || note3 > 20){
        printf("Saisisissez la troisieme note sur 20 :\n");
        scanf("%f", &note3);}
    printf("La moyenne de vos notes est %f \n\n", (note1 + note2 + note3) / 3);
}

int exercice_7 (){
    int nbrClasses = 0, nbrEleves = 0, nbrElevesClasse = 0;
    printf("Saisissez le nombre de classe :\n");
    scanf("%d", &nbrClasses);
    for (int i = 1; i <= nbrClasses; i++){
        printf("Saisissez le nombre d'eleves dans la classe %d : \n", i);
        scanf("%d", &nbrElevesClasse);
        nbrEleves = nbrEleves + nbrElevesClasse;}
    printf("Il y a %d eleves dans l'ecole \n\n", nbrEleves);
}

int exercice_8 (){
    int a = 0;
    etape1:
    printf("Saisissez un nombre entier :\n");
    scanf("%d", &a);
    while (!(a % 2 == 0 && a % 7 == 0)){
        goto etape1;}
}

int exercice_9 () {
    int nbrDePierres = 0, nbrEtages = 0, somme = 0;
    printf("Entrez le nombre de pierres disponibles :\n");
    scanf("%d", &nbrDePierres);
    for (int i  = 0; i<= nbrDePierres; i++){
        if (somme <= nbrDePierres){
            nbrEtages += 1;
            somme += nbrEtages * nbrEtages;}}
    printf("Il pourra y avoir %d etages dans la pyramide \n\n", nbrEtages - 1);
}

int exercice_10 (){

}


int main() {
    //exercice_1();     /* fonctionnel */
    //exercice_2();     /* fonctionnel */
    //exercice_3();     /* fonctionnel */
    //exercice_4();     /* bug etudiants */
    //exercice_5();     /* fonctionnel */
    //exercice_6();     /* fonctionnel */
    //exercice_7();     /* fonctionnel */
    //exercice_8();     /* fonctionnel */
    //exercice_9();     /* fonctionnel */
    //exercice_10();

    return 0;
}
