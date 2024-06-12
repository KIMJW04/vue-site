<template>
  <section id="intro">
    <div class="intro__inner">
      <div class="intro__title">port developer</div>
      <div class="intro__lines" aria-hidden="true">
        <span class="line"></span>
        <span class="line"></span>
        <span class="line"></span>
        <span class="line"></span>
        <span class="line"></span>
        <span class="line"></span>
        <span class="line"></span>
      </div>
      <div class="intro__text">
        <div class="text">
          <div>talnet is</div>
          <div>Heart of Iron IV</div>
          <div>civilztion VI</div>
        </div>
        <div class="img">
          <img
            src="https://images.unsplash.com/photo-1610186594416-2c7c0131e35d?q=80&w=2787&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
            alt="나"
          />
        </div>
      </div>
      <div class="intro__lines bottom" aria-hidden="true">
        <span class="line"></span>
        <span class="line"></span>
        <span class="line"></span>
        <span class="line"></span>
        <span class="line"></span>
        <span class="line"></span>
        <span class="line"></span>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
#intro {
  height: 100vh;
  .intro__inner {
    width: 100%;
    height: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    padding: 16px;

    .intro__title {
      color: var(--black);
      font-family: var(--fontF);
      font-size: 12vw;
      line-height: 1;
      font-weight: 900;
      white-space: nowrap;
      text-transform: uppercase;
      letter-spacing: -0.3vw;
    }

    .intro__lines {
      width: 100%;
      display: flex;
      flex-direction: column;
      align-items: center;
      .line {
        display: block;
        width: 100%;
        height: 1px;
        background-color: var(--black);
        box-shadow: 0 10px 10px 3px var(--black100);
        margin-bottom: 0.63vw;
        &:nth-child(1) {
          width: 76%;
          height: 3px;
        }
        &:nth-child(2) {
          width: 80%;
          height: 4px;
        }
        &:nth-child(3) {
          width: 85%;
          height: 5px;
        }
        &:nth-child(4) {
          width: 89%;
          height: 6px;
        }
        &:nth-child(5) {
          width: 92%;
          height: 7px;
        }
        &:nth-child(6) {
          width: 96%;
          height: 8px;
        }
        &:nth-child(7) {
          width: 99%;
          height: 9px;
        }
      }
      &.bottom {
        display: none;
      }
    }

    .intro__text {
      width: 100%;
      height: 40vh;
      background-color: var(--black);
      color: var(--white);
      display: flex;
      align-items: center;
      justify-content: center;
      flex-direction: column;
      position: relative;
      .text {
        font-family: var(--fontF);
        color: var(--white200);
        font-size: 3vw;
        line-height: 1;
        font-weight: 900;
        text-transform: uppercase;
        text-decoration: underline;
        text-align: center;
        position: relative;
        z-index: 100;
        transition: all 0.6s;
        cursor: all-scroll;
        &:hover {
          opacity: 0.01;
          margin-bottom: -24px;
        }
      }
      .img {
        position: absolute;
        left: 50%;
        top: 50%;
        transform: translate(-50%, -50%);
        width: 30vh;
        height: 30vh;
        border-radius: 50%;
        overflow: hidden;
        filter: grayscale(100%);
        transition: all 0.3s;
      }
    }
  }
}
</style>
