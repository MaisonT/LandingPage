<template>
  <div class="plan">
    <h3>{{name}}</h3>
    <p>{{ users }}</p>
    <hr>
    <h1><span>$</span>{{price}}</h1>
    <p>per month</p>
    <button>Order</button>
  </div>
</template>

<script>
export default {
  name: "PlanInfo",
  props: {
    name: String,
    price: String,
    users: String,
  }
}
</script>

<style scoped lang="scss">

.plan {
  width: 340px;
  height: 440px;
  box-shadow: 0 18px 50px -15px rgba(25, 42, 89, 0.2);
  border-radius: 30px;
  background: #0F1F4B;
  margin-right: 80px;

  h1 {
    font-weight: 700;
    font-size: 50px;
    line-height: 120%;
    text-align: center;
    color: #FFFFFF;
    margin: 0;
    span {
      font-size: 30px;
    }
  }
  h3 {
    padding-top: 50px;
    margin: 0 0 10px 0;
    font-weight: 700;
    font-size: 30px;
    line-height: 35px;
    text-align: center;
    color: #FFFFFF;
  }
  p {
    margin: 0;
  }
  hr {
    width: 220px;
    height: 1px;
    border: none;
    margin-top: 37px;
    margin-bottom: 28px;
    background: #2A407C;
  }
  button {
    cursor: pointer;
    align-items: center;
    padding: 10px 80px;
    width: 200px;
    height: 50px;
    border-radius: 68px;
    background: transparent;
    color: white;
    border: 1px solid #2A407C;
    margin-top: 42px;
  }
}
.plan:hover {
  background: #FFFFFF;
  hr {
    background: #D3D9E9;
  }
  h1, h3, span {
    color: black;
  }
  button {
    background: #EF2A82;
    border: none;
  }
}
</style>