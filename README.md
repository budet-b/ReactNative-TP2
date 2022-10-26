# TP2 - Myflix

## Présentation

Le but de ce TP est de manipuler des queries et mutations en GraphQL. Vous avez une partie `server` pour le lancer:
```
cd server
yarn
node index.js
```

Si tout se passe bien vous devriez voir:
```
Server running
```
<img src="./assets/myflix.gif" width="400" height="790">

C'est un exemple de rendu, le design n'est pas la partie la plus importante dans le TP.

### Step by step

1. Créer une `MovieCard` prenant en props: `picture, title, category, year`. Il sera utile d'avoir un `TouchableOpacity` autour de cette carte pour la suite.
2. Créer la query `getAllMovies` avec `@apollo/client` https://www.apollographql.com/docs/react/integrations/react-native/
3. Créer le hooks `useGetAllMovies`
4. Gérer la navigation, créer un router avec `react-navigation` et utiliser `NavigationContainer, Stack.Navigator, Stack.Screen`
5. Récupérer les `movies` via le hooks `useGetAllMovies` et afficher une liste horizontal 
6. Ajouter un bouton `Add` qui navigue vers une nouvelle page
7. Créer un formulaire avec les champs suivants: category, title, year. Vous avez le choix entre essayer une lib de formulaire ou bien de faire des `state`
8. Créer la mutation `createMovie` et en faire un hooks `useCreateMovie`
9. Lier le formulaire avec la nouvelle mutation
10. Afficher le dernier `movie` créée via le formulaire

### Bonus
- Créer la page de Détail qui récupère les informations d'un `movie` au `onPress` sur un item de la liste
- Afficher plusieurs catégories/listes sans passer les movies en props et en ayant uniquement un seul appel graphql
- Créer un storybook 
