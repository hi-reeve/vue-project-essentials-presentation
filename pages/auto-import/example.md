# Example

<br/>
<span>Without Unplugin auto import</span>

```ts
import { computed, ref } from 'vue'
const count = ref(0)
const doubled = computed(() => count.value * 2)
```

<span>With unplugin auto import</span>

```ts
const count = ref(0)
const doubled = computed(() => count.value * 2)
```