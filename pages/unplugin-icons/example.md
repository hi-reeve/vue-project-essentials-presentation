# Example

<br/>

<p>Two different way of using unplugin-icons</p>

<div class="grid grid-cols-2 gap-4">

<div>


```tsx
<script setup>
import IconAccessibility from '~icons/carbon/accessibility'
import IconAccountBox from '~icons/mdi/account-box'
</script>

<template>
  <icon-accessibility/>
  <icon-account-box style="font-size: 2em; color: red"/>
</template>
```

</div>


<div>


```html
<template>
  <icon:mdi:account />
</template>
```

</div>

</div>