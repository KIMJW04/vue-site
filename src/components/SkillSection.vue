<script setup>
import { skillText } from "@/constants";
</script>
<template>
  <section id="skill">
    <div class="skill__inner">
      <div class="skill__title">
        <h2>Challenge <em>나의 도전</em></h2>
      </div>
      <div class="skill__desc" :class="{ show: isNavVisible }">
        <div v-for="(text, index) in skillText" :key="index">
          <span>{{ index + 1 }}.</span>
          <h3>{{ text.title }}</h3>
          <p>{{ text.desc }}</p>
        </div>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
#skill {
  min-height: 100vh;
}
.skill__inner {
  padding: 16px;
  display: flex;
  justify-content: space-between;
  @media (max-width: 800px) {
    flex-direction: column;
  }
  .skill__title {
    position: sticky;
    top: 100px;
    left: 0;
    width: 48%;
    height: 5vw;
    h2 {
      font-size: 4vw;
      font-weight: 700;
      line-height: 0.8;
      text-transform: uppercase;
      color: var(--black100);
      border-bottom: 0.4vw solid var(--black100);
      @media (max-width: 800px) {
        margin-top: -30px;
        line-height: 1.5;
        background-color: var(--mainBg-color);
      }
      em {
        font-size: 1.25rem;
        font-weight: 700;
        line-height: 0.7;
        @media (max-width: 800px) {
          line-height: 1.5;
        }
      }
    }
    @media (max-width: 800px) {
      width: 100%;
      background-color: var(--mainBg-color);
    }
  }
  .skill__desc {
    width: 50%;
    span {
      font-size: 5vw;
      font-weight: 700;
      line-height: 1.3;
      font-family: var(--mainNum-font);
      @media (max-width: 800px) {
        margin-top: 50px;
        display: block;
        font-size: 7vw;
      }
    }
    h3 {
      font-size: 1.3rem;
      text-decoration: underline;
      text-underline-position: under;
      margin-bottom: 1vw;
      @media (max-width: 800px) {
        margin-bottom: 1.2vw;
        font-size: 1.8rem;
      }
    }
    p {
      margin-bottom: 30vh;
      font-size: 0.9rem;
      color: var(--black300);
      line-height: 1.8;
      @media (max-width: 800px) {
        font-size: 1.2rem;
        margin-bottom: 20vh;
      }
    }
    @media (max-width: 800px) {
      width: 100%;
    }
  }
}
</style>
