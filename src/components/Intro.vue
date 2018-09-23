<template>
  <div class="intro">
    <div class="grid">
      <img src="img/awskurg.png"
        class="AWSKURG"/>
      <div class="slogun" v-html="slogun"></div>
      <div class="description" v-html="description"></div>
      <a class="facebook">
        <img src="img/facebook.svg"
          class="facebook">
      </a>
      <img src="img/small-square.png"
        srcset="img/small-square@2x.png 2x,
                img/small-square@3x.png 3x"
        class="small_square">
      <a class="slack">
        <img src="img/slack.svg"
          class="slack">
      </a>
      <a class="github">
        <img src="img/github.svg"
          class="github">
      </a>
      <img src="img/big-square.png"
        srcset="img/big-square@2x.png 2x,
                img/big-square@3x.png 3x"
        class="big_square">
      <a class="slideshare">
        <img src="img/slideshare.svg"
          class="slideshare">
      </a>
    </div>
  </div>
</template>

<script lang="ts">
import { Vue, Component } from 'nuxt-property-decorator'

@Component
export default class IntroComponent extends Vue {
  slogun = `
  우리는 나누고 <br/>
  전파합니다
  `
  description = `
  <b>AWSKRUG</b>는 2012년 시작된 아마존 웹서비스 한국 사용자모임으로서, <br/>
  <b>AWS클라우드</b>를 처음 배우는 분들로 부터 고급 개발자까지 정보 교류를
  위해 만들었습니다. <br/><br/>

  각종 반기 및 월간 세미나, 지역별 분야별 소모임 <br/>
  그리고 글로벌 유저그룹 연계 활동 등 다양한 프로젝트를 수행하고<br/>
  있으며, 자세한 내용은 아래 소개 자료를 참고하시기 바랍니다.
  `
}
</script>

<style scoped>
.intro {
  /* float: right; */
  padding-top: 17em;
  display: flex;
  flex-direction: column;
  align-items: flex-end;
}

.AWSKURG {
  width: 959px;
  height: 515px;
  object-fit: contain;
  opacity: 0.46;
  position: absolute;
  margin-top: -17em;
  margin-left: -21em;
  align-self: flex-start;
}

.grid {
  display: grid;
  grid-template-columns: repeat(5, auto);
}

.slogun {
  /* width: 546px;
  height: 240px; */
  font-family: AppleSDGothicNeo;
  font-size: 100px;
  font-weight: 800;
  font-style: normal;
  font-stretch: normal;
  line-height: normal;
  letter-spacing: normal;
  color: #ffffff;
  border-bottom: solid 1.5px white;
  grid-row-start: 1;
  grid-row-end: 2;
  grid-column-start: 1;
  grid-column-end: 6;
}

.description {
  width: 740px;
  height: 315px;
  font-family: SpoqaHanSans;
  font-size: 25px;
  font-weight: 300;
  font-style: normal;
  font-stretch: normal;
  line-height: 1.8;
  letter-spacing: normal;

  margin: 1em 0em;
  color: #ffffff;
  grid-column-start: 1;
  grid-column-end: 4;
  grid-row-start: 2;
  grid-row-end: 4;
}

.description .text-style-1 {
  font-family: Arial;
  font-weight: bold;
}

.description .text-style-2 {
  font-weight: bold;
}

.small_square {
  width: 188px;
  height: 188px;
  object-fit: contain;
  grid-column-start: 4;
  grid-column-end: 5;
  grid-row-start: 3;
  grid-row-end: 4;
}

.big_square {
  width: 263px;
  height: 263px;
  object-fit: contain;
  grid-column-start: 2;
  grid-column-end: 3;
  grid-row-start: 5;
  grid-row-end: 6;
}

.facebook .slack .github .slideshare {
  width: 188px;
  height: 188px;
  object-fit: contain;
}

.facebook {
  grid-column-start: 4;
  grid-column-end: 5;
  grid-row-start: 2;
  grid-row-end: 3;
}

.slack {
  grid-column-start: 5;
  grid-column-end: 6;
  grid-row-start: 3;
  grid-row-end: 4;
}

.github {
  grid-column-start: 3;
  grid-column-end: 4;
  grid-row-start: 4;
  grid-row-end: 5;
}

.slideshare {
  grid-column-start: 4;
  grid-column-end: 5;
  grid-row-start: 5;
  grid-row-end: 6;
}

</style>
