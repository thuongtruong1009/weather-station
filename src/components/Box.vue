<template>
  <form @submit.prevent="onSubmit">
    <input
      type="text"
      placeholder="Enter your city..."
      onfocus="this.placeholder = ''"
      onblur="this.placeholder = 'Enter your city...'"
      v-model="submitValue"
    />
    <input type="submit" />
    <svg class="search-icon" @click="onSubmit" viewBox="0 0 24 24">
      <path
        d="M15.5 14h-.79l-.28-.27C15.41 12.59 16 11.11 16 9.5 16 5.91 13.09 3 9.5 3S3 5.91 3 9.5 5.91 16 9.5 16c1.61 0 3.09-.59 4.23-1.57l.27.28v.79l5 4.99L20.49 19l-4.99-5zm-6 0C7.01 14 5 11.99 5 9.5S7.01 5 9.5 5 14 7.01 14 9.5 11.99 14 9.5 14z"
      />
      <path fill="none" d="M0 0h24v24H0z" />
    </svg>
  </form>
</template>

<script>
export default {
  data() {
    return {
      submitValue: "",
      tempValue: 23,
      descValue: "",
    };
  },
  methods: {
    onSubmit: function () {
      console.log("Hello OK");
    },
  },
};
</script>

<style scoped>
form {
  display: flex;
  justify-content: center;
  align-items: center;
  grid-gap: 15px;
  padding: 6px 0;
}
input[type="text"] {
  width: 70%;
  height: 35px;
  border-radius: 10px;
  border: none;
  outline: none;
  padding-left: 15px;
}
input[type="submit"] {
  width: 10%;
  height: 30px;
  display: none;
}
.search-icon {
  width: 10%;
  cursor: pointer;
  transform: translateY(3px);
  border-radius: 50%;
  transition: 0.3s;
}
.search-icon:hover {
  transform: scale(1.05) translateY(3px);
  box-shadow: 1px 1px 2px rgb(58, 58, 58);
}
</style>