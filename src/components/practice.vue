<template>
  <div class="practice-practice">
    <div class="practice-heading">
      <h3 class="practice-header">{{ title }}</h3>
      <p class="practice-caption">{{ description }}</p>
    </div>
    <div class="read-more">
      <span class="practice-text">Read more</span>
      <img alt="image" src="/Icons/arrow-2.svg" class="practice-image" />
    </div>
  </div>
</template>

<script>
export default {
  name: 'Practice',
  props: {
    title: {
      type: String,
      default: 'Cardiology',
    },
    description: {
      type: String,
      default:
        'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt.',
    },
  },
}
</script>

<style scoped>
.practice-practice {
  gap: var(--dl-layout-space-oneandhalfunits);
  display: flex;
  position: relative;
  align-items: flex-start;
  padding-top: var(--dl-layout-space-threeunits);
  border-color: #B4B9C6;
  flex-direction: column;
  border-top-width: 1px;
}
 
.practice-heading {
  gap: var(--dl-layout-space-unit);
  display: flex;
  align-items: flex-start;
  flex-direction: column;
}
 
.practice-header {
  font-size: 30px;
  font-style: normal;
  font-weight: 600;
  line-height: 36px;
}
 
.practice-caption {
  max-width: 385px;
  line-height: 24px;
}
 
.practice-text {
  font-style: normal;
  font-weight: 600;
  line-height: 24px;
}
 
.practice-image {
  width: 12px;
  object-fit: cover;
}
 
@media(max-width: 767px) {
  .practice-practice {
    padding-top: var(--dl-layout-space-oneandhalfunits);
  }
  .practice-header {
    font-size: 20px;
    line-height: 24px;
  }
  .practice-caption {
    font-size: 14px;
    line-height: 21px;
  }
}
</style>
