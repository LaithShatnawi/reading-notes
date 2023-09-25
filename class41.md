# React Native

## getting started with react native

### 1.Name three Core Components of React Native and describe what they do.

1. < View > A container that supports layout with flexbox, style, some touch handling, and accessibility controls

2. < Text > Displays, styles, and nests strings of text and even handles touch events

3. < ScrollView > 	A generic scrolling container that can contain multiple components and views

### 2.What problem does React Native solve (why call it native)?

The advantage of React Native is that a single code allows you to create an application at once for two systems, iOS and Android. This is suitable for small applications or MVPs. React Native is a JavaScript platform that allows developers to write real-time, native-looking Android mobile app development.

“React Native brings React’s declarative UI framework to iOS and Android. With React Native, you use native UI controls and have full access to the native platform.”

So basically, React Native is a JavaScript library that allows you to use native UI controls and everything in the native platform.

### 3.What are the building blocks of a React Native app? How does that compare to a React app?

React Native utilizes APIs and native UI components to build mobile applications.

Using React, you can write code in JavaScript. Thereafter, React.Js renders Html-like components with < p >, < div >, < h1 >, etc. tags. You may use JSX - a special syntax extension for JavaScript.

If you wish to use React Native, you have to be aware of its specific syntax. Here, React Native renders native components with < view >, < text >, < images >, etc. instead of rendering HTML-like components.

## expo

### 1.What solution does expo provide?

Expo is an open-source framework for apps that run natively on Android, iOS, and the web. Expo brings together the best of mobile and the web and enables many important features for building and scaling an app such as live updates, instantly sharing your app, and web support.


### 2.Expo tries to manage as much of the complexity of building apps as possible, which is why we call it the ____ workflow.

Managed

### 3.What is the difference between React Native and Expo?

The expo package provides a suite of features that make it easier to develop, and scale complex React Native applications. You can install expo in nearly any React Native app.

## expo snack

### 1.Checkout this tool. What does snack allow you to do?

Expo Snack is a web-based code editor for building shareable, runnable React Native code examples. One of the key benefits of Expo Snack is that it allows developers to collaborate with others in real-time. This is beneficial when working on a team or when seeking advice from others.

## ejecting

### 1.What does “eject” mean within the context of Expo?

The term "eject" was popularized by create-react-app, and it is used in Expo to describe leaving the cozy comfort of the standard Expo development environment, where you do not have to deal with build configuration or native code. When you "eject" from Expo, you have two choices:

Eject to bare workflow, where you jump between workflows and move into the bare workflow, where you can continue to use Expo APIs but have access and full control over your native Android and iOS projects.

Eject to ExpoKit, where you get the native projects along with ExpoKit. This option is deprecated and support for ExpoKit was removed after SDK 38.

### 2.When should you not eject?

Expo eject is a deprecated term and is no longer necessary. It was replaced by the npx expo prebuild command which continuously generates native projects for you based on the libraries in your project and the app config (app.json). Learn more in the Expo Prebuild documentation.

Unlike the expo eject library, authors can configure their libraries to work with Expo Prebuild by creating a config plugin. This means you can use any library with Expo Prebuild. You can also use any custom native code with Expo Prebuild by creating a development build.

Limitations

Previously, Expo had large native binary sizes and didn't support custom native code without "ejecting". These issues went away in December 2020 when we released EAS Build which supports any React Native app. The concept of "ejecting" was replaced by the popular Expo Prebuild feature which has been around since SDK 41 (April 2021). The expo eject command was fully deprecated in Expo SDK 46 (August 2022).

We believe Expo tools are a great option for anyone looking to create amazing cross-platform apps quickly. Nonetheless, everyone's project is unique, and there may be reasons Expo is not the right choice for what you're building. Reasons, why you may not want to use certain Expo tools with your project, are listed below:

### 3.Why might you choose to eject?

    1- You want to add an “NPM” package to your project which requires a react–native link. And as a rule of thumb, if the documentation for a third-party package states that you need to run the command react-native link as part of the setup process, then this package can’t be used with expo.


    2- You are more of a native (Java/Kotlin/Swift/Objective C) person, and want to integrate native module into your React–native app but couldn’t find a way to do it in the expo, so want to get rid of it?


    3- You want to add an awesome push notification library like OneSignal in your app which expo doesn’t support.