With `@vueuse/head`

<div class="grid grid-cols-2 gap-4">

<div v-click> 

```tsx
import { useHead } from '@vueuse/head'
useHead({
  title: 'Page Title',
  script: [
    {
      src: 'https://js.stripe.com/v3/',
      defer: true,
      onload: (e) => {
        console.log(e);
      },
    },
  ],
})
```
</div>

<div v-click="2">

```tsx
<script setup lang="ts">
import { Head } from '@vueuse/head'

</script>

<template>
  <Head>
    <title>{{ count }}</title>
    <html lang="en" />
    <body class="body" />
    <meta name="description" content="desc">
    <component is="style">
      body { background: lightgreen; } {{ style }}
    </component>
  </Head>
</template>
```

</div>
</div>