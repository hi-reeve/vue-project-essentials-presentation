

<div class="grid grid-cols-2 gap-4">

<div >

Without `@vueuse/components`

```tsx
<script setup>
import { ref } from 'vue'
import { onClickOutside } from '@vueuse/core'

const el = ref()

function close () {
  /* ... */
}

onClickOutside(el, close)
</script>

<template>
  <div ref="el">
    Click Outside of Me
  </div>
</template>

```
</div>


<div v-click>

With `@vueuse/components`

```tsx
<script setup>
import { OnClickOutside } from '@vueuse/components'

function close () {
  /* ... */
}
</script>

<template>
  <OnClickOutside @trigger="close">
    <div>
      Click Outside of Me
    </div>
  </OnClickOutside>
</template>

```

</div>

</div>