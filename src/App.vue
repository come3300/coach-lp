<template>
 <div id="app">
<Header></Header>
<main>
      <div class="mv">
        <h2 class="mv-title">機械ではできない仕事を</h2>
        <div class="mv-card">
          <div class="mv-card-left">
            <p>2019/01/01</p>
            <p>ニュースタイトルがここに入ります。3月の決算報告書</p>
          </div>
          <div class="mv-card-right">
            <p>news</p>
          </div>
        </div>
      </div>
      <div class="mission">
        <div class="mission-text">
          <h2 class="mission-title">
            お客様のために進化する成長企業であり続ける
          </h2>
          <p class="mission-description">
            顧客主導型サービスを提供する企業として、お客様の会社経営に必要なサービスと情報を提供し続ける企業支援会社を目指します。<br />企業が現在直面している『勝ち取るため』の戦略を提供できる会社として、ホームページをはじめ、各種マーケティングをご提供いたし<br />ます。
          </p>
          <button class="mission-button">ミッション詳細</button>
        </div>
        <img src="./img2/mission-img.jpg" alt="" />
      </div>
      <div class="service">
        <div class="service-list">
          <h2 class="service-title">service</h2>
          <div class="service-list-top">
            <h3 class="service-list-title">web制作事業</h3>
            <h4 class="service-list-subtitle">コーチングのミッション</h4>
            <p class="service-list-description">
              ユーザーが求める物を分析し、ユーザービリティを備えた最適なサイトを提供。建<br />設業から美容、ブライダル、飲食店まで多種多様な業種の制作実績があります
            </p>
            <div class="service-list-button">
              <button>サービス詳細</button>
            </div>
          </div>
          <img class="service-top-img" src="./img2/service2.jpg" alt="" />
          <div class="service-list-bottom">
            <h3 class="service-list-title">web制作事業</h3>
            <h4 class="service-list-subtitle">コーチングのミッション</h4>
            <p class="service-list-description">
              ユーザーが求める物を分析し、ユーザービリティを備えた最適なサイトを提供。建<br />設業から美容、ブライダル、飲食店まで多種多様な業種の制作実績があります
            </p>
            <div class="service-list-button">
              <button>サービス詳細</button>
            </div>
          </div>
          <img class="service-bottom-img" src="./img2/service1.jpg" alt="" />
        </div>
      </div>
      <div class="company-list">
        <div class="company">
          <div class="company-content" v-for="(data,index)in company2" :key="index">
            <h2>{{data.name}}</h2>
            <p>{{data.this}}</p>
          </div>
        </div>
      </div>
      <div class="faq">
        <h2>FAQ</h2>
        <p>よくある質問</p>
      </div>
      <div class="contact">
        <div class="contact-inner">
          <h2 class="contact-title">contact</h2>
          <p class="contact-subtitle">お問い合わせ</p>
          <p class="contact-copy">お気軽にお問い合わせください</p>
          <p class="contact-description">
            資料請求・お問い合わせなどお問い合わせなどなんでも気軽に問い合わせください。お仕事のご連絡もお問い合わせページに飛んでいただいて、入力フォームにご記入お願いいたします。
          </p>
          <div class="contact-button">
            <button>お問い合わせへ</button>
          </div>
        </div>
      </div>
    </main>
<Footer></Footer>
 </div>
</template>

<script>
import Header from"../src/Header"
import Footer from"../src/Footer"
export default {
  data(){
    return{
      company2: [
       { name:"company",
        this: "会社概要"
       },

       {
         name:"recruit",
         this:"採用情報"
       }
      ]
    };
  },
  components:{
Header,
Footer
  }
};
</script>





<style>
html,
body,
div,
span,
object,
iframe,
h1,
h2,
h3,
h4,
h5,
h6,
p,
blockquote,
pre,
abbr,
address,
cite,
code,
del,
dfn,
em,
img,
ins,
kbd,
q,
samp,
small,
strong,
sub,
sup,
var,
b,
i,
dl,
dt,
dd,
ol,
ul,
li,
fieldset,
form,
label,
legend,
table,
caption,
tbody,
tfoot,
thead,
tr,
th,
td,
article,
aside,
canvas,
details,
figcaption,
figure,
footer,
header,
hgroup,
menu,
nav,
section,
summary,
time,
mark,
audio,
video {
  margin: 0;
  padding: 0;
  border: 0;
  outline: 0;
  font-size: 100%;
  vertical-align: baseline;
  background: transparent;
}

body {
  line-height: 1;
}

article,
aside,
details,
figcaption,
figure,
footer,
header,
hgroup,
menu,
nav,
section {
  display: block;
}

nav ul {
  list-style: none;
}

blockquote,
q {
  quotes: none;
}

blockquote:before,
blockquote:after,
q:before,
q:after {
  content: "";
  content: none;
}

a {
  margin: 0;
  padding: 0;
  font-size: 100%;
  vertical-align: baseline;
  background: transparent;
}

/* change colours to suit your needs */
ins {
  background-color: #ff9;
  color: #000;
  text-decoration: none;
}

/* change colours to suit your needs */
mark {
  background-color: #ff9;
  color: #000;
  font-style: italic;
  font-weight: bold;
}

del {
  text-decoration: line-through;
}

abbr[title],
dfn[title] {
  border-bottom: 1px dotted;
  cursor: help;
}

