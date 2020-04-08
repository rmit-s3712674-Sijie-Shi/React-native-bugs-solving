# React-native-bugs-solving

1. Add react-native-router-flux to APP

When moving the APP from React-native-cli to Expo-cli, some bugs occurred indicated that the react-native-router-flux did not work well.

I tried to rebuild react native in the project but it did not work

Then I figure out that before setting up react-native-router-flux, react-navigation need to be installed.
https://github.com/aksonov/react-native-router-flux

So, the solution is:
  
  1. install react-navigation first:

  npm install @react-navigation/native
  
  expo install react-native-gesture-handler react-native-reanimated react-native-screens react-native-safe-area-context @react-native-community/masked-view
  
  2. intall react-native-router-flux
  yarn add react-native-router-flux
  
  If still doesn't work, try to go through the tutorial: https://reactnavigation.org/docs/getting-started/
  


2. sha-1 for file is not computed

When moving files from old project to the new one, I forgot to copy image files, so firstly it showed the error with cannot find image files.
After I copy the image files to the project, it showed this bug.

Solution: Restart the CMD or other console and restart the APP project

