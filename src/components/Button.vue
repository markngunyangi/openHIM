<template>
    <button @click="$emit('toggle')" class="btn" :style="{background:color}">{{ name }}</button>
</template>

<script>
export default{
    name: "Button",
    props: {
        name: String,
        color: String
    },

}
</script>

<style>
.btn {
  display: inline-block;
  background: #000;
  color: #fff;
  border: none;
  padding: 10px 20px;
  margin: 5px;
  border-radius: 5px;
  cursor: pointer;
  text-decoration: none;
  font-size: 15px;
  font-family: inherit;
}

.btn:focus {
  outline: none;
}

.btn:active {
  transform: scale(0.98);
}

.btn-block {
  display: block;
  width: 100%;
}
</style>