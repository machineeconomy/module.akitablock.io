<template>
  <footer id="EngageNow" class="contain section">
    <div class="footer__information">
      <h3 class="title">The time to engage is now.</h3>
      <p class="text footer__text">
        Did our demonstration provide you a better understanding about the true power beyond blockchain?
        Then let's build a competitve advantage today to stay ahead of the competition:
      </p>
    </div>
    <div class="send__email">
      <a
        class="email__button"
        href="mailto:hello@akitablock.io?subject=Machine%20Economy%20Use%20Case"
      >
        <standartButton />
      </a>
    </div>
    <div class="network__icons">
      <ul>
        <li>
          <a href="https://twitter.com/AkitaBlock" target="_blank" class="network__link twitter"></a>
        </li>
        <li>
          <a
            href="https://www.linkedin.com/in/nino-ulrich"
            target="_blank"
            class="network__link linkedIn"
          ></a>
        </li>
        <li>
          <a href="https://github.com/machineeconomy" target="_blank" class="network__link gitHub"></a>
        </li>
        <li>
          <a href="https://www.iota.org" target="_blank" class="network__link iota"></a>
        </li>
      </ul>
    </div>
    <div class="contain">
      <span class="footer__background"></span>
      <div class="footer__bottom text">
        <span class="bottom__text">
          Open source project
          <br />made by AKITA
        </span>
        <a
          class="bottom__link"
          href="https://github.com/machineeconomy/m2m.akitablock.io/blob/master/Site%20Notice"
          target="_blank"
        >Site Notice</a>
      </div>
    </div>
  </footer>
</template>

<script>
import StandartButton from "../StandartButton";
export default {
  name: "Footer",
  components: {
    StandartButton
  }
};
</script>

<style lang="scss">
#EngageNow {
  position: relative;
}
.footer__background {
  display: block;
  position: absolute;
  bottom: 0;
  right: 0;
  width: 50%;
  height: 155%;
  background: url("./assets/MachineChain.png") no-repeat;
  background-size: 1400px;
}
.footer__information {
  max-width: 850px;
}
.send__email {
  margin: 30px 40px 80px;
}
.network__icons {
  margin: 50px 0px;
}
.network__icons ul {
  list-style: none;
  display: flex;
  padding: 0px;
}
.linkedIn {
  background: url("./assets/linkedin_logo.png");
}
.twitter {
  background: url("./assets/twitter_logo.png");
}
.gitHub {
  background: url("./assets/github_logo.png");
}
.iota {
  background: url("./assets/Iota_logo.png");
}
.network__link {
  display: block;
  height: 60px;
  width: 60px;
  margin: 0px 25px;
  background-size: 100%;
  background-repeat: no-repeat;
  &:hover {
    transform: scale(1.1);
  }
}
.footer__bottom {
  height: 80px;
  color: #fff;
  position: relative;
  z-index: 2;
  display: flex;
  font-weight: lighter;
}
.bottom__text {
  text-align: center;
  flex: 3 1 auto;
  margin: auto;
  line-height: 1;
}
.bottom__link {
  position: absolute;
  right: 10%;
  bottom: 30%;
  color: #fff;
  &:hover {
    color: #fff;
    text-decoration: underline;
  }
}
@media (max-width: 1750px) {
  .footer__background {
    height: 140%;
    background-size: 1200px;
  }
}
@media (max-width: 1500px) {
  .footer__background {
    height: 125%;
    background-size: 1000px;
  }
  .input__background {
    max-width: 500px;
  }
  .footer__information {
    max-width: 700px;
  }
}
@media (max-width: 1250px) {
  .footer__background {
    height: 115%;
    background-size: 800px;
  }
  .input__background {
    max-width: 400px;
  }
  .footer__information {
    max-width: 600px;
  }
}
@media (max-width: 1100px) {
  .footer__background {
    height: 90%;
    background-size: 600px;
  }
  .input__background {
    max-width: 330px;
  }
  .footer__information {
    max-width: 550px;
  }
}
@media (max-width: 1000px) {
  .footer__background {
    display: none;
  }
}
@media (max-width: 500px) {
  .network__link {
    width: 40px;
    height: 40px;
    margin: 0px 20px 0px 0px;
  }
  .bottom__link {
    position: static;
    flex: 1 1 auto;
    margin: auto;
  }
}
</style>