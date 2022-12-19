---
clicks: 9
---

# Typescript vs Javascript

<div class="grid grid-cols-2 gap-8">


<div v-click="1">

```js {all|all|9|9} 
const user = {
	first_name: "Christopher",
	last_name: "Reeve",
	email: "work@creeve.me",
	phone: "+62-851xx",
	age: 26,
}

console.log(user.full_name) // undefined
```

<arrow v-click="3" x1="180" y1="350" x2="200" y2="280" color="#564" width="2" arrowSize="3" />

<div class="mt-18" v-click="3">

`user.full_name is undefined`

</div>

</div>

<div v-click="4">

```ts {all|1-7|9-16|12} 
interface UserResponse{
	first_name: string;
	last_name: string;
	email: string;
	phone: string;
	age: number;
}

const user : UserResponse = {
	first_name: "Christopher",
	last_name: "Reeve",
	full_name : "Christopher Reeve",
	email: "reeve@creeve.me",
	phone: "+62-851xx",
	age: 26
}
```


<arrow v-click="9" x1="600" y1="450" x2="600" y2="330" color="#564" width="2" arrowSize="3" />

<img v-click="9"  src="/images/typescript/code-error.png" class="mt-12"/>
</div>

</div>



