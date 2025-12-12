React native

How its works

## Components
View - as container or wrapper like div
Text - like text on the screen
TextInput - input in html
ScrollView - 

## Create
npx create-expo-app@latest .
npm run reset-project the 'no' to remove boilerplate code

## styles
import stlesheet from react-native

## Expo Router
### Expo router is a file based routing system.
must inside app folder
any file has default export is a route
index file represent the root

### navigation Link (stack navigation)
import { Link } from 'expo-router';
<Link href="/about/>About<Link>

### dynamic routing
[id].tsx
import {useLocalSearchParams} from 'expo-router'
const {id} = useLocalSearchParams()

### catch all segment
[...params].tsx

### not found
+not-found.tsx

### layout
_layout.tsx

### Route groups
Logically organize groups without impacting the URL structure
wrap folder in () example (auth)

### navigation
'onChild' and 'pressable' to use pressable text
check 'relativetodirectory'
<Button title="Login" onPress={() => router.push("/profile")} />
<Button title="Login" onPress={() => router.replace("/profile")} />
<Button title="Login" onPress={() => router.back("/profile")} />

const is Logged In = false;
if (!isLoggedIn) {
return <Redirect href="/login" />;
}

### stack navigation
-<Stack. Screen name="about" options={{ title: "About" }} />
-<Stack. Screen
name="about"
options={{
title: "About",
headerRight: () => (
<Pressable onPress={() => alert("Menu button pressed!")}>
<Text style={{ color: "#fff", fontSize: 16 }}>Menu</Text>
</Pressable>
}}
/>
</Stack>

### tab navigation
swich between different tabs
wrap the folder like (tabs)

### Drawer navigation
npx expo install @react-navigation/drawer react-native-gesture-handler react-native-reanimated

### modals

### plateform specific code
about.ios.tsx
about.tsx
about.web.tsx
import { Platform } from "react-native";
if (Platform.OS === "web") {}

### api route

## env
every enivronment variable has to start with EXPO_PUBLIC_NAME
44