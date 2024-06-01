# Outils pour ma veille techno

Dans ce document j'aimerais vous proposer les outils que je découvre en effectuant ma veille technologique qui sont pour moi un plus.

Je vous donnerai le nom de l'outil, un lien de ressource et mon avis.

## .NET

### XSD2Code

Développé par un des mes anciens chef, `Pascal Cabanel` est un developpeur .NET très performant et conscienceux.
Quand j'ai débuté dans le monde du dév pro c'était sur du .NET avec lui.
A l'époque nous avions travaillé ensemble sur un logiciel en rapport avec le Ségu de la santé pour l'entreprise CGM (Compute group medical).

Monsieur cabanel m'avait alors présenté un outil de sont cru [XSD2Code](https://www.xsd2code.com/)

Cet outil, qui se présente sous forme d'un plugin visual studio, permet de générer les classes C# avec leurs dépendences et relations entre elles en utilisant une description dans un fichier XSD (syntaxe très proche du XML)

C'est vraiment un super outil et je le recommande grandement.

## Spring (Boot)

#### Spring initializr

Il s'agit d'une très bonne pratique de commencer un projet spring (boot) avec un starter comme [Spring initializr](https://start.spring.io/)
Il permet de démmarer un projet rapidement et simplement.
Il n'y a pas grand chose à dire de plus.
Super outil

## Angular

### QucikType

L'outil que je vais vous présenter n'est passpécifique à Angular mais à typescript.
En tant que développeur full-stack ou frontend on à tous connu une personne (des fois nous-même) utiliser le type any dans les Observables ou dans des classes car la description de l'objet était trop longue.

Ce bout de code vous parle t-il ?
```typescript
public getCars(): Observable<any> {
  return this.http.get<any>(`${this.serverUrl}`/cars);
```

Alors que les bonnes pratiques typescript imposent une utilisation typée
```typescript
public getCars(): Observable<Car[]> {
  return this.http.get<Car[]>(`${this.serverUrl}`/cars);
```

C'est que que vous promet [QuickType](https://quicktype.io/). Donnez lui la réponse du backend et il vous produira vos classes typescript.

### Typescript's Getters Setters

Je sais bien qu'en typescript nous pouvons accèder aux propriété de la classe.
Mais j'avoue bien aimer le principe du Getter et Setter. Pourquoi ?
Quand je veux le nom d'une personne de la classe `Person` peut être que j'aimerai que ce nom soit en `lowercase` et éviter d'utiliser un pipe.
Quand j'utilise un setter c'est bien aussi pour appliquer une logique de tranformation et uniformisation de la donnée.
Donc voici un plugin VSCode qui vous génére des Getters et Setters basiques.
[getters-and-setters](https://marketplace.visualstudio.com/items?itemName=Wilson-Godoi.wg-getters-and-setters)
