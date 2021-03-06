# react-simple-minimal-carousel.

A lightweight and fully customizable carousel component for React

### DEMO

<https://neon010.github.io/react-simple-minimal-carousel-demo/>

### Installing as a package

```
npm install react-simple-minimal-carousel
```

```
yarn add react-simple-minimal-carousel
```

### Usage

```jsx
import {Carousel} from "react-simple-minimal-carousel"

function App() {
  return (
    <div className="App">
      <Carousel 
      images={
        [
          'https://images.unsplash.com/photo-1544005313-94ddf0286df2?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxzZWFyY2h8Mnx8cG9ydHJhaXR8ZW58MHx8MHx8&auto=format&fit=crop&w=500&q=60', 
          'https://images.unsplash.com/photo-1616776005756-4dca36124bf9?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxzZWFyY2h8MTN8fHBvcnRhaXR8ZW58MHx8MHx8&auto=format&fit=crop&w=500&q=60',
          'https://images.unsplash.com/photo-1611451444023-7fe9d86fe1d0?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxzZWFyY2h8MXx8cG9ydHJhaXQlMjB3b21hbnxlbnwwfHwwfHw%3D&auto=format&fit=crop&w=500&q=60',
          'https://images.unsplash.com/photo-1494790108377-be9c29b29330?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxzZWFyY2h8NHx8Z2lybHxlbnwwfHwwfHw%3D&auto=format&fit=crop&w=500&q=60'
        ]}
      width={650}
      height={500}
      showDots={true}
      leftArrowLabel={"left"}
      rightArrowLabel={"right"}
      arrowStyle={{padding:"5px", background:"black", color:"#fff", border:'none'}}
      />
    </div>
  );
}

export default App;
```

### Props

| Name                                     | Value                        | Description                                                                                                                                                                                                           |
| ---------------------------------------- | ---------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| width                                | `number`                         | Set the width of image.                   |
| height                               | `number`                         | Set the height of image                   |
| images                               | `array`                          | Set the image                             |                  
| showDots                             | `boolean` default `true`         | enable dots at the bottom of slide        |
| currentImageDotsColor                | `string` default `#1e293b`       | color of current image dots               |
| otherDotColor                        | `string` defaults `#e5e7eb`      | color of of other dots                    |
| leftArrowLabel                       | `string` or `JSX`                | Set the label for left button             |
| rightArrowLabel                      | `string` or `JSX`                | Set the label for right button            |
| arrowStyle                           | `object`                         | Style object for left and right button    |
| showCurrentSlideNumber               | `boolean` default `true`         | current slide number at the left top      |