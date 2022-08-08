<template>
<div class="pricing-plan">
  <h2>Pricing Plans</h2>
  <p>
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Elementum nisi aliquet<br>
    volutpat pellentesque volutpat est.
  </p>
  <div class="plans-info">
    <div v-for="plan in plansInfo" :key="plan">
    <PlanInfo :name="plan.name" :price="plan.price" :users="plan.usersAllowed" />
    </div>
  </div>
</div>
</template>

<script>
import PlanInfo from "@/components/PlanInfo";
export default {
  name: "PricingPlan",
  components: {PlanInfo},
  data() {
    return {
      plansInfo: {
        starterPlan: {
          name: 'Starter',
          price: '29',
          usersAllowed: 'up to 3 users',
        },
        standardPlan: {
          name: 'Standard',
          price: '99',
          usersAllowed: 'up to 20 users',
        },
        premiumPlan: {
          name: 'Premium',
          price: '299',
          usersAllowed: 'up to 200 users',
        },
      },
    };
  },
}
</script>

<style scoped lang="scss">
.pricing-plan {
  width: 1180px;
  margin-left: auto;
  margin-right: auto;

  h2 {
    font-style: normal;
    font-weight: 700;
    font-size: 40px;
    line-height: 47px;
    text-align: center;
    color: #FFFFFF;
  }
  p {
    text-align: center;
  }

  .plans-info {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
  }
}
</style>