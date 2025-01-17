# Backgrounds

## Background Attachment

Utilities for controlling how a background image behaves when scrolling.

<PlaygroundWithVariants
  variant='fixed'
  :variants="['fixed', 'local', 'scroll']"
  prefix='bg'
  fixed='p-2 dark:text-white opacity-85 overflow-hidden'
  nested=true
  appended='w-full h-48 overflow-y-scroll h-screen bg-center bg-no-repeat'
  html='&lt;div class="{class} w-full h-screen overflow-y-scroll bg-no-repeat bg-center" style="background-image:url(&#39;/assets/bg-blue.svg&#39;);"
&gt;&lt;p&gt;The quick brown fox jumps over the lazy dog&lt;/p&gt;&lt;/div&gt;'
/>

## Background Clip

Utilities for controlling the bounding box of an element's background.

<PlaygroundWithVariants
  variant='border'
  :variants="['border', 'padding', 'content']"
  prefix='bg-clip'
  fixed='p-2 dark:text-white opacity-85 overflow-hidden'
  nested=true
  appended='p-6 rounded-md bg-blue-300 border-4 border-blue-400 border-dashed font-extrabold text-white flex justify-center items-center py-2'
  html="&lt;div class=&quot;{class} p-6 rounded-md bg-blue-300 border-4 border-blue-400 border-dashed font-extrabold text-white flex justify-center items-center&quot;&gt;
      &lt;span class=&quot;py-2&quot;&gt;Hello World&lt;/span&gt;
    &lt;/div&gt;"
/>

<PlaygroundWithVariants
  variant='text'
  :variants="[]"
  prefix='bg-clip'
  fixed='p-2 dark:text-white opacity-85 overflow-hidden'
  nested=true
  appended='text-5xl font-extrabold bg-clip-text text-transparent bg-gradient-to-r from-green-400 to-blue-500'
  html="&lt;div class=&quot;text-5xl font-extrabold&quot;&gt;
  &lt;span class=&quot;bg-clip-text text-transparent bg-gradient-to-r from-green-400 to-blue-500&quot;&gt;
    Hello world
  &lt;/span&gt;
&lt;/div&gt;"
/>

## Background Color

Utilities for controlling an element's background color.

<PlaygroundWithVariants
  variant='gray-500'
  type='color'
  prefix='bg'
  fixed='p-2 dark:text-white opacity-85 overflow-hidden'
  nested=true
  appended='p-2 rounded-md'
  html="&lt;div class='{class} p-2 rounded-md'&gt;&lt;p&gt;The quick brown fox jumps over the lazy dog&lt;/p&gt;&lt;/div&gt;"
/>

<Customizing>

```js
// windi.config.js
export default {
  theme: {
    backgroundColor: theme => ({
      ...theme('colors'),
      primary: '#3490dc',
      secondary: '#ffed4a',
      danger: '#e3342f',
    }),
  },
}
```

</Customizing>

## Background Opacity

Utilities for controlling the opacity of an element's background color.

<PlaygroundWithVariants
  variant='50'
  type='opacity'
  prefix='bg-opacity'
  fixed='p-2 dark:text-white opacity-85 overflow-hidden'
  nested=true
  appended='p-2 rounded-md bg-blue-500'
  html="&lt;div class='bg-blue-500 {class} p-2 rounded-md'&gt;&lt;p&gt;The quick brown fox jumps over the lazy dog&lt;/p&gt;&lt;/div&gt;"
/>

<Customizing>

```js
// windi.config.js
export default {
  theme: {
    extend: {
      opacity: {
        light: '0.15',
      },
    },
  },
}
```

</Customizing>

## Background Position

Utilities for controlling the position of an element's background image.

<PlaygroundWithVariants
  variant='bottom'
  :variants="['bottom', 'center', 'left', 'left-bottom', 'left-top', 'right', 'right-bottom', 'right-top', 'top']"
  prefix='bg'
  fixed='h-screen dark:text-white opacity-85 flex flex-col justify-center pb-4'
  nested=true
  appended='mx-auto bg-blue-300 rounded-md w-36 h-36 bg-no-repeat'
  html='&lt;div class=&quot;mx-auto {class} bg-blue-300 rounded-md w-36 h-36 bg-no-repeat&quot; style=&quot;background-image:url(&#39;/assets/bg-square.svg&#39;);&quot;&gt;&lt;/div&gt;'
/>

<Customizing>

```js
// windi.config.js
export default {
  theme: {
    backgroundPosition: {
      'bottom': 'bottom',
      'bottom-4': 'center bottom 1rem',
      'center': 'center',
      'left': 'left',
      'left-bottom': 'left bottom',
      'left-top': 'left top',
      'right': 'right',
      'right-bottom': 'right bottom',
      'right-top': 'right top',
      'top': 'top',
      'top-4': 'center top 1rem',
    },
  },
}
```

</Customizing>

## Background Repeat

Utilities for controlling the repetition of an element's background image.

