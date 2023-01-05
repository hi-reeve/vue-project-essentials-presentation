# Example

<div class="grid grid-cols-2 gap-4">

<div>
<span>Without Unplugin Vue Component</span>

```tsx
<template>
  <div>
    <HelloWorld msg="Hello Vue 3.0 + Vite" />
  </div>
</template>

<script>
import HelloWorld from './src/components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    HelloWorld
  }
}
</script>
```

</div>

<div>

<span>With Unplugin vue component</span>

```tsx
<template>
  <div>
    <HelloWorld msg="Hello Vue 3.0 + Vite" />
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>
```

</div>

</div>