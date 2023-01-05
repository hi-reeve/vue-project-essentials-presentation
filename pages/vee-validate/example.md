# Example


<div class="grid grid-cols-2 gap-4">

<div>

`useField`
```tsx
<script setup>
import { useField } from 'vee-validate';
import * as yup from 'yup';

const { value, errorMessage } = useField('email', yup.string().email().required())

value.value = 1; // ⛔️  Error
value.value = 'test@example.com'; // ✅
</script>

<template>
	<input type="text" name="email" />
	<span v-if="errorMessage"> {{errorMessage}} </span>
<template>
```

</div>


<div>

`useForm`
```tsx
<script setup>
import { useField, useForm } from 'vee-validate';
import * as yup from 'yup';

const validationSchema = yup.object({
	email: yup.string().email().required()
})
const { handleSubmit } = useForm({
	validationSchema
});

const onSubmit = handleSubmit(values => {
  console.log(values)
});
</script>
<template>
	<form @submit="onSubmit">
		<input type="text" name="email" />
	</form>
</template>
```

</div>

</div>