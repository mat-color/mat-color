# @mat-color/sass

Wherewith are you creating a material palette for an Angular Material project? Usual it doing with online tools or apps. 

A custom material palette is a big sass map, and makes it manually is a tricky thing. It looks like this:
```sass
$primary: mat-palette(
    (
      50: #fffee6,
      100: #fefbbf,
      200: #fcf893,
      300: #faf464,
      400: #f6ef39,
      500: #fff500,
      600: #ffe100,
      700: #ffc800,
      800: #ffae00,
      900: #ff8100,
      contrast: (
        50: rgba(0, 0, 0, 0.87),
        100: rgba(0, 0, 0, 0.87),
        200: rgba(0, 0, 0, 0.87),
        300: rgba(0, 0, 0, 0.87),
        400: rgba(0, 0, 0, 0.87),
        500: rgba(0, 0, 0, 0.87),
        600: rgba(0, 0, 0, 0.87),
        700: rgba(0, 0, 0, 0.87),
        800: rgba(0, 0, 0, 0.87),
        900: rgba(0, 0, 0, 0.87)
      )
    )
);
```

But what if we could make a palette using one color in our code? It is possible because SASS can do the math!

This sass library helps you generate a material palette for use in [@angular/material](https://material.angular.io/) with one base color!

## How it use
1. Install package `npm i @mat-color/sass`
2. Import `@mat-color/sass/mat-color` in your sass-file.
3. Use the 'generate-mat-color' function.
4. Call the 'mat-palette' function with the returned result.
5. Enjoy!
```sass
@import "~@mat-color/sass/mat-color";

$primary: mat-palette(generate-mat-color(#b9ffaf));
```
### Say thanks
<a href="https://www.buymeacoffee.com/katsuba" target="_blank">
  <img src="https://cdn.buymeacoffee.com/buttons/v2/default-blue.png" alt="Buy Me A Coffee" height="41" width="174" style="box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;-webkit-box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;" >
</a>