table {
  border-collapse: collapse;
  border-spacing: 0;
}

/* change border colour to suit your needs */
hr {
  display: block;
  height: 1px;
  border: 0;
  border-top: 1px solid #cccccc;
  margin: 1em 0;
  padding: 0;
}

input,
select {
  vertical-align: middle;
}

.mv {
  background-image: url(../img/eyecatch.jpg);
  background-position: center center;
  background-size: 100% 100%;
  background-repeat: no-repeat;
  height: 80vh;
  position: relative;
}

.mv-title {
  color: white;
  font-size: 40px;
  font-weight: bold;
  position: absolute;
  top: 60%;
  left: 15%;
}

.mv-card {
  background: white;
  width: 40%;
  height: 50px;
  font-size: 14px;
  display: flex;
  justify-content: space-between;
  position: absolute;
  right: 0;
  bottom: 0;
}

.mv-card-right {
  background: black;
  width: 25%;
  color: white;
  font-size: 14px;
  font-weight: bold;
  text-align: center;
  line-height: 50px;
}

.mission {
  background-color: black;
  height: 500px;
  position: relative;
}

.mission-text {
  color: white;
  position: absolute;
  top: 30%;
  left: 10%;
  z-index: 1;
}

.mission-title {
  font-size: 20px;
  padding-bottom: 20px;
}

.mission-button {
  margin-top: 20px;
  padding: 10px;
}

.mission img {
  width: 400px;
  height: auto;
  position: absolute;
  top: 30%;
  right: 10%;
}

.service {
  background-color: rgb(209, 209, 209);
  height: 1200px;
  margin-top: 100px;
  padding: 40px;
  position: relative;
}

.service-title {
  text-align: center;
  font-size: 30px;
  color: rgb(110, 108, 108);
}

.service-list-top {
  background-color: white;
  position: absolute;
  left: 15%;
  top: 20%;
  padding: 60px 40px;
  z-index: 1;
  font-size: 14px;
}

.service-list-subtitle {
  margin-top: 20px;
  font-weight: normal;
}

.service-list-description {
  margin-top: 20px;
}

.service-list-button {
  margin-top: 20px;
  text-align: right;
}

.service-list-button button {
  background-color: #fff;
  border: none;
  border: 1px solid #000;
  padding: 5px 10px;
}

.service-top-img {
  position: absolute;
  top: 10%;
  right: 0;
  width: 50%;
  height: auto;
}

.service-list-bottom {
  background-color: white;
  position: absolute;
  right: 15%;
  bottom: 15%;
  padding: 60px 40px;
  z-index: 1;
  font-size: 14px;
}

.service-bottom-img {
  position: absolute;
  bottom: 10%;
  left: 0;
  width: 50%;
  height: auto;
}

.company-list {
  margin-top: 100px;
  display: flex;
  justify-content: space-between;
}

.company {
  background-image: url(../img/company.jpeg);
  background-size: cover;
  background-position: center;
  width: 48%;
  height: 300px;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  color: #fff;
}


.company-content h2{
  font-size: 24px;
  margin-bottom: 10px;
}

.faq {
  color: white;
  background-color: black;
  height: 100px;
  width: 900px;
  margin: 80px auto;
  display: flex;
  align-items: center;
  position: relative;
}

.faq h2 {
  font-size: 30px;
  margin-left: 20px;
}

.faq p {
  position: absolute;
  left: 50%;
  transform: translateX(-50%);
}

.contact {
  background-image: url(../img/contact-bg.jpg);
  height: 600px;
  background-size: cover;
  color: white;
  text-align: center;
  display: flex;
  justify-content: center;
  align-items: center;
}

.contact-title {
  font-size: 30px;
}

.contact-subtitle {
  margin-top: 15px;
}

.contact-copy {
  font-size: 24px;
  margin-top: 20px;
}

.contact-description {
  margin-top: 20px;
  font-size: 14px;
}

.contact-button button {
  background-color: transparent;
  border: none;
  border: 1px solid #fff;
  color: #fff;
  padding: 5px 10px;
  margin-top: 20px;
}

@media screen and (max-width: 480px) {
  .mv {
    display: block;
  }

  .mv-card {
    position: absolute;
    width: 100%;
  }

  .mission {
    position: relative;
  }

  .mission-title {
    font-size: 40px;
    line-height: 130%;
  }

  .mission-description {
    line-height: 130%;
  }

  .mission img {
    position: absolute;
    right: 0;
    top: 90%;

    height: 100px;
    width: 100px;
  }

  .service {
    display: block;
    position: relative;
  }

  .service-top-img {
    width: 85%;
    position: absolute;
    right: 6%;
    top: 8%;
  }

  .service-list-top {
    position: absolute;
    top: 24.5%;
    left: 9%;
    right: 6%;
  }

  .service-list-description {
    line-height: 135%;
  }

  .service-bottom-img {
    width: 87%;
    height: 20%;
    position: absolute;
    top: 55%;
    left: 8%;
  }

  .service-list-bottom {
    position: absolute;
    top: 75%;
    left: 8%;
    right: 5%;
    height: 14%;
  }

  .company-list {
    display: block;

    font-size: 200%;
  }

  .company {
    width: 480px;
    width: 100%;
  }


  .faq {
    width: 100%;
  }

  .contact {
    font-size: 200%;
  }
}
</style>