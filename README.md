# Jeu de Tic Tac Toe et Puissance 4 en C++

Choix du jeu possible !
```cpp
while (choixIsDone == false){
    cout << "Entrez le choix de votre jeu \"TicTacToe\" ou \"Puissance_4\"" << endl;
    cin >> choixJoueur;
    if(choixJoueur == "TicTacToe" || choixJoueur == "tictactoe" || choixJoueur == "ticTacToe" || choixJoueur == "TictacToe" || choixJoueur = "TicTactoe"){
        monJeu = jeuTicTacToe;
        choixIsDone = true;
    } else if(choixJoueur == "Puissance_4" || choixJoueur == "puissance_4" || choixJoueur == "Puissance4" || choixJoueur == "puissance4"){
        monJeu = jeuPuissance_4;
        choixIsDone = true;
    } else{
        cout << "Ce choix n'existe pas, veuillez ressayer" << endl;
    }
}
```

# Stratégie affichage

[Site de ref de design patern](https://refactoring.guru/fr)

```mermaid
classDiagram


AffStrategy --* Contexte
<<interface>> AffStrategy

class AffStrategy{
    execute()
}

class AffichageA{
    execute()
}

class AffichageB{
    execute()
}

AffStrategy <-- AffichageA
AffStrategy <-- AffichageB

```
