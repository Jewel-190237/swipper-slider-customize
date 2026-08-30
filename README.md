# Swiper Slider Customize - Customized Swiper Slider Component

A customized Swiper slider component built with React and CSS. Features advanced customization, responsive design, and interactive controls.

## Features

- Advanced slider customization
- Responsive design
- Interactive controls
- Touch support
- Keyboard navigation
- Custom animations
- Multiple slide layouts
- Autoplay functionality

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/Jewel-190237/swipper-slider-customize.git
   ```

2. Install required dependencies:
   ```bash
   npm install swiper
   ```

3. Copy `swipper.tsx` and `global.css` into your project

4. Import and use the component:
   ```tsx
   import SwiperSlider from './swipper';

   function App() {
     return (
       <SwiperSlider
         slides={[
           { id: 1, image: '/slide1.jpg', title: 'Slide 1' },
           { id: 2, image: '/slide2.jpg', title: 'Slide 2' },
           { id: 3, image: '/slide3.jpg', title: 'Slide 3' },
         ]}
       />
     );
   }
   ```

## Usage

### Basic Usage
```tsx
import SwiperSlider from './swipper';

function App() {
  const slides = [
    { id: 1, image: '/slide1.jpg', title: 'Slide 1' },
    { id: 2, image: '/slide2.jpg', title: 'Slide 2' },
    { id: 3, image: '/slide3.jpg', title: 'Slide 3' },
  ];

  return <SwiperSlider slides={slides} />;
}
```

### Custom Layout
```tsx
<SwiperSlider
  slides={slides}
  layout="featured"
  showThumbnails
  showNavigation
  showPagination
/>
```

### With Autoplay
```tsx
<SwiperSlider
  slides={slides}
  autoplay
  autoplayDelay={3000}
  pauseOnHover
/>
```

### Custom Styling
```css
/* Override default styles */
.swiper-slide {
  transition: transform 0.3s ease;
}

.swiper-slide-active {
  transform: scale(1.05);
}

.swiper-pagination-bullet-active {
  background: #007bff;
  transform: scale(1.2);
}
```

### Different Slide Types
```tsx
<SwiperSlider
  slides={slides}
  slideType="image" // or "video", "text", "custom"
/>
```

## Props

| Prop | Type | Default | Description |
|------|------|---------|-------------|
| slides | array | [] | Array of slide objects |
| layout | string | 'default' | Layout type |
| showNavigation | boolean | true | Show navigation arrows |
| showPagination | boolean | true | Show pagination dots |
| autoplay | boolean | false | Enable autoplay |
| autoplayDelay | number | 3000 | Autoplay delay in ms |
| pauseOnHover | boolean | false | Pause on hover |
| showThumbnails | boolean | false | Show thumbnail navigation |
| slideType | string | 'image' | Type of slides |

## Features in Detail

### Advanced Customization
- Multiple layout options
- Custom slide transitions
- Interactive hover effects
- Custom navigation styles

### Responsive Design
- Mobile-first approach
- Breakpoint-based layouts
- Touch-friendly controls

### Interactive Controls
- Click-to-navigate
- Drag to slide
- Keyboard navigation
- Thumbnail navigation

## Author

**Jewel-190237**
- GitHub: [Jewel-190237](https://github.com/Jewel-190237)
- Email: jewel190237@gmail.com

## Contributing

Feel free to fork this project and create pull requests for any improvements.

## License

This project is open source and available under the [MIT License](LICENSE).
