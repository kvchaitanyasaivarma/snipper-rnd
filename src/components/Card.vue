<template>
  <div class="container">
    <div class="card">
      <div class="title">
        <h1>{{ Cardtitle }}</h1>
        <h2>"{{ Cardtags }}"</h2>
      </div>
      <div class="content">
        <div class="social">
          <textarea id="note"> {{ decodedMessage }} </textarea>
        </div>
      </div>
      <div class="circle"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Card',
  props: {
    Cardtitle: String,
    Cardtags: String,
    Cardcode: String,
  }//,
  //computed: {
    //decodedMessage() {
      // `this` points to the component instance
      //var de_code = btoa(this.Cardcode);
      //return this.de_code;
    //},
  //},
};
</script>

<style>
body {
  font-family: 'Roboto', sans-serif;
  background: #f0f5f9;
}
.card {
  position: relative;
  margin: 150px auto;
  width: 450px;
  padding: 20px;
  box-shadow: 3px 10px 20px rgba(0, 0, 0, 0.2);
  border-radius: 3px;
  border: 0;
  .circle {
    border-radius: 3px;
    width: 150px;
    height: 150px;
    background: black;
    position: absolute;
    right: 0px;
    top: 0;
    background-image: linear-gradient(to top, #fbc2eb 0%, #a6c1ee 100%);
    border-bottom-left-radius: 170px;
  }
  .content {
    margin-top: 25px;
    display: flex;
    flex-direction: column;
  }
  h1 {
    font-size: 34px;
    font-weight: bold;
    margin-bottom: 0;
  }
  h2 {
    font-size: 18px;
    letter-spacing: 0.5px;
    font-weight: 300;
  }
  .social {
    margin-bottom: 5px;
    a {
      text-decoration: none;
      color: black;
      margin-left: 8px;
      font-weight: 300;
      i {
        font-weight: 400;
      }
      textarea#note {
        width: 100%;
        direction: rtl;
        display: block;
        max-width: 100%;
        line-height: 1.5;
        padding: 15px 15px 30px;
        border-radius: 3px;
        border: 1px solid #f7e98d;
        font: 13px Tahoma, cursive;
        transition: box-shadow 0.5s ease;
        box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        font-smoothing: subpixel-antialiased;
        background: linear-gradient(#f9efaf, #f7e98d);
        background: -o-linear-gradient(#f9efaf, #f7e98d);
        background: -ms-linear-gradient(#f9efaf, #f7e98d);
        background: -moz-linear-gradient(#f9efaf, #f7e98d);
        background: -webkit-linear-gradient(#f9efaf, #f7e98d);
      }
    }
  }
  .location {
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    i {
      color: red;
    }
    p {
      font-weight: 300;
    }
  }
}
</style>
