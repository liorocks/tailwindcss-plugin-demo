# tailwindcss-plugin-demo

> Demo plugin created with create-tailwind-plugin

Install the plugin from npm:

```
$ npm install tailwindcss-plugin-demo
```

Then add the plugin to your `tailwind.config.js` file:

```js
// tailwind.config.js
module.exports = {
  theme: {
    // ...
    // Optional. Your plugin might not have any options at all.
    demo: {
      // ...
      YOUR_PLUGIN_CUSTOM_OPTION: true,
      // ...
    },
  },
  variants: {
    // ...
    // Optional. Your plugin might not have any variants at all.
    demo: ['responsive'],
    // ...
  },
  plugins: [
    // ...
    require('tailwindcss-plugin-demo'),
    // ...
  ],
};
```

This plugin will generate following CSS:

```css
/* ... */
.example-utility-class {
  display: block;
}

.custom-utility-class {
  background-color: red;
}
/* ... */
```

## License

tailwindcss-plugin-demo is licensed under the MIT License.

## Credits

Created with [create-tailwind-plugin](https://github.com/Landish/create-tailwind-plugin).
