<template>
    <div>
        <h2> Pizza Name: {{pizzaName}}</h2>
        <p>Price: {{pizzaPrice}}</p>
        <p>Size: {{pizzaSize}}</p>
        <slot name='content'> </slot>
    </div>
</template>
<script>
export default {
    props: ['pizzaName','pizzaPrice', 'pizzaSize']   
}
</script>