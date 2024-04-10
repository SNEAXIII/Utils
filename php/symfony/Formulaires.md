# Les formulaires en Symfony
Dans symfony, les formulaires sont des classes qui contiennent les valeurs saisies dans le formulaire
## Exemple:
### Contexte
Si on a un formulaire pour créer une personne, on a:

`Prénom = ???`

`Nom = ???`
### Ce qu'il y a faire
On crée une classe sous la forme `{NomClasseVisée}Type` associée à une classe existante
### Représentation visuelle de la classe `PersonneType`
```php
class PersonneType(){
    private string $prenom;
    private string $nom;
}
```
### Utilisation
Symfony va lui même convertir les données de la classe `PersonneType` en un objet de l'entité `Personne`