<PlaygroundWithVariants
  variant='repeat'
  :variants="['repeat', 'no-repeat', 'repeat-x', 'repeat-y', 'repeat-round', 'repeat-space']"
  prefix='bg'
  fixed='h-screen dark:text-white opacity-85 flex flex-col justify-center pb-4'
  nested=true
  appended='mx-auto w-full h-36 bg-blue-300 rounded-md'
  html='&lt;div class=&quot;mx-auto w-full h-36 bg-blue-300 rounded-md {class}&quot; style=&quot;background-image:url(&#39;/assets/bg-square.svg&#39;);&quot;&gt;
  &lt;/div&gt;'
/>

## Background Size

Utilities for controlling the background size of an element's background image.

<PlaygroundWithVariants
  variant='auto'
  :variants="['auto', 'cover', 'contain']"
  prefix='bg'
  fixed='p-2 dark:text-white opacity-85 overflow-hidden'
  nested=true
  appended='w-full h-36 bg-no-repeat bg-center'
  html="&lt;div class=&quot;w-full h-36 {class} bg-no-repeat bg-center&quot; style=&quot;background-image:url(&#39;/assets/bg-blue.svg&#39;);&quot;&gt;
  &lt;/div&gt;"
/>

<Customizing>

```js
export default {
  theme: {
    backgroundSize: {
      'auto': 'auto',
      'cover': 'cover',
      'contain': 'contain',
      '50%': '50%',
      '16': '4rem',
    },
  },
}
```

</Customizing>

## Background Image

Utilities for controlling an element's background image.

<PlaygroundWithVariants
  variant='gradient-to-r'
  :variants="['none', 'gradient-to-t', 'gradient-to-tr', 'gradient-to-r', 'gradient-to-br', 'gradient-to-b', 'gradient-to-bl', 'gradient-to-l', 'gradient-to-tl']"
  prefix='bg'
  fixed='p-2 dark:text-white opacity-85 overflow-hidden'
  nested=true
  appended='h-36 w-36 rounded-md from-green-400 to-blue-500'
  html="&lt;div class=&quot;h-36 w-36 rounded-md {class} from-green-400 to-blue-500&quot;&gt;&lt;/div&gt;"
/>

<Customizing>

```js
// windi.config.js
export default {
  theme: {
    extend: {
      backgroundImage: theme => ({
        'hero-pattern': 'url(\'/img/hero-pattern.svg\')',
        'footer-texture': 'url(\'/img/footer-texture.png\')',
      }),
    },
  },
}
```

</Customizing>

## Gradient Color Stops

Utilities for controlling the color stops in background gradients.

### Gradient From

<PlaygroundWithVariants
  variant='green-500'
  type='color'
  prefix='from'
  fixed='p-2 dark:text-white opacity-85 overflow-hidden'
  nested=true
  appended='h-36 w-36 rounded-md bg-gradient-to-r to-blue-500'
  html="&lt;div class=&quot;h-36 w-36 rounded-md bg-gradient-to-r {class} to-blue-500&quot;&gt;&lt;/div&gt;"
/>

### Gradient Via

<PlaygroundWithVariants
  variant='gray-500'
  type='color'
  prefix='via'
  fixed='p-2 dark:text-white opacity-85 overflow-hidden'
  nested=true
  appended='h-36 w-36 rounded-md bg-gradient-to-r from-red-500 to-blue-500'
  html="&lt;div class=&quot;h-36 w-36 rounded-md bg-gradient-to-r from-red-500 {class} to-blue-500&quot;&gt;&lt;/div&gt;"
/>

### Gradient To

<PlaygroundWithVariants
  variant='yellow-500'
  type='color'
  prefix='to'
  fixed='p-2 dark:text-white opacity-85 overflow-hidden'
  nested=true
  appended='h-36 w-36 rounded-md bg-gradient-to-r from-green-500'
  html="&lt;div class=&quot;h-36 w-36 rounded-md bg-gradient-to-r from-green-500 {class}&quot;&gt;&lt;/div&gt;"
/>

## Background Blend Mode

Utilities for controlling how an element's background image should blend with its background color.

<PlaygroundWithVariants
  variant='normal'
  :variants="['normal', 'multiply', 'screen', 'overlay', 'darken', 'lighten', 'color-dodge', 'color-burn', 'hard-light', 'soft-light', 'difference', 'exclusion', 'hue', 'saturation', 'color', 'luminosity']"
  prefix='bg-blend'
  fixed='dark:text-white opacity-85 overflow-hidden'
  nested=true
  appended='w-full h-36 bg-no-repeat bg-contain bg-center bg-green-300 rounded-md'
  html="&lt;div class=&quot;w-full h-36 bg-no-repeat bg-green-300 rounded-md bg-contain bg-center {class}&quot; style=&quot;background-image:url(&#39;/assets/bg-blue.svg&#39;);&quot;&gt;
  &lt;/div&gt;"
/>
