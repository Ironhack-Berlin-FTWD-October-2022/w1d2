## Responsive Web Design

- the site or application that you are building should look good on every device

- actually the device isn't the important factor, what matters is the size of the 
screen - the viewport size

## Mobile First Approach 

- instead of designing the app for a large screen first and then adapting it to a smaller
screen it is a better strategy to implement the small screen version first and then expand 
it to the larger screen
- you concentrate on the essential functionality first, exactly as in the MVP (Minimum viable product) principle 
- we achieve responsiveness via media queries that set break points where according to the screen size the css styling changes

## Nice list for screen sizes and media queries can be found here: 
https://gist.github.com/gokulkrishh/242e68d1ee94ad05f488

## Advice for font size : set a font size in the html of 16px (font size that has best UX)

```
    html {
        font-size: 16px;
    }
```

- and from that point on rem (relative to the html font size) e.g. 2rem = 32px
- or if the same result but easier to calculate html : 10px - 1.6rem -> 16px  
- if for some reason you want relative to the parent use em instead of rem
#### Responsiveness is achieved via media queries
```
// style.css - this styling is applied for any screen width up to 480px 
@media (max-width: 480px) {
	.container {
		flex-direction: column;
	}
	.box {
		width: 80vw;
	}
}
```