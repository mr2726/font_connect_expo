<h1 align="center">Font connect expo</h1>

### Exemple
```js
import { Text, View } from 'react-native';
import { useFonts } from 'expo-font';

export default function App() {
  const [fontLoaded] = useFonts({
    'font_name' : require('./assets/fonts/JosefinSans-Regular.ttf')
  });
  if(!fontLoaded){
    return (
      <View style={{flex: 1, justifyContent: 'center', alignItems: 'center'}}>
        <Text>Fonts is not loaded!</Text>
      </View>
    );
  }
  return (
    <View style={{flex: 1, justifyContent: 'center', alignItems: 'center'}}>
      <Text style={{fontFamily: 'font_name'}}>Open up App.js to start working on your app!</Text>
    </View>
  );
}
```
