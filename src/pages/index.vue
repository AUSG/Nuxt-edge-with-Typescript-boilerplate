<template>
  <div class="main">
    <div class="intro">
      <img src="img/awskurg.png"
        srcset="img/awskurg@2x.png 2x, img/awskurg@3x.png 3x"
        class="AWSKURG"/>
      <div class="slogun">
        <span>
          우리는 나누고 <br/>
          전파합니다
        </span>
      </div>
      <div class="grid">
        <pre class="AWSKRUG-2012-">
          <b>AWSKRUG</b>는 2012년 시작된 아마존 웹서비스 한국 사용자모임으로서, 
          <b>AWS클라우드</b>를 처음 배우는 분들로 부터 고급 개발자까지 정보 교류를
          위해 만들었습니다. 

          각종 반기 및 월간 세미나, 지역별 분야별 소모임 
          그리고 글로벌 유저그룹 연계 활동 등 다양한 프로젝트를 수행하고
          있으며, 자세한 내용은 아래 소개 자료를 참고하시기 바랍니다.
        </pre>
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
        <img src="img/slack.svg"
          class="slack">
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
  </div>
</template>

<script lang="ts">
import { Vue, Component, Prop } from "nuxt-property-decorator";

@Component({
  components: {}
})
export default class IndexPage extends Vue {}
</script>

<style>
.main {
  padding-top: 4em;
}

.intro {
  display: flex;
  justify-content: flex-end;
  flex-wrap: wrap;
}

.AWSKURG {
  width: 959px;
  height: 515px;
  object-fit: contain;
  opacity: 0.46;
  flex: 1;
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
  flex: 1;
}

.AWSKRUG-2012- {
  width: 740px;
  height: 315px;
  font-family: SpoqaHanSans;
  font-size: 25px;
  font-weight: 300;
  font-style: normal;
  font-stretch: normal;
  line-height: 1.8;
  letter-spacing: normal;
  color: #ffffff;
  border-top: solid 0.1em white;
}

.AWSKRUG-2012- .text-style-1 {
  font-family: Arial;
  font-weight: bold;
}

.AWSKRUG-2012- .text-style-2 {
  font-weight: bold;
}

.small_square {
  width: 188px;
  height: 188px;
  object-fit: contain;
}

.big_square {
  width: 263px;
  height: 263px;
  object-fit: contain;
}

.facebook .slack .github .slideshare {
  width: 188px;
  height: 188px;
  object-fit: contain;
}

</style>

