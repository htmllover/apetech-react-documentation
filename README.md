## How to configure

Stack We Used
1. React Js and React Router Dom 
2. HTML5

Folder Structure
1) Components
2) themes
3) routers

## components

If you are familiar with react or create react app architecture, then we are familiar with components.
Components are reusable codes that you will use throughout your project.Here in components folder,
Under components folder we wrote all of our components individually.We have written these components 
to make the developer’s life easy.By using these basic components, For example in our components dir 
there is HeroSection folder whrere we wrote our different styled heroSection.
For example

```text
.
└── Src
    ├── components
        ├── Header
          └── header.js (here we wrote all the code for header)
          (we have six different style for hero section and we maid component for every single style)
    └── HeroSection
        ├── heroOne.js (code for hero one style)
        └── heroTwo.js
        └── .....
        └── heroSix.js (code for her six style)
        you can write custom components according to your need.
```

## themes
Under themes dir we wrote all of our root theme like themeOne, themeTwo where we combined all of our components as per our theme design.
For example -- here is the combination to build themeOne
```text
└── themes
    ├── theme-one.js
```
```js
<div className="">
    <Header />
    <HeroSection />
    .....
    <Footer />
</div>
```
Now if you want's to make a theme as your default theme as per your requirements.Just import the theme on `app.js` and render it.
like
```js
import ThemeOne from "./themes/theme-one";

function App() {
  return (
    <div>
      <ThemeOne />
    </div>
  );
}
```

## routers
In router section we used route js. where we linked all the route for our all theme.
For routing we used react-router-dom.To view theme-two use with your root url
```text
/theme-two 
```

## theme installtion
To install the theme you have to install [react](https://create-react-app.dev/) than go to the theme root dir where `package.json` located and use
```bash
npm install
```
it will install the packeges.

After install process now you can run local server- local server port is 'http://localhost:3000'
For developement start use
```bash
npm start
```
## Build your theme
```bash
npm run build
```

## For deployment -- static server
First install
```bash
npm install -g serve
serve -s build
```
If you want know more about static deployment please visit [Create react app deployment](https://create-react-app.dev/docs/deployment)

Enjoy your theme :) 
