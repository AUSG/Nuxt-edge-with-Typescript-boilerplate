<template>
  <div class="ausg">
    <div class="contents">
      <div class="box-1-1"><hr/></div>

      <div class="AWSKRUG box-1-2">
        <b>AWSKRUG 대학생</b> 그룹
      </div>

      <div class="box-2-2">
        <img src="img/group-3.png" class="Group-3">
        <div class="AUSG-IT" v-html="description"></div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { Vue, Component } from 'nuxt-property-decorator'

@Component
export default class AusgComponent extends Vue {
  description = `
  <b>AUSG</b>는 최신 IT기술과 클라우드에 대한 이해를 바탕으로 <b>AWS</b>를 학습하고 전파하는 대학생 그룹입니다.
  <br/><br/>
  <b>AWS</b>와 <b>AWSKRUG</b>의 지원을 받고 <b>AWSKRUG</b>에 소속되어 있습니다.
  `
}
</script>

<style scoped>
.contents {
  display: grid;
  grid-template-columns: 2fr 8fr;
}

.box-1-1 {
  /* grid-row: 1 / 2; */
  /* grid-column: 1 / 3; */
  grid-row-start: 1;
  grid-row-end: 2;
  grid-column-start: 1;
  grid-column-end: 2;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-content: center;
}

.box-1-2 {
  /* grid-row: 1 / 2;
  grid-column: 2 / 3; */
  grid-row-start: 1;
  grid-row-end: 2;
  grid-column-start: 2;
  grid-column-end: 3;
  padding-left: 0.5em;
}

.box-2-2 {
  /* grid-row: 2 / 2;
  grid-column: 2 / 3; */
  grid-row-start: 2;
  grid-row-end: 3;
  grid-column-start: 2;
  grid-column-end: 3;
}

hr {
  border: solid 1px white;
}

.AWSKRUG {
  /* width: 255px; */
  height: 37px;
  font-family: Arial;
  font-size: 25px;
  font-weight: normal;
  font-style: normal;
  font-stretch: normal;
  line-height: normal;
  letter-spacing: normal;
  color: #ffffff;
}

.AWSKRUG .text-style-1 {
  font-family: SpoqaHanSans;
  font-weight: bold;
}

.AWSKRUG .text-style-2 {
  font-family: SpoqaHanSans;
  font-weight: 300;
}

.Group-3 {
  width: 388px;
  height: 74px;
  object-fit: contain;
  margin-top: 5em;
}

.AUSG-IT {
  width: 699px;
  height: 185px;
  font-family: SpoqaHanSans;
  font-size: 25px;
  font-weight: 300;
  font-style: normal;
  font-stretch: normal;
  line-height: normal;
  letter-spacing: normal;
  color: #ffffff;

  margin-top: 3em;
  padding-left: 5em;
}

.AUSG-IT .text-style-1 {
  font-family: Arial;
  font-size: 27px;
  font-weight: bold;
}
</style>

