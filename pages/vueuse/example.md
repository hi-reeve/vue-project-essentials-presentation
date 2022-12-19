# Example

<div class="grid ">


<div v-click="1">

<span>

[useTimeoutFn](https://vueuse.org/shared/useTimeoutFn/)

</span>

```ts
import { useTimeoutFn } from '@vueuse/core'

const { isPending, start, stop } = useTimeoutFn(() => {
  /* your code here */
}, 3000)
```

</div>


<div v-click="2">

<span>

[useMediaQuery](https://vueuse.org/core/usemediaquery/)

</span>

```ts
import { useMediaQuery } from '@vueuse/core'
import { computed } from 'vue'

const isLargeScreen = useMediaQuery('(min-width: 1024px)')
const isPreferredDark = useMediaQuery('(prefers-color-scheme: dark)')

const buttonText = computed(() => isLargeScreen ? 'Large' : 'Small')
```

</div>

</div